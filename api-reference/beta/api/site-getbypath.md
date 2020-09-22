---
author: JeremyKelley
description: Recupere as propriedades e as relações de um recurso do site.
ms.date: 09/10/2017
title: Obter site do SharePoint por caminho
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f5b61c84146701782c1dbe5e8b24631ca30bbb79
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013969"
---
# <a name="get-a-site-resource-by-path"></a>Obter um recurso de site pelo caminho

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.

[site]: ../resources/site.md

Além de recuperar um [site pelo ID](site-get.md), você pode recuperar um site com base no caminho da URL relativa ao servidor.

* Hostname do conjunto de sites (contoso.sharepoint.com)
* Caminho do site, em relação ao nome de host do servidor.

Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:

* `/sites/root`: O site raiz do locatário.
* `/groups/{group-id}/sites/root`: O site da equipe do grupo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para acessar o site raiz do SharePoint com um caminho relativo:

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a>Resposta

Este método retorna um recurso de [site][] para o site referenciado pelo identificador exclusivo.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": { 
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path",
  "suppressions": []
}
-->


