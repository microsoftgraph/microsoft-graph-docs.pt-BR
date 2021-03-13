---
title: Migrar aplicativos do Azure AD Graph .NET para o Microsoft Graph
description: Descreve como migrar aplicativos de API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 286f631a9d5787d972e8d7db2559b0c359384c75
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761294"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="ca475-103">Migrar o uso da biblioteca de clientes .NET para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca475-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="ca475-104">Este artigo faz parte da *etapa 3:* revisar detalhes do aplicativo do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="ca475-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="ca475-105">Se seu aplicativo atualmente usa a biblioteca de clientes do Azure AD Graph, alternar para a biblioteca de clientes [do Microsoft Graph .NET](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span><span class="sxs-lookup"><span data-stu-id="ca475-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="ca475-106">OBSERVAÇÃO: a biblioteca de clientes do Microsoft Graph .NET só tem suporte para .NET Framework 4.5 e .NET Standard 1.1.</span><span class="sxs-lookup"><span data-stu-id="ca475-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="ca475-107">No entanto, consulte a biblioteca de clientes do Microsoft Graph .NET para obter as informações de suporte mais recentes.</span><span class="sxs-lookup"><span data-stu-id="ca475-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="ca475-108">Aqui, vamos ver algumas etapas gerais para migrar para a biblioteca de clientes do Microsoft Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="ca475-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="ca475-109">Como criar um cliente do Microsoft Graph, dado um token de acesso (que você pode adquirir usando ADAL ou MSAL)</span><span class="sxs-lookup"><span data-stu-id="ca475-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="ca475-110">Como formular solicitações</span><span class="sxs-lookup"><span data-stu-id="ca475-110">How to formulate requests</span></span>
- <span data-ttu-id="ca475-111">Como usar construtores de consulta</span><span class="sxs-lookup"><span data-stu-id="ca475-111">How to use query builders</span></span>
- <span data-ttu-id="ca475-112">Como lidar com coleções e pajamento</span><span class="sxs-lookup"><span data-stu-id="ca475-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="ca475-113">Visão geral das etapas de migração</span><span class="sxs-lookup"><span data-stu-id="ca475-113">Overview of the migration steps</span></span>

<span data-ttu-id="ca475-114">As etapas a seguir pressuem que seu aplicativo já está usando o ADAL para adquirir tokens de acesso para chamar o Azure AD Graph e que, por enquanto, você continuará a usar o ADAL.</span><span class="sxs-lookup"><span data-stu-id="ca475-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="ca475-115">Alternar para MSAL pode ser feito como uma etapa separada descrita na [migração para MSAL](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal).</span><span class="sxs-lookup"><span data-stu-id="ca475-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal).</span></span>

