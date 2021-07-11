---
title: Recursos avançados de consulta nos objetos do diretório Microsoft Azure Active Directory
description: Os objetos do diretório Microsoft Azure Active Directory suportam recursos avançados de consulta para acesso eficiente aos dados.
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 03210e9c46776c4fbc92057870737a87c7e47371
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366511"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Recursos avançados de consulta nos objetos do diretório Microsoft Azure Active Directory

Como o Microsoft Azure Active Directory continua a oferecer mais capacidades e melhorias na estabilidade, disponibilidade e desempenho, o Microsoft Graph também continua a evoluir e a escalar para acessar os dados de forma eficiente. Uma maneira é através do suporte crescente do Microsoft Graph para capacidades avançadas de consulta em vários objetos Microsoft Azure Active Directory e suas propriedades. Por exemplo, a adição de **Não** (`NOT`), **Não é igual a** (`ne`), e **Termina com** (`endsWith`) operadores no parâmetro `$filter` de consulta em outubro de 2020.

O mecanismo de consulta do Microsoft Graph usa uma loja de índices para atender aos pedidos de consulta. Para adicionar suporte para capacidades adicionais de consulta em algumas propriedades, estas propriedades são agora indexadas em um servidor separado. Esta indexação separada permite que o MIcrosoft Azure Active Directory aumente o suporte e melhore o desempenho dos pedidos de consulta. Entretanto, estas capacidades avançadas de consulta não estão disponíveis por padrão, mas o solicitante também deve definir o **ConsistencyLevel** como `eventual` *e*, com exceção de `$search`, usar o parâmetro `$count` consulta (seja como [segmento URL](/graph/query-parameters#other-odata-url-capabilities) ou `$count=true` cadeia de caracteres). O cabeçalho **ConsistencyLevel** e `$count` são referidos como *parâmetros de consulta avançados*.

Por exemplo, se você deseja recuperar apenas contas de usuários inativos, você pode executar qualquer uma destas consultas que utilizam o Parâmetro de consulta `$filter`.

+ Usar o parâmetro `$filter` consulta com o operador `eq`. Esta solicitação funcionará por padrão, ou seja, a solicitação não requer os parâmetros de consulta avançados.

<!-- {
  "blockType": "ignored",
  "name": "get_users_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
```

+ Usar o parâmetro `$filter` consulta com o operador `ne`. Esta solicitação não é suportada por padrão porque o `ne` operador só é suportado em consultas avançadas. Portanto, você deve adicionar o **ConsistencyLevel** cabeçalho para `eventual`*e* usar a `$count=true` cadeia de caracteres.

<!-- {
  "blockType": "ignored",
  "name": "get_users_not_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
ConsistencyLevel: eventual
```

Estes recursos avançados de consulta são suportados apenas em objetos Microsoft Azure Active Directory, ou seja, os seguintes recursos e suas relações que derivam do [directoryObject](/graph/api/resources/directoryobject):

- [aplicativo](/graph/api/resources/application)
- [orgContact](/graph/api/resources/orgcontact)
- [device](/graph/api/resources/device)
- [group](/graph/api/resources/group)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [user](/graph/api/resources/user)

A tabela a seguir lista cenários de consulta em objetos de diretório que são suportados apenas em consultas avançadas.

| Descrição                                                              | Exemplo                                                                                                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usar `$count` como um segmento URL                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                       |
| Usar o `$count` como parâmetro consultar cadeia de caracteres                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                     |
| Usar de `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                     |
| Usar `$orderby` em propriedades selecionadas                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                               |
| Usar o `$filter` com o `endsWith` operador                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                       |
| Usar o `$filter` e `$orderby` na mesma consulta                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                       |
| Uso o `$filter` com os `startsWith` operadores em propriedades específicas. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true` |
| Usar o `$filter` com `ne` e `NOT` operadores                           | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                     |
| Usar o `$filter` com `NOT` e `startsWith` operadores                   | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                |
| Usar o molde de OData com outro parâmetro de consulta                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                             |

> [!NOTE]
> Estas capacidades avançadas de consulta não estão disponíveis nos locatários do Azure AD B2C.

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>Suporte para filtro nas propriedades dos objetos do diretório Microsoft Azure Active Directory

As propriedades dos objetos de diretório se comportam de forma diferente em seu suporte aos parâmetros de consulta. Os cenários a seguir são comuns para objetos de diretório:

+ Salvo indicação em contrário, as propriedades com o mesmo nome nos recursos de diretório suportam os mesmos operadores `$filter`. Por exemplo, a propriedade **createdDateTime** está disponível no **aplicação**, **grupo**, **organização**, e **usuário** recursos. Ele suporta os operadores `eq`, `ge`, e `le` por padrão e os operadores `in`, `ne`, e `NOT` apenas em consultas avançadas.
+ O `endsWith` operador é suportado apenas em **email** e **userPrincipalNameerPrincipalName** propriedades.
+ Consultas que são suportadas por padrão também funcionarão em consultas avançadas.
+ Os operadores `NOT` e `ne` de negação são suportados apenas em consultas avançadas. 
  + Todas as propriedades que suportam o `eq` operador também suportam os `ne` ou `NOT` operadores.
  + O `ne` operador nega onde de outra forma o `eq` operador avaliaria para `true`. Para consultas que utilizam o `any` operador lambda, usar o `NOT` operador. Veja [Filtrar utilizando operadores lambda](/graph/query-parameters#filter-using-lambda-operators).

A tabela a seguir resume o suporte a `$filter` operadores por propriedades no [objeto de diretório](/graph/api/resources/user) de usuários.

- ![Funciona por padrão. Não requer parâmetros de consulta avançados.](/graph/images/advanced-query-parameters/default.png) A propriedade suporta `$filter` com o operador por padrão.
- ![Requer parâmetros de consulta avançados.](/graph/images/advanced-query-parameters/advanced.png) O operador específico `$filter` requer *parâmetros de consulta avançados*:
  - `ConsistencyLevel=eventual` cabeçalho
  - `$count=true` cadeia de caracteres
- Células em branco indicam que a propriedade não suporta o uso de `$filter` com o operador.
- A coluna **valores nulos** indica que a propriedade é filtrável em `null` valores.
- As propriedades que não estão listadas aqui não suportam `$filter`.

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]


## <a name="error-handling-for-advanced-queries-on-directory-objects"></a>Tratamento de erros para consultas avançadas sobre objetos de diretório

A contagem de objetos de diretório só é suportada usando os parâmetros de consultas avançados. Se o cabeçalho `ConsistencyLevel=eventual` não for especificado, o pedido retorna um erro quando o segmento `$count` URL é usado ou ignora silenciosamente o parâmetro `$count` consulta (`?$count=true`) se for usado.

```http
https://graph.microsoft.com/v1.0/users/$count
```

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

`$search` nos recursos do Microsoft Azure Active Directory que derivam de [diretórioObject](/graph/api/resources/directoryobject) funciona apenas em consultas avançadas. Se o cabeçalho **ConsistencyLevel** não for especificado, o pedido retorna um erro.

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

```http
https://graph.microsoft.com/beta/users?$filter=endsWith(mail,'@outlook.com')
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

```http
https://graph.microsoft.com/v1.0/users?$filter=id ge '398164b1-5196-49dd-ada2-364b49f99b27'&$count=true
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

No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente. Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte. Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado. Por exemplo, no exemplo a seguir, falta o parâmetro `@odata.count` mesmo que a consulta seja bem sucedida.

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

- [Usar parâmetros de consulta para personalizar respostas](/graph/query-parameters)
- [Limitações do parâmetro de consulta](known-issues.md#query-parameter-limitations)
- [Usar o parâmetro de consulta $search para corresponder a um critério de pesquisa](/graph/search-query-parameter)
