---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b559ce1ee1d6f0a79734e65b3a491a047fbb9cd8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029091"
---
# <a name="conversationthread-resource-type"></a>tipo de recurso conversationThread

Namespace: microsoft.graph

Um conversationThread é uma coleção de [postagens](post.md).

A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar threads](../api/group-list-threads.md) | Coleção [conversationThread](conversationthread.md) |Obter todos os threads de um grupo.|
|[Criar thread](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.|
|[Obter conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Obtenha um thread específico pertencente a um grupo. |
|[Update](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Atualize o objeto conversationThread. |
|[Delete](../api/conversationthread-delete.md) | None |Exclua um objeto conversationThread. |
|[Responder](../api/conversationthread-reply.md)|Nenhuma|Responda a este thread criando uma nova entidade Post.|
|[Listar Postagens](../api/conversationthread-list-posts.md) |Coleção [post](post.md)| Obtenha as postagens do thread especificado. |

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo                                 | Descrição                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | Somente leitura. <br/><br/>Devolvido por padrão.                                                                                                                                                                                      |
| toRecipients          | Coleção [recipient](recipient.md) | Os destinatários Para: do thread. <br/><br/>Retornado apenas em `$select`.                                                                                                                                                              |
| ccRecipients          | Coleção [recipient](recipient.md) | Os destinatários Cc: do thread. <br/><br/>Retornado apenas em `$select`.                                                                                                                                                               |
| topic                 | String                               | O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada. <br/><br/>Devolvido por padrão.                                                                              |
| hasAttachments        | Booliano                              | Indica se qualquer uma das postagens neste thread tem pelo menos um anexo. <br/><br/>Devolvido por padrão.                                                                                                              |
| lastDeliveredDateTime | DateTimeOffset                       | O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.<br/><br/>Retornado por padrão. |
| uniqueSenders         | Coleção de cadeias de caracteres                    | Todos os usuários que enviaram uma mensagem para este thread. <br/><br/>Devolvido por padrão.                                                                                                                                               |
| visualização               | String                               | Um breve resumo do corpo da postagem mais recente nesta conversa. <br/><br/>Devolvido por padrão.                                                                                                                           |
| isLocked              | Booliano                              | Indica se o thread está bloqueado. <br/><br/>Devolvido por padrão.                                                                                                                                                              |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|postagens|Coleção [post](post.md)| Somente leitura. Anulável.|

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

