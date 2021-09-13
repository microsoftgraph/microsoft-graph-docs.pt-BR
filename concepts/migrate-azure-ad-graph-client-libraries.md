---
title: Migrar Azure Active Directory (Azure AD) Graph aplicativos .NET para o Microsoft Graph
description: Descreve como migrar o Azure Active Directory (Azure AD) Graph aplicativos de API para a API Graph Microsoft.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: b774b14ffc480ca889392c31b2090c7578dfa207
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135960"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>Migrar o uso da biblioteca de clientes .NET para o Microsoft Graph

Este artigo faz parte da *etapa 3:* revisar detalhes do aplicativo do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Se o aplicativo atualmente usa a biblioteca de Azure Active Directory (Azure AD) Graph cliente, alternar para a biblioteca de clientes [do Microsoft Graph .NET.](https://github.com/microsoftgraph/msgraph-sdk-dotnet)

>OBSERVAÇÃO: a biblioteca de clientes do Microsoft Graph .NET só tem suporte para .NET Framework 4.5 e .NET Standard 1.1.  No entanto, consulte a biblioteca de clientes do Microsoft Graph .NET para obter as informações de suporte mais recentes.

Aqui, vamos ver algumas etapas gerais para migrar para a biblioteca de clientes do Microsoft Graph .NET:

- Como criar um cliente microsoft Graph, dado um token de acesso (que você pode adquirir usando a Biblioteca de Autenticação Azure Active Directory (ADAL) ou a Biblioteca de Autenticação da Microsoft (MSAL))
- Como formular solicitações
- Como usar construtores de consulta
- Como lidar com coleções e pajamento  

## <a name="overview-of-the-migration-steps"></a>Visão geral das etapas de migração

As etapas a seguir pressuem que seu aplicativo já está usando o ADAL para adquirir tokens de acesso para chamar o Azure AD Graph e que, por enquanto, você continuará a usar o ADAL. Alternar para MSAL pode ser feito como uma etapa separada descrita na [migração para MSAL](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal).

1. Para adquirir um token de acesso ao Microsoft Graph, atualize **resourceUrl** `https://graph.windows.net` de para `https://graph.microsoft.com` .

2. Em seu aplicativo, atualize referências à biblioteca de Graph cliente da Microsoft alterando:

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    Para:

    ``` csharp
    using Microsoft.Graph;
    ```

3. Use seu gerenciador de pacotes para baixar e atualizar as [dependências](https://www.nuget.org/packages/Microsoft.Graph/) do pacote Graph NuGet microsoft e atualizar.

4. Atualize o construtor do cliente para criar `GraphServiceClient` um , em vez de `ActiveDirectoryClient` .  Os trechos de código a seguir pressuem que seu aplicativo está usando o `AcquireTokenAsyncForUser()` método para adquirir novos tokens. Você pode encontrar uma definição para esse método como parte do exemplo [active-directory-dotnet-graphapi-console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).

    Alterar:

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    Para:

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    Para a Graph cliente da Microsoft, `serviceRoot` o valor também inclui o número da versão. Atualmente, esse valor é `https://graph.microsoft.com/v1.0` .

5. Atualize solicitações para usar Graph de construtor de solicitações de cliente da Microsoft, alterando:

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    Para:

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    >A biblioteca de clientes do Azure AD Graph com suporte à sintaxe de consulta baseada em LINQ. No entanto, a biblioteca Graph cliente da Microsoft não.  Consequentemente, você precisará converter as consultas relevantes em uma expressão mais RESTful.  

    Para fazer isso, altere:

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    Para:

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. Se seu código for páginas por coleções, faça os seguintes ajustes secundários. O exemplo a seguir compara e contrasta a busca de um grupo e a paagem através de seus membros, 5 de cada vez. Embora o código do Azure AD Graph requer uma construção de buscador para buscar os membros de um grupo, o Microsoft Graph não tem esse requisito. Fora isso, o código é relativamente semelhante.  Para ser conciso, apenas os membros do usuário são exibidos, as condições de tentativa/captura e erro não são mostradas e os trechos de código são para um aplicativo de console de thread único.

    Como exemplo, altere o código a seguir usando a biblioteca de clientes do Azure AD Graph .NET:

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

    Para o código a seguir usando a biblioteca de clientes do Microsoft Graph .NET:

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

7. Crie e corrige qualquer recurso, propriedade, navegação e erros de ação de serviço, geralmente relacionados a alterações de nome.

## <a name="see-also"></a>Confira também

O [C# trechos](https://github.com/microsoftgraph/console-csharp-snippets-sample) de console realça mais das diferenças entre a biblioteca de clientes do Microsoft Graph e a biblioteca de clientes do Azure AD Graph cliente.

A biblioteca de clientes do Azure AD Graph suporta apenas a plataforma .NET.  No entanto, Graph biblioteca de clientes da Microsoft oferece suporte a [plataformas](/graph) e idiomas adicionais que podem ser mais úteis para suas soluções.

## <a name="next-steps"></a>Próximas etapas

- Saiba como [implantar, testar e estender](./migrate-azure-ad-graph-deploy-test-extend.md) aplicativos que você migrou para o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.
