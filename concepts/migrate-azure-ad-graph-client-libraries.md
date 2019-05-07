---
title: Migrar aplicativos do Azure AD Graph .NET para o Microsoft Graph
description: Descreve como migrar aplicativos de API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fbc7c7550cda7654f603feeafb17ff3f0eb281e1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630255"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="e0d82-103">Migrar o .NET Client library use para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e0d82-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="e0d82-104">Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="e0d82-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="e0d82-105">Se seu aplicativo usa atualmente a biblioteca de cliente do Azure AD Graph, alterne para a [biblioteca de cliente .net do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span><span class="sxs-lookup"><span data-stu-id="e0d82-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="e0d82-106">Observação: a biblioteca de cliente .NET do Microsoft Graph só tem suporte para o .NET Framework 4,5 e o .NET Standard 1,1.</span><span class="sxs-lookup"><span data-stu-id="e0d82-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="e0d82-107">No entanto, consulte a biblioteca de cliente .NET do Microsoft Graph para obter as informações mais recentes sobre suporte.</span><span class="sxs-lookup"><span data-stu-id="e0d82-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="e0d82-108">Veja aqui algumas etapas gerais para migrar para a biblioteca de cliente .NET do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="e0d82-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="e0d82-109">Como criar um cliente do Microsoft Graph, dado um token de acesso (que você pode adquirir usando ADAL ou MSAL)</span><span class="sxs-lookup"><span data-stu-id="e0d82-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="e0d82-110">Como formular solicitações</span><span class="sxs-lookup"><span data-stu-id="e0d82-110">How to formulate requests</span></span>
- <span data-ttu-id="e0d82-111">Como usar construtores de consulta</span><span class="sxs-lookup"><span data-stu-id="e0d82-111">How to use query builders</span></span>
- <span data-ttu-id="e0d82-112">Como lidar com coleções e paginação</span><span class="sxs-lookup"><span data-stu-id="e0d82-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="e0d82-113">Visão geral das etapas de migração</span><span class="sxs-lookup"><span data-stu-id="e0d82-113">Overview of the migration steps</span></span>

<span data-ttu-id="e0d82-114">As etapas a seguir supõem que o seu aplicativo já esteja usando a ADAL para adquirir tokens de acesso para chamar o Azure AD Graph e que, por enquanto, você continuará a usar a ADAL.</span><span class="sxs-lookup"><span data-stu-id="e0d82-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="e0d82-115">Mudar para o MSAL pode ser feito como uma etapa separada descrita na [migração para o MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).</span><span class="sxs-lookup"><span data-stu-id="e0d82-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).</span></span>

