---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 285178adb4f0df591e1d1270d60b572f346d57e1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472892"
---
# <a name="create-outlooktaskfolder-deprecated"></a>Criar outlookTaskFolder (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Criar uma pasta de tarefas do Outlook em um [outlookTaskGroup especificado.](../resources/outlooktaskgroup.md)
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Tasks.ReadWrite    |
|Delegada (conta pessoal da Microsoft) | Tasks.ReadWrite    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir cria uma pasta de tarefas `Cooking` chamada no grupo de tarefas especificado.

<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```

No corpo da solicitação, fornece uma representação JSON do [objeto outlookTaskFolder.](../resources/outlooktaskfolder.md)
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


