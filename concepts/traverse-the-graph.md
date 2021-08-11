---
title: Acessar dados e métodos ao navegar no Microsoft Graph
description: Além de usar a API do Microsoft Graph para ler e gravar dados, você pode usar diversos padrões de solicitação para desviar pelos recursos no Microsoft Graph. O documento de metadados também ajuda a entender o modelo de dados dos recursos e das relações no Microsoft Graph.
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e1e7c7fd35f6564e2021ebf0b222d81c6246447e546fa11c69c4f3b4a6cbe671
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54132939"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a>Acessar dados e métodos ao navegar no Microsoft Graph

Além de usar a API do Microsoft Graph para ler e gravar dados, você pode usar diversos padrões de solicitação para desviar pelos recursos no Microsoft Graph. O documento de metadados também ajuda a entender o modelo de dados dos recursos e das relações no Microsoft Graph.

## <a name="microsoft-graph-api-metadata"></a>Metadados da API do Microsoft Graph

O documento de metadados ($metadata) é publicado na raiz do serviço. Você pode exibir o documento de serviço das versões 1.0 e beta da API Microsoft Graph com as URLs a seguir.

**Metadados 1.0 da API do Microsoft Graph**

```msgraph-interactive
https://graph.microsoft.com/v1.0/$metadata
```

**Metadados beta da API do Microsoft Graph**

```msgraph-interactive
https://graph.microsoft.com/beta/$metadata
```

Com os metadados, você pode exibir e entender o modelo de dados do Microsoft Graph, inclusive os tipos de entidade, os tipos complexos e as enumerações que compõem os recursos representados nos pacotes de solicitação e resposta. 

Os metadados também são compatíveis com os tipos, métodos e enumerações que os define em espaços de nomes (ou namespace),OData correspondentes. A maior parte da API do Microsoft Graph é definida no espaço de nomes OData, `microsoft.graph`.

Você pode usar os metadados para compreender as relações entre entidades no Microsoft Graph e estabelecer URLs que navegam entre essas entidades.

> [!NOTE]
> - Use as IDs de recurso no mesmo caso de serem retornadas das APIs do Microsoft Graph.
> - Presuma que as IDs de recurso, valores atribuídos e outros valores codificados em base 64 _diferenciam maiúsculas de minúsculas_.
> - Presuma que os nomes de recursos do caminho da URL, parâmetros de consulta, nomes de ações e funções, solicitação de parâmetros de corpo, inclusive os nomes e valores da propriedade da API _não diferenciam maiúsculas e minúsculas_.

## <a name="view-a-collection-of-resources"></a>Exibir um conjunto de recursos

O Microsoft Graph permite exibir recursos em um locatário usando consultas HTTP `GET`. A resposta da consulta inclui as propriedades de cada recurso. Os recursos de entidade são identificados pelas respectivas IDs. O formato da ID do recurso pode ser um GUID e normalmente varia de acordo com o tipo de recurso.

Por exemplo, você pode obter uma coleção de recursos de [user](/graph/api/resources/user) definida no locatário:

```
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

Se tiver êxito, você receberá uma resposta 200 OK que contém a coleção de recursos **user** no payload. Cada usuário será identificado pela propriedade **id** e acompanhado pelas respectivas propriedades padrão. O payload exibido abaixo foi truncado por uma questão de resumo.

```
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

O Microsoft Graph também permite exibir coleções navegando entre as relações de um recurso com o outro. Por exemplo, por meio de uma propriedade de navegação **mailFolders**,você pode consultar uma coleção de recursos [mailFolder](/graph/api/resources/mailfolder), na caixa de correio do usuário:

```
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

Se tiver êxito, você receberá uma resposta 200 OK que contém a coleção de recursos [mailFolder](/graph/api/resources/user) no payload. Cada recurso **mailFolder** será identificado pela propriedade **id** e acompanhado pelas respectivas propriedades. O payload exibido abaixo foi truncado por uma questão de resumo.

```
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a>Exibir um recurso específico de uma coleção pela ID

Para exibir as informações sobre um usuário, ainda com o uso do recurso **user** como exemplo, use uma solicitação GET HTTPS para chegar a um usuário específico pela ID do usuário. No caso de uma entidade **user**, você pode usar a propriedade **id** ou **userPrincipalName** como identificador.

A solicitação de exemplo a seguir usa o valor **userPrincipalName** como ID do usuário.

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

Se tiver êxito, você obterá uma resposta 200 OK que contém a representação do recurso do usuário na carga, conforme mostrado.

```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ...
}
```

## <a name="read-specific-properties-of-a-resource"></a>Ler propriedades específicas de um recurso
Para recuperar apenas os dados biográficos do usuário, conforme fornecido por ele na descrição _Sobre mim_, e suas habilidades, você pode adicionar o parâmetro de consulta [$select](query-parameters.md) à solicitação anterior, como mostrado no exemplo a seguir.

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.

```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
Aqui, em vez de todos os conjuntos de propriedade na entidade **user**, somente as propriedades básicas **aboutMe**, **displayName** e **skills** são retornadas.

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>Ler propriedades específicas dos recursos em uma coleção
Além de ler propriedades específicas de um único recurso, você também pode aplicar o parâmetro de consulta [$select](query-parameters.md) semelhante a uma coleção para obter todos os recursos na coleção com apenas as propriedades específicas retornadas em cada um.

Por exemplo, para consultar o nome dos itens na unidade do usuário conectado, você pode enviar a seguinte solicitação HTTPS GET.

```
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

A resposta bem-sucedida retorna um código de status 200 OK e uma carga que contém apenas os nomes dos arquivos compartilhados, conforme mostrado no exemplo abaixo.

```
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>Passar de um recurso para outro pela relação
Um gerente tem uma relação **directReports** com outros usuários diretamente subordinados a ele. Para consultar a lista de subordinados de um usuário, você pode usar a solicitação HTTPS GET a seguir para navegar para o destino pretendido via passagem de relação.

```
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.

```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

Da mesma forma, você pode seguir um relacionamento para navegar até os recursos relacionados. Por exemplo, a relação mensagens-usuário habilita a passagem de um usuário do Azure Active Directory (Microsoft Azure AD) para um conjunto de mensagens de email do Outlook. O exemplo a seguir mostra como fazer isso em uma chamada à API REST.


```
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.


```
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",

       ...
    }
  ]
}
```
Você pode ver todas as relações em um determinado recurso indo para os metadados, localizando `EntityType` e examinando todas as`NavigationProperty` do `EntityType`.

## <a name="call-actions-and-functions"></a>Funções e ações de chamada
O Microsoft Graph também oferece suporte a _ações_ e _funções_ para manipular recursos de maneiras que não são apenas operações de criação, leitura, atualização e exclusão (CRUD). Eles normalmente estão na forma de solicitações de HTTPS POST para receber argumentos para a ação ou função. Por exemplo, a seguinte ação permite que o usuário conectado (`me`) envie uma mensagem de email.

```
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@contoso.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

Você pode ver todas as funções que estão disponíveis nos metadados. Eles aparecem como Funções ou Ações.

## <a name="use-the-microsoft-graph-sdks"></a>Usar os SDKs do Microsoft Graph

Como o poder e a facilidade dos SDKs? Enquanto você sempre pode usar APIs REST para chamar o Microsoft Graph, também fornecemos SDKs para muitas plataformas populares. Para explorar os SDKs disponíveis, veja [Amostras de código e SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).

## <a name="see-also"></a>Confira também

- [Usar a API do Microsoft Graph](use-the-api.md)
- [Obter tokens de autenticação](./auth/index.yml)