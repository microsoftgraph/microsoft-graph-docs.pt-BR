---
title: Recursos avançados de consulta nos objetos do diretório Microsoft Azure Active Directory
description: Os objetos do diretório Microsoft Azure Active Directory suportam recursos avançados de consulta para acesso eficiente aos dados.
author: Licantrop0
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 8156670a19364be7a58722ce966067c2e9e4a8b3
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461552"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Recursos avançados de consulta nos objetos do diretório Microsoft Azure Active Directory

Como o Microsoft Azure Active Directory continua a oferecer mais capacidades e melhorias na estabilidade, disponibilidade e desempenho, o Microsoft Graph também continua a evoluir e a escalar para acessar os dados de forma eficiente. Uma maneira é através do suporte crescente do Microsoft Graph para capacidades avançadas de consulta em vários objetos Microsoft Azure Active Directory e suas propriedades. Por exemplo, a adição de **não** (`not`), **não é igual a** (`ne`) e **termina com** (`endswith`) operadores no parâmetro de consulta`$filter`.

O mecanismo de consulta do Microsoft Graph usa um repositório de índice para atender às solicitações de consulta. Para adicionar suporte as funcionalidades adicionais de consulta em algumas propriedades, essas propriedades agora são indexadas em um repositório separado. Essa indexação separada permite que o Microsoft Azure AD aumente o suporte e melhore o desempenho das solicitações de consulta. No entanto, essas funcionalidades de consulta avançada não estão disponíveis por padrão, mas o solicitante também deve definir o cabeçalho **ConsistencyLevel** para `eventual` *e*, com exceção de `$search`, use o parâmetro de consulta `$count`. O cabeçalho **ConsistencyLevel** e `$count` são referidos como *parâmetros de consulta avançados*.

Por exemplo, para recuperar apenas contas de usuários inativos, você pode executar qualquer uma destas consultas que utilizam o parâmetro de consulta `$filter`.

<!-- markdownlint-disable MD023 MD024 MD025 -->
+ Opção 1: Use o parâmetro de consulta `$filter` com o operador `eq`. Esta solicitação funcionará por padrão, ou seja, a solicitação não requer os parâmetros de consulta avançados.

    # <a name="http"></a>[HTTP](#tab/http)
    <!-- {
      "blockType": "request",
      "name": "get_users_enabled"
    } -->
    ```msgraph-interactive
    GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
    ```

    # <a name="c"></a>[C#](#tab/csharp)

    ```csharp
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=CS
    var user = await graphClient.Users.Request()
        .Filter("accountEnabled eq false")
        .GetAsync();
    ```

    # <a name="javascript"></a>[JavaScript](#tab/javascript)

    ```javascript
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Javascript
    let users = await client.api('/users')
      .filter('accountEnabled eq false')
      .get();
    ```

    # <a name="objective-c"></a>[Objective-C](#tab/objc)

    ```objectivec
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Objective-C
    NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$filter=accountEnabled eq false"]]];
    [urlRequest setHTTPMethod:@"GET"];

    MSURLSessionDataTask *usersDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

      NSError *jsonError = nil;
      MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
      MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

    }];

    [usersDataTask execute];
    ```

    # <a name="java"></a>[Java](#tab/java)

    ```java
    // See https://docs.microsoft.com/en-us/graph/sdks/create-client?tabs=Java
    UserCollectionPage users = graphClient.users()
        .buildRequest()
        .filter("accountEnabled eq false")
        .get();
    ```

    # <a name="go"></a>[Ir](#tab/go)

    ```go
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Go
    requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
        Filter: "accountEnabled eq false",
    }

    options := &msgraphsdk.UsersRequestBuilderGetOptions{
        Q: requestParameters,
    }

    result, err := client.Users().Get(options)
    ```

    # <a name="powershell"></a>[PowerShell](#tab/powershell)

    ```powershell
    Import-Module Microsoft.Graph.Users

    Get-MgUser -Filter "accountEnabled eq false"
    ```

    ---

