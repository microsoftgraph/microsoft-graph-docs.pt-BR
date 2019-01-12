---
title: Excluir uma atividade
description: Exclua uma atividade do usuário existente para seu aplicativo.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: cbe12a373f06c2893a5ca202247865f4ce4a8f52
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966850"
---
# <a name="delete-an-activity"></a>Excluir uma atividade

Exclua uma atividade do usuário existente para seu aplicativo.

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
DELETE /me/activities/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|Autorização | string | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Nenhum corpo da solicitação.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará o `204 No Content` código de resposta se a atividade foi excluída.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