1. <span data-ttu-id="e0d82-116">Para adquirir um token de acesso ao Microsoft Graph, \*\*\*\* atualize o `https://graph.windows.net` resourceurl pela `https://graph.microsoft.com`de para.</span><span class="sxs-lookup"><span data-stu-id="e0d82-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="e0d82-117">Em seu aplicativo, atualize as referências à biblioteca de cliente do Microsoft Graph alterando:</span><span class="sxs-lookup"><span data-stu-id="e0d82-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="e0d82-118">Para:</span><span class="sxs-lookup"><span data-stu-id="e0d82-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="e0d82-119">Use o Gerenciador de pacotes para baixar e atualizar o [pacote NuGet do Microsoft Graph](https://www.nuget.org/packages/Microsoft.Graph/) e atualizar as dependências.</span><span class="sxs-lookup"><span data-stu-id="e0d82-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="e0d82-120">Atualize o construtor de cliente para criar `GraphServiceClient`um, em `ActiveDirectoryClient`vez de.</span><span class="sxs-lookup"><span data-stu-id="e0d82-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="e0d82-121">Os trechos de código a seguir pressupõem que seu `AcquireTokenAsyncForUser()` aplicativo está usando o método para adquirir novos tokens.</span><span class="sxs-lookup"><span data-stu-id="e0d82-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="e0d82-122">Você pode encontrar uma definição para este método como parte do [exemplo Active-Directory-dotnet-graphapi-console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span><span class="sxs-lookup"><span data-stu-id="e0d82-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="e0d82-123">Trocar</span><span class="sxs-lookup"><span data-stu-id="e0d82-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () =\> await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="e0d82-124">Para:</span><span class="sxs-lookup"><span data-stu-id="e0d82-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="e0d82-125">Para a biblioteca de cliente do Microsoft `serviceRoot` Graph, o valor também inclui o número da versão.</span><span class="sxs-lookup"><span data-stu-id="e0d82-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="e0d82-126">No momento, esse valor `https://graph.microsoft.com/v1.0`é.</span><span class="sxs-lookup"><span data-stu-id="e0d82-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="e0d82-127">Atualizar solicitações para usar a sintaxe do construtor de solicitação do cliente Microsoft Graph, alterando:</span><span class="sxs-lookup"><span data-stu-id="e0d82-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="e0d82-128">Para:</span><span class="sxs-lookup"><span data-stu-id="e0d82-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    [!NOTE]
    <span data-ttu-id="e0d82-129">A biblioteca de cliente do Azure AD Graph oferece suporte à sintaxe de consulta baseada em LINQ.</span><span class="sxs-lookup"><span data-stu-id="e0d82-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="e0d82-130">No entanto, a biblioteca de cliente do Microsoft Graph não.</span><span class="sxs-lookup"><span data-stu-id="e0d82-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="e0d82-131">Consequentemente, você precisará converter as consultas relevantes para uma expressão mais RESTful.</span><span class="sxs-lookup"><span data-stu-id="e0d82-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="e0d82-132">Para fazer isso, altere:</span><span class="sxs-lookup"><span data-stu-id="e0d82-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g =\> g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="e0d82-133">Para:</span><span class="sxs-lookup"><span data-stu-id="e0d82-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="e0d82-134">Se suas páginas de código por meio de coleções, faça os seguintes ajustes secundários.</span><span class="sxs-lookup"><span data-stu-id="e0d82-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="e0d82-135">O exemplo a seguir compara e contrasta a busca de um grupo e uma paginação por meio de seus membros, 5 por vez.</span><span class="sxs-lookup"><span data-stu-id="e0d82-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="e0d82-136">Embora o código do Microsoft Azure AD Graph exija uma construção de busca para buscar membros de um grupo, o Microsoft Graph não tem essa exigência.</span><span class="sxs-lookup"><span data-stu-id="e0d82-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="e0d82-137">Além de isso, o código é relativamente semelhante.</span><span class="sxs-lookup"><span data-stu-id="e0d82-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="e0d82-138">Para ser conciso, somente os membros do usuário são exibidos, as condições de try/catch e de erro não são mostradas, e os trechos de código são para um aplicativo de console de thread único.</span><span class="sxs-lookup"><span data-stu-id="e0d82-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="e0d82-139">Por exemplo, altere o código a seguir usando a biblioteca de cliente .NET do Azure AD Graph:</span><span class="sxs-lookup"><span data-stu-id="e0d82-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

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

    <span data-ttu-id="e0d82-140">Para o código a seguir usando a biblioteca de cliente .NET do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="e0d82-140">To the following code using the Microsoft Graph .NET client library:</span></span>

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

7. <span data-ttu-id="e0d82-141">Criar e corrigir qualquer recurso, propriedade, navegação e erros de ação de serviço, geralmente relacionados a alterações de nome.</span><span class="sxs-lookup"><span data-stu-id="e0d82-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="e0d82-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="e0d82-142">See also</span></span>

<span data-ttu-id="e0d82-143">O [aplicativo trechos de console C#](https://github.com/microsoftgraph/console-csharp-snippets-sample) realça mais das diferenças entre a biblioteca de cliente do Microsoft Graph e a biblioteca de cliente do Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="e0d82-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="e0d82-144">A biblioteca de cliente do Azure AD Graph oferece suporte somente à plataforma .NET.</span><span class="sxs-lookup"><span data-stu-id="e0d82-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="e0d82-145">No entanto, a biblioteca de cliente do Microsoft Graph oferece suporte a [plataformas e idiomas](/graph) adicionais que podem ser úteis para suas soluções.</span><span class="sxs-lookup"><span data-stu-id="e0d82-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e0d82-146">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="e0d82-146">Next Steps</span></span>

- <span data-ttu-id="e0d82-147">Saiba como [implantar, testar e estender](/graph/migrate-azure-ad-graph-deploy-test-extend) aplicativos que você migrou para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e0d82-147">Learn how to [deploy, test, and extend](/graph/migrate-azure-ad-graph-deploy-test-extend) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="e0d82-148">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="e0d82-148">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="e0d82-149">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e0d82-149">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
