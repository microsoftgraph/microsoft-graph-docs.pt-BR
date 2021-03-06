---
title: Obter página
description: Recupere as propriedades e os relacionamentos de um objeto Page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 98c15b4638ce41debc9e8dd040d77d610ad1665b
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401999"
---
# <a name="get-page"></a>Obter página

Namespace: microsoft.graph

Recupere as propriedades e os relacionamentos de um objeto [Page](../resources/page.md) .

**Obtendo informações da página**

Acessar os metadados de uma página por identificador de página:

```
GET /me/onenote/pages/{id}
```

**Obtendo o conteúdo da página**

Você pode usar o ponto de `content` extremidade da página para obter o conteúdo HTML de uma página:

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

A `includeIDs=true` opção de consulta é usada para [Atualizar páginas](../api/page-update.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Notes. Read, Notes. ReadWrite, Notes. Read. All, Notes. ReadWrite. All    |
|Delegado (conta pessoal da Microsoft) | Notes. Read, Notes. ReadWrite    |
|Aplicativo | Notes.Read.All, Notes.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte `select` aos `expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

A resposta padrão expande `parentSection` e seleciona as `id` `name` Propriedades, e e `self` . `expand`Os valores válidos para páginas são `parentNotebook` e `parentSection` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Aceitar | string | `application/json` |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [Page](../resources/page.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto Response mostrado aqui é truncado por brevidade. Todas as propriedades serão retornadas de uma chamada real.
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->