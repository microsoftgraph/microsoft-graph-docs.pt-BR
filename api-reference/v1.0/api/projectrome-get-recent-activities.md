---
title: Obter atividades recentes do usuário
description: " API. O serviço consultará os historyItems mais recentes e, em seguida, puxará essas atividades relacionadas. As atividades serão ordenadas de acordo com o **últimoModified mais** recente no **historyItem**. Isso significa que as atividades **sem historyItems** não serão incluídas na resposta. A permissão UserActivity.ReadWrite.CreatedByApp também aplicará filtragem extra à resposta, para que somente as atividades criadas por seu aplicativo sejam retornadas. Essa filtragem do lado do servidor poderá resultar em páginas vazias se o usuário estiver particularmente ativo e outros aplicativos criarem atividades mais recentes. Para obter as atividades do aplicativo, use a **propriedade nextLink** para paginar."
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 8a6b72fbe2041faf909dc3a2429d8891c5859261
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292326"
---
# <a name="get-recent-user-activities"></a>Obter atividades recentes do usuário

Namespace: microsoft.graph

Obter atividades recentes para um determinado usuário. Essa função OData tem alguns comportamentos padrão incluídos para fazê-la funcionar como uma API "usada mais recentemente". O serviço consultará os [historyItems](../resources/projectrome-historyitem.md)mais recentes e, em seguida, puxará essas atividades relacionadas. As atividades serão ordenadas de acordo com o **últimoModified mais** recente no **historyItem**. Isso significa que as atividades **sem historyItems** não serão incluídas na resposta. A permissão UserActivity.ReadWrite.CreatedByApp também aplicará filtragem extra à resposta, para que somente as atividades criadas por seu aplicativo sejam retornadas. Essa filtragem do lado do servidor poderá resultar em páginas vazias se o usuário estiver particularmente ativo e outros aplicativos criarem atividades mais recentes. Para obter as atividades do aplicativo, use a **propriedade nextLink** para paginar.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | UserActivity.ReadWrite.CreatedByApp    |
|Delegado (conta pessoal da Microsoft) | UserActivity.ReadWrite.CreatedByApp    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte a alguns [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta. Há suporte para os seguintes parâmetros de consulta:

- $expand para a **propriedade de navegação historyItems.**
- $top limitar o número máximo de itens entre páginas.
- $filter na propriedade **lastModifiedDateTime** para **atividades** ou **historyItems**, se expandido.

A seguir estão alguns exemplos de consultas com suporte com codificação de URL.

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|Autorização | string | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não especifique um corpo de solicitação.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` o código de resposta com as atividades recentes do usuário para seu aplicativo.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/activities/recent
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recent-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recent-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recent-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recent-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->
