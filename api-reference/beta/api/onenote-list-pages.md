---
title: Listar páginas
description: Recupere uma lista de objetos de página.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 82e09e6274713c043fd3d7f1bf7c9d8bb07cbaa6
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942090"
---
# <a name="list-pages"></a>Listar páginas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos de](../resources/onenotepage.md) página.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) | Notes.Read, Notes.ReadWrite    |
|Aplicativo | Notes.Read.All, Notes.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

A consulta padrão para páginas retorna as 20 principais páginas ordenadas por `lastModifiedTime desc` . Se a consulta padrão retornar mais de 20 páginas, a resposta conterá um que você pode usar para página `@odata.nextLink` através do conjunto de resultados. O número máximo de páginas retornadas para `top` uma solicitação é 100.

A resposta padrão `parentSection` expande e seleciona as `id` propriedades e , da `displayName` `self` seção. Os `expand` valores válidos para páginas `parentNotebook` são e `parentSection` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Aceitar | string | `application/json` |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos onenotePage](../resources/onenotepage.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "title": "title-value",
      "createdByAppId": "createdByAppId-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      },
      "contentUrl": "contentUrl-value",
      "content": "content-value",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