1. <span data-ttu-id="ca475-116">Para adquirir um token de acesso ao Microsoft Graph, atualize **resourceUrl** `https://graph.windows.net` de para `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="ca475-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="ca475-117">Em seu aplicativo, atualize referências à biblioteca de clientes do Microsoft Graph alterando:</span><span class="sxs-lookup"><span data-stu-id="ca475-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="ca475-118">Para:</span><span class="sxs-lookup"><span data-stu-id="ca475-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="ca475-119">Use seu gerenciador de pacotes para baixar e atualizar o [pacote nuGet do Microsoft Graph](https://www.nuget.org/packages/Microsoft.Graph/) e atualizar dependências.</span><span class="sxs-lookup"><span data-stu-id="ca475-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="ca475-120">Atualize o construtor do cliente para criar `GraphServiceClient` um , em vez de `ActiveDirectoryClient` .</span><span class="sxs-lookup"><span data-stu-id="ca475-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="ca475-121">Os trechos de código a seguir pressuem que seu aplicativo está usando o `AcquireTokenAsyncForUser()` método para adquirir novos tokens.</span><span class="sxs-lookup"><span data-stu-id="ca475-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="ca475-122">Você pode encontrar uma definição para esse método como parte do exemplo [active-directory-dotnet-graphapi-console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span><span class="sxs-lookup"><span data-stu-id="ca475-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="ca475-123">Alterar:</span><span class="sxs-lookup"><span data-stu-id="ca475-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="ca475-124">Para:</span><span class="sxs-lookup"><span data-stu-id="ca475-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="ca475-125">Para a biblioteca de clientes do Microsoft Graph, `serviceRoot` o valor também inclui o número da versão.</span><span class="sxs-lookup"><span data-stu-id="ca475-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="ca475-126">Atualmente, esse valor é `https://graph.microsoft.com/v1.0` .</span><span class="sxs-lookup"><span data-stu-id="ca475-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="ca475-127">Atualizar solicitações para usar a sintaxe do construtor de solicitações de cliente do Microsoft Graph, alterando:</span><span class="sxs-lookup"><span data-stu-id="ca475-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="ca475-128">Para:</span><span class="sxs-lookup"><span data-stu-id="ca475-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    ><span data-ttu-id="ca475-129">A biblioteca de clientes do Azure AD Graph suportava sintaxe de consulta baseada em LINQ.</span><span class="sxs-lookup"><span data-stu-id="ca475-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="ca475-130">No entanto, a biblioteca de clientes do Microsoft Graph não.</span><span class="sxs-lookup"><span data-stu-id="ca475-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="ca475-131">Consequentemente, você precisará converter as consultas relevantes em uma expressão mais RESTful.</span><span class="sxs-lookup"><span data-stu-id="ca475-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="ca475-132">Para fazer isso, altere:</span><span class="sxs-lookup"><span data-stu-id="ca475-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="ca475-133">Para:</span><span class="sxs-lookup"><span data-stu-id="ca475-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="ca475-134">Se seu código for páginas por coleções, faça os seguintes ajustes secundários.</span><span class="sxs-lookup"><span data-stu-id="ca475-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="ca475-135">O exemplo a seguir compara e contrasta a busca de um grupo e a paagem através de seus membros, 5 de cada vez.</span><span class="sxs-lookup"><span data-stu-id="ca475-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="ca475-136">Embora o código do Azure AD Graph exija uma construção de buscador para buscar os membros de um grupo, o Microsoft Graph não tem esse requisito.</span><span class="sxs-lookup"><span data-stu-id="ca475-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="ca475-137">Fora isso, o código é relativamente semelhante.</span><span class="sxs-lookup"><span data-stu-id="ca475-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="ca475-138">Para ser conciso, apenas os membros do usuário são exibidos, as condições de tentativa/captura e erro não são mostradas e os trechos de código são para um aplicativo de console de thread único.</span><span class="sxs-lookup"><span data-stu-id="ca475-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="ca475-139">Como exemplo, altere o código a seguir usando a biblioteca de clientes do Azure AD Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="ca475-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

    ```csharp
    Group retrievedGroup = client.Groups.
        Where(g => g.ObjectId.Equals(id)).ExecuteAsync().Result;
    IGroupFetcher retrievedGroupFetcher = (IGroupFetcher) retrievedGroup;

    var membersPage = retrievedGroupFetcher.Members.Take(5).ExecuteAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<IDirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (IDirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        membersPage = membersPage.GetNextPageAsync().Result;
    } while (membersPage != null);

    ```

    <span data-ttu-id="ca475-140">Para o código a seguir usando a biblioteca de clientes do Microsoft Graph .NET:</span><span class="sxs-lookup"><span data-stu-id="ca475-140">To the following code using the Microsoft Graph .NET client library:</span></span>

    ```csharp
    var membersPage = client.Groups[id].Members.Request().Top(5).GetAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<DirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (DirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        if (membersPage.NextPageRequest != null)
            membersPage = membersPage.NextPageRequest.GetAsync().Result;
        else membersPage = null;
    } while (membersPage != null);

    ```

7. <span data-ttu-id="ca475-141">Crie e corrige qualquer recurso, propriedade, navegação e erros de ação de serviço, geralmente relacionados a alterações de nome.</span><span class="sxs-lookup"><span data-stu-id="ca475-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="ca475-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca475-142">See also</span></span>

<span data-ttu-id="ca475-143">O [C# de console](https://github.com/microsoftgraph/console-csharp-snippets-sample) realça mais das diferenças entre a biblioteca de clientes do Microsoft Graph e a biblioteca de clientes do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="ca475-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="ca475-144">A biblioteca de clientes do Azure AD Graph dá suporte apenas à plataforma .NET.</span><span class="sxs-lookup"><span data-stu-id="ca475-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="ca475-145">No entanto, a biblioteca de clientes do Microsoft Graph oferece suporte a [plataformas](/graph) e idiomas adicionais que podem ser mais úteis para suas soluções.</span><span class="sxs-lookup"><span data-stu-id="ca475-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ca475-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ca475-146">Next Steps</span></span>

- <span data-ttu-id="ca475-147">Saiba como [implantar, testar e estender](./migrate-azure-ad-graph-deploy-test-extend.md) aplicativos que você migrou para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ca475-147">Learn how to [deploy, test, and extend](./migrate-azure-ad-graph-deploy-test-extend.md) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="ca475-148">Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.</span><span class="sxs-lookup"><span data-stu-id="ca475-148">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