+ Opção 2: Use o parâmetro de consulta `$filter` com o operador `ne`. Esta solicitação não é suportada por padrão porque o `ne` operador só é suportado em consultas avançadas. Portanto, você deve adicionar o **ConsistencyLevel** cabeçalho para `eventual`*e* usar a `$count=true` cadeia de caracteres.

    # <a name="http"></a>[HTTP](#tab/http)
    <!-- {
      "blockType": "request",
      "name": "get_users_not_enabled"
    } -->
    ```msgraph-interactive
    GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
    ConsistencyLevel: eventual
    ```

    # <a name="c"></a>[C#](#tab/csharp)

    ```csharp
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=CS
    var user = await graphClient.Users.Request()
        .Request(new Option[] { new QueryOption("$count", "true")})
        .Header("ConsistencyLevel", "eventual")
        .Filter("accountEnabled ne true")
        .GetAsync();
    ```

    # <a name="javascript"></a>[JavaScript](#tab/javascript)

    ```javascript
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Javascript
    let users = await client.api('/users')
      .header('ConsistencyLevel','eventual')
      .filter('accountEnabled ne true')
      .count(true)
      .get();
    ```

    # <a name="objective-c"></a>[Objective-C](#tab/objc)

    ```objectivec
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Objective-C
    NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$filter=accountEnabled ne true&$count=true"]]];
    [urlRequest setHTTPMethod:@"GET"];
    [urlRequest setValue:@"eventual" forHTTPHeaderField:@"ConsistencyLevel"];

    MSURLSessionDataTask *usersDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

      NSError *jsonError = nil;
      MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
      MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

    }];

    [usersDataTask execute];
    ```

    # <a name="java"></a>[Java](#tab/java)

    ```java
    // See https://docs.microsoft.com/en-us/graph/sdks/create-client?tabs=Java
    LinkedList<Option> requestOptions = new LinkedList<Option>();
    requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
    requestOptions.add(new QueryOption("$count", "true"))

    UserCollectionPage users = graphClient.users()
        .buildRequest(requestOptions)
        .filter("accountEnabled ne true")
        .get();
    ```

    # <a name="go"></a>[Ir](#tab/go)

    ```go
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Go
    requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
        Filter: "accountEnabled ne true",
        Count: true,
    }

    headers := map[string]string{
        "ConsistencyLevel": "eventual"
    }

    options := &msgraphsdk.UsersRequestBuilderGetOptions{
        Q: requestParameters,
        H: headers,
    }

    result, err := client.Users().Get(options)
    ```

    # <a name="powershell"></a>[PowerShell](#tab/powershell)

    ```powershell
    Import-Module Microsoft.Graph.Users

    Get-MgUser -Filter "accountEnabled ne true" -CountVariable CountVar -ConsistencyLevel eventual
    ```

    ---

<!-- markdownlint-enable MD023 MD024 MD025 -->

Estas funcionalidades avançados de consulta são compatíveis somente com objetos de diretório do Microsoft Azure AD e suas relações, incluindo os seguintes objetos usados com frequência:

| Objeto                                                         | Relações                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Unidade administrativa](/graph/api/resources/administrativeunit) | <li>[membros](/graph/api/administrativeunit-list-members)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [Aplicativo](/graph/api/resources/application)                | <li>[proprietários](/graph/api/application-list-owners)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [Dispositivo](/graph/api/resources/device)                          | <li>[memberOf](/graph/api/device-list-memberof) <li>[transitiveMemberOf](/graph/api/device-list-transitivememberof) <li>[registeredUsers](/graph/api/device-list-registeredusers) <li>[registeredOwners](/graph/api/device-list-registeredowners)                                                                                                                                                                                                                                                                                                                                                                   |
| [Grupo](/graph/api/resources/group)                            | <li>[membros](/graph/api/group-list-members) <li>[transitiveMembers](/graph/api/group-list-transitivemembers) <li>[memberOf](/graph/api/group-list-memberof) <li>[transitiveMemberOf](/graph/api/group-list-transitivememberof) <li>[proprietários](/graph/api/group-list-owners) <li>[appRoleAssignments](/graph/api/group-list-approleassignments)                                                                                                                                                                                                                                                                       |
| [Contatos organizacionais](/graph/api/resources/orgContact)                     | <li>[memberOf](/graph/api/orgcontact-list-memberof) <li>[transitiveMemberOf](/graph/api/orgcontact-list-transitiveMemberOf)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [Entidade de serviço](/graph/api/resources/serviceprincipal)     | <li>[memberOf](/graph/api/serviceprincipal-list-memberof) <li>[transitiveMemberOf](/graph/api/serviceprincipal-list-transitivememberof) <li>[appRoleAssignments](/graph/api/serviceprincipal-list-approleassignments) <li>[appRoleAssignmentsTo](/graph/api/serviceprincipal-list-approleassignedto) <li>[oAuth2PermissionGrant](/graph/api/serviceprincipal-list-oauth2permissiongrants)                                                                                                                                                                                                                           |
| [Usuário](/graph/api/resources/user)                              | <li>[memberOf](/graph/api/user-list-memberof) <li>[transitiveMemberOf](/graph/api/user-list-transitivememberof)<li>[ownedObjects](/graph/api/user-list-ownedobjects) <li>[registeredDevices](/graph/api/user-list-registereddevices) <li>[ownedDevices](/graph/api/user-list-owneddevices) <li>[transitiveManagers](/graph/api/user-list-manager) <li>[directReports](/graph/api/user-list-directreports) <li>[transitiveReports](/graph/api/user-get-transitivereports) <li>[appRoleAssignments](/graph/api/user-list-approleassignments) <li>[oAuth2PermissionGrant](/graph/api/user-list-oauth2permissiongrants) |

