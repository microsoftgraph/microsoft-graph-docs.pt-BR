---
title: Obter workbookCommentReply
description: Recupere as propriedades e os relacionamentos do objeto workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 97ae39d4cfb68aafaea0613f524deb9a7f6be0af
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775724"
---
# <a name="get-workbookcommentreply"></a>Obter workbookCommentReply

Recupere as propriedades e os relacionamentos do objeto [workbookCommentReply](../resources/workbookcommentreply.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Files.ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments/{id}/replies/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workbookCommentReply](../resources/workbookcommentreply.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies/{id}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is text of comment.",
  "contentType": "Plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
