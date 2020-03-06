---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4e49e8617125758f606c42c47de3d9d13495666f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531752"
---
# <a name="conversationthread-resource-type"></a>tipo de recurso conversationThread

Namespace: Microsoft. Graph A conversationThread é uma coleção de [postagens](post.md).

A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar threads](../api/group-list-threads.md) | Coleção [conversationThread](conversationthread.md) |Obter todos os threads de um grupo.|
|[Criar thread](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.|
|[Obter conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Obtenha um thread específico pertencente a um grupo. |
|[Update](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Atualize o objeto conversationThread. |
|[Excluir](../api/conversationthread-delete.md) | Nenhum |Exclua um objeto conversationThread. |
|[Responder](../api/conversationthread-reply.md)|Nenhuma|Responda a este thread criando uma nova entidade Post.|
|[Listar Postagens](../api/conversationthread-list-posts.md) |Coleção [post](post.md)| Obtenha as postagens do thread especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: do thread.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: do thread.|
|topic|String|O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.||
|hasAttachments|Booliano|Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.|
|lastDeliveredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|uniqueSenders|Coleção de cadeias de caracteres|Todos os usuários que enviaram uma mensagem para este thread.|
|visualização|String|Um breve resumo do corpo da última postagem nesta conversa.|
|isLocked|Booliano|Indica se o thread está bloqueado.|

## <a name="relationships"></a>Relacionamento
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