A tabela a seguir lista os cenários de consulta em objetos de diretório com suporte apenas em consultas avançadas:

| Descrição                                                              | Exemplo                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :----------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Usar `$count` como um segmento URL                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                       |
| Usar o `$count` como parâmetro consultar cadeia de caracteres                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                     |
| Uso de `$count` em uma expressão `$filter`                                 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedLicenses%2F%24count%2Bne%2B0%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedLicenses/$count eq 0&$count=true`                                                                                                                                                                                       |
| Usar de `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                     |
| Usar `$orderby` em propriedades selecionadas                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                               |
| Usar o `$filter` com o `endsWith` operador                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                       |
| Usar o `$filter` e `$orderby` na mesma consulta                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                       |
| Uso o `$filter` com os `startsWith` operadores em propriedades específicas. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true` |
| Usar o `$filter` com `ne` e `not` operadores                           | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                           |
| Usar o `$filter` com `not` e `startsWith` operadores                   | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                      |
| Usar o molde de OData com outro parâmetro de consulta                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                             |

> [!NOTE]
>
> + O uso de `$filter` e `$orderBy` juntos é suportado apenas em consultas avançadas.
> + `$expand` atualmente não é suportado em consultas avançadas.
> + As funcionalidades de consulta avançada não estão disponíveis no momento para locatários do Azure AD B2C.
> + Para usar recursos avançados de consulta em [solicitações em lote](json-batching.md), especifique o cabeçalho **ConsistencyLevel** na propriedade **cabeçalhos** da solicitação JSON.

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>Suporte para filtro nas propriedades dos objetos do diretório Microsoft Azure Active Directory

As propriedades dos objetos de diretório se comportam de forma diferente em seu suporte aos parâmetros de consulta. Os cenários a seguir são comuns para objetos de diretório:

+ As consultas que são suportadas por padrão também funcionarão em consultas avançadas, mas a resposta será eventualmente consistente.
+ O operador `in` é suportado por padrão sempre que o operador `eq` for suportado por padrão.
+ O operador `endsWith` é suportado apenas em consultas avançadas nas propriedades **email**, e **userPrincipalName**, e propriedades **proxyAddresses**.
+ Os operadores de negação `not` e `ne` são suportados apenas em consultas avançadas.
  + Todas as propriedades que suportam o `eq` operador também suportam os `ne` ou `not` operadores.
  + Para consultas que utilizam o `any` operador lambda, usar o `not` operador. Veja [Filtrar utilizando operadores lambda](/graph/query-parameters#filter-using-lambda-operators).

As tabelas a seguir resumem o suporte para `$filter` operadores por propriedades de objetos de diretório suportados pelas funcionalidades de consulta avançada.

### <a name="legend"></a>Legenda

+ ![Funciona por padrão. Não requer parâmetros de consulta avançados.](../concepts/images/yesandnosymbols/greencheck.svg) O operador `$filter` funciona por padrão para essa propriedade.
+ ![Requer parâmetros de consulta avançados.](../concepts/images/yesandnosymbols/whitecheck-in-greencircle.svg) O `$filter` operador **exige** *parâmetros de consulta avançados*, que são:
  + `ConsistencyLevel=eventual` cabeçalho
  + `$count=true` cadeia de caracteres
+ ![Não suportado.](../concepts/images/yesandnosymbols/no.svg) O operador `$filter` não é suportado nessa propriedade. [Envie-nos comentários](https://aka.ms/MsGraphAADSurveyDocs) para solicitar que esta propriedade suporte `$filter` para seus cenários.
+ As células em branco indicam que a consulta não é válida para aquela propriedade.
+ A coluna de **valor nulo** indica que a propriedade pode ser anulada e filtrada usando `null`.
+ As propriedades que não estão listadas aqui não suportam `$filter` de forma alguma.

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]

## <a name="error-handling-for-advanced-queries-on-directory-objects"></a>Tratamento de erros para consultas avançadas sobre objetos de diretório

A contagem de objetos de diretório só é suportada usando os parâmetros de consultas avançadas. Se o `ConsistencyLevel=eventual` cabeçalho não for especificado, a solicitação retornará um erro quando o `$count` segmento de URL for usado ou ignorará silenciosamente o `$count` parâmetro de consulta (`?$count=true`) se for usado.

<!-- {
  "blockType": "request",
  "name": "get_users_count_bad"
} -->
```http
https://graph.microsoft.com/v1.0/users/$count
```

<!-- {
  "blockType": "response",
  "@odata.type": "odata.error",
  "expectError": true
} -->
```json
{
    "error": {
        "code": "Request_BadRequest",
        "message": "$count is not currently supported.",
        "innerError": {
            "date": "2021-05-18T19:03:10",
            "request-id": "d9bbd4d8-bb2d-44e6-99a1-71a9516da744",
            "client-request-id": "539da3bd-942f-25db-636b-27f6f6e8eae4"
        }
    }
}
```

Para objetos de diretório, `$search` funciona apenas em consultas avançadas. Se o cabeçalho **ConsistencyLevel** não for especificado, o pedido retorna um erro.

<!-- {
  "blockType": "request",
  "name": "get_applications_search_displayName"
} -->
```http
https://graph.microsoft.com/v1.0/applications?$search="displayName:Browser"
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Request with $search query parameter only works through MSGraph with a special request header: 'ConsistencyLevel: eventual'",
        "innerError": {
            "date": "2021-05-27T14:26:47",
            "request-id": "9b600954-ba11-4899-8ce9-6abad341f299",
            "client-request-id": "7964ef27-13a3-6ca4-ed7b-73c271110867"
        }
    }
}
```

Se uma propriedade ou parâmetro de consulta na URL for suportado apenas em consultas avançadas, mas o cabeçalho **ConsistencyLevel** ou a cadeia de caracteres `$count=true` estiver faltando, a solicitação retorna um erro.

<!-- {
  "blockType": "request",
  "name": "get_users_filer_endsWith"
} -->
```http
https://graph.microsoft.com/v1.0/users?$filter=endsWith(mail,'@outlook.com')
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Unsupported Query.",
        "innerError": {
            "date": "2021-05-18T19:12:36",
            "request-id": "63f2093c-399c-4350-9609-3ce9b62abe3c",
            "client-request-id": "e60ed0ba-df5d-e190-f056-f9c0318456d7"
        }
    }
}
```

Se uma propriedade não tiver sido indexada para suportar um parâmetro de consulta, mesmo que os parâmetros de consulta avançados sejam especificados, a solicitação retorna um erro.

<!-- {
  "blockType": "request",
  "name": "get_groups_unindexed_bad"
} -->
```http
https://graph.microsoft.com/beta/groups?$filter=createdDateTime ge 2021-11-01&$count=true
ConsistencyLevel: eventual
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "The request uses a filter property that is not indexed",
        "innerError": {
            "date": "2021-06-10T19:32:01",
            "request-id": "5625ba13-0c9f-4fce-a853-4b52f3e0bd09",
            "client-request-id": "76fe4cd8-df3a-f8c3-659b-594274b6bb31"
        }
    }
}
```

No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.
Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.
Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado. Por exemplo, no exemplo a seguir, falta o parâmetro `@odata.count` mesmo que a consulta seja bem sucedida.

```http
https://graph.microsoft.com/v1.0/users?$count=true
```

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "displayName":"Oscar Ward",
      "mail":"oscarward@contoso.com",
      "userPrincipalName":"oscarward@contoso.com"
    },
  ]
}
```

## <a name="see-also"></a>Confira também

+ [Usar parâmetros de consulta para personalizar respostas](/graph/query-parameters)
+ [Limitações do parâmetro de consulta](known-issues.md#some-limitations-apply-to-query-parameters)
+ [Usar o parâmetro de consulta $search para corresponder a um critério de pesquisa](/graph/search-query-parameter#using-search-on-directory-object-collections)
+ [Explorar os recursos de consulta avançados para objetos de diretório do Azure Active Directory com o .NET SDK](https://github.com/microsoftgraph/dotnet-aad-query-sample/)
