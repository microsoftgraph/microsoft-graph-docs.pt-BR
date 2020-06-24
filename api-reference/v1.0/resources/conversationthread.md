---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8608ea72c8c136b54f94c73f99ca0f79fbc7ec0b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845264"
---
# <a name="conversationthread-resource-type"></a>tipo de recurso conversationThread

Namespace: microsoft.graph

Um conversationThread é uma coleção de [postagens](post.md).

The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients.
A new thread is created when a recipient is removed from the thread.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar threads](../api/group-list-threads.md) | Coleção [conversationThread](conversationthread.md) |Obter todos os threads de um grupo.|
|[Criar thread](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.|
|[Obter conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Obtenha um thread específico pertencente a um grupo. |
|[Update](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Atualize o objeto conversationThread. |
|[Delete](../api/conversationthread-delete.md) | Nenhum |Exclua um objeto conversationThread. |
|[Responder](../api/conversationthread-reply.md)|Nenhuma|Responda a este thread criando uma nova entidade Post.|
|[Listar Postagens](../api/conversationthread-list-posts.md) |Coleção [post](post.md)| Obtenha as postagens do thread especificado. |

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo                                 | Descrição                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | Somente leitura.                                                                                                                                                                                       |
| toRecipients          | Coleção [recipient](recipient.md) | Os destinatários Para: do thread.                                                                                                                                                               |
| ccRecipients          | Coleção [recipient](recipient.md) | Os destinatários Cc: do thread.                                                                                                                                                               |
| topic                 | String                               | The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.                                                                              |
| hasAttachments        | Booliano                              | Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.                                                                                                               |
| lastDeliveredDateTime | DateTimeOffset                       | The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` |
| uniqueSenders         | Coleção de cadeias de caracteres                    | Todos os usuários que enviaram uma mensagem para este thread.                                                                                                                                                |
| visualização               | String                               | Um breve resumo do corpo da última postagem nesta conversa.                                                                                                                           |
| isLocked              | Booliano                              | Indica se o thread está bloqueado.                                                                                                                                                               |

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|postagens|Coleção [post](post.md)| Read-only. Nullable.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
