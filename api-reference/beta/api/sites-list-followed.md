---
author: learafa
description: Listar os sites que foram seguidos pelo usuário conectado.
title: Listar sites seguidos
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: a5a1fa349440a998bdd33a6bdddddf32fcbc162d
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934861"
---
# <a name="list-followed-sites"></a>Listar sites seguidos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar os [sites](../resources/site.md) que foram seguidos pelo usuário conectado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Este método é acessível apenas por meio do OneDrive for Business.

<!-- { "blockType": "ignored" } -->

```http
POST /me/followedSites
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | Portador {código}. Obrigatório.|

## <a name="request-body"></a>Corpo da Solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Este método retorna uma coleção de recursos do [site](../resources/site.md) que o usuário está seguindo.
Se nenhum site for encontrado, uma coleção vazia será retornada.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
POST /me/followedSites
```
### <a name="response"></a>Resposta
<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.site)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
            "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site",
            "webUrl": "https://contoso.sharepoint.com/teams/1drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "2C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/1drvteam",
                "webId": "2D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,1C712604-1370-44E7-A1F5-426573FDA80A,1D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site1",
            "webUrl": "https://contoso.sharepoint.com/teams/2drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "1C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/2drvteam",
                "webId": "1D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the sites a user is following.",
  "keywords": "site,onedrive.site,list followed sites, followedSites",
  "section": "documentation",
  "tocPath": "Sites/List followed sites",
  "suppressions": [
  ]
}
-->
