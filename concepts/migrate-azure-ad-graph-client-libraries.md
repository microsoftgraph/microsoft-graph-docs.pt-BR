---
title: Migrar aplicativos do Azure AD Graph .NET para o Microsoft Graph
description: Descreve como migrar aplicativos de API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 7fea43e808d14f2d80dc01690055257908f7fe18
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288353"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>Migrar o .NET Client library use para o Microsoft Graph

Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Se seu aplicativo usa atualmente a biblioteca de cliente do Azure AD Graph, alterne para a [biblioteca de cliente .net do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet).

>Observação: a biblioteca de cliente .NET do Microsoft Graph só tem suporte para o .NET Framework 4,5 e o .NET Standard 1,1.  No entanto, consulte a biblioteca de cliente .NET do Microsoft Graph para obter as informações mais recentes sobre suporte.

Veja aqui algumas etapas gerais para migrar para a biblioteca de cliente .NET do Microsoft Graph:

- Como criar um cliente do Microsoft Graph, dado um token de acesso (que você pode adquirir usando ADAL ou MSAL)
- Como formular solicitações
- Como usar construtores de consulta
- Como lidar com coleções e paginação  

## <a name="overview-of-the-migration-steps"></a>Visão geral das etapas de migração

As etapas a seguir supõem que o seu aplicativo já esteja usando a ADAL para adquirir tokens de acesso para chamar o Azure AD Graph e que, por enquanto, você continuará a usar a ADAL. Mudar para o MSAL pode ser feito como uma etapa separada descrita na [migração para o MSAL](./migrate-azure-ad-graph-authentication-library.md#migrating-to-msal).

1. Para adquirir um token de acesso ao Microsoft Graph, atualize o **resourceurl pela** de `https://graph.windows.net` para `https://graph.microsoft.com` .

2. Em seu aplicativo, atualize as referências à biblioteca de cliente do Microsoft Graph alterando:

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    Para:

    ``` csharp
    using Microsoft.Graph;
    ```

3. Use o Gerenciador de pacotes para baixar e atualizar o [pacote NuGet do Microsoft Graph](https://www.nuget.org/packages/Microsoft.Graph/) e atualizar as dependências.

4. Atualize o construtor de cliente para criar um `GraphServiceClient` , em vez de `ActiveDirectoryClient` .  Os trechos de código a seguir pressupõem que seu aplicativo está usando o `AcquireTokenAsyncForUser()` método para adquirir novos tokens. Você pode encontrar uma definição para este método como parte do [exemplo Active-Directory-dotnet-graphapi-console](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).

    Trocar

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

    Para a biblioteca de cliente do Microsoft Graph, o `serviceRoot` valor também inclui o número da versão. No momento, esse valor é `https://graph.microsoft.com/v1.0` .

5. Atualizar solicitações para usar a sintaxe do construtor de solicitação do cliente Microsoft Graph, alterando:

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    Para:

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    >[!NOTE]
    >A biblioteca de cliente do Azure AD Graph oferece suporte à sintaxe de consulta baseada em LINQ. No entanto, a biblioteca de cliente do Microsoft Graph não.  Consequentemente, você precisará converter as consultas relevantes para uma expressão mais RESTful.  

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

6. Se suas páginas de código por meio de coleções, faça os seguintes ajustes secundários. O exemplo a seguir compara e contrasta a busca de um grupo e uma paginação por meio de seus membros, 5 por vez. Embora o código do Microsoft Azure AD Graph exija uma construção de busca para buscar membros de um grupo, o Microsoft Graph não tem essa exigência. Além de isso, o código é relativamente semelhante.  Para ser conciso, somente os membros do usuário são exibidos, as condições de try/catch e de erro não são mostradas, e os trechos de código são para um aplicativo de console de thread único.

    Por exemplo, altere o código a seguir usando a biblioteca de cliente .NET do Azure AD Graph:

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

    Para o código a seguir usando a biblioteca de cliente .NET do Microsoft Graph:

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

7. Criar e corrigir qualquer recurso, propriedade, navegação e erros de ação de serviço, geralmente relacionados a alterações de nome.

## <a name="see-also"></a>Confira também

O [aplicativo trechos de console C#](https://github.com/microsoftgraph/console-csharp-snippets-sample) realça mais das diferenças entre a biblioteca de cliente do Microsoft Graph e a biblioteca de cliente do Azure ad Graph.

A biblioteca de cliente do Azure AD Graph oferece suporte somente à plataforma .NET.  No entanto, a biblioteca de cliente do Microsoft Graph oferece suporte a [plataformas e idiomas](/graph) adicionais que podem ser úteis para suas soluções.

## <a name="next-steps"></a>Próximas etapas

- Saiba como [implantar, testar e estender](./migrate-azure-ad-graph-deploy-test-extend.md) aplicativos que você migrou para o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.
