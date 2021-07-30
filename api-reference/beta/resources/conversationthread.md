---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d73c84fec11ae4ee3bbf1d07b237b82fbfc6ddf7
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660307"
---
# <a name="conversationthread-resource-type"></a>tipo de recurso conversationThread

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um conversationThread é uma coleção de [postagens](post.md).

A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar threads](../api/group-list-threads.md) | Coleção [conversationThread](conversationthread.md) |Obter todos os threads de um grupo.|
|[Criar thread](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.|
|[Obter conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Obtenha um thread específico pertencente a um grupo. |
|[Update](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Atualize o objeto conversationThread. |
|[Delete](../api/conversationthread-delete.md) | Nenhum |Exclua um objeto conversationThread. |
|[reply](../api/conversationthread-reply.md)|Nenhum|Responda a este thread criando uma nova entidade Post.|
|[Listar Postagens](../api/conversationthread-list-posts.md) |Coleção [post](post.md)| Obtenha as postagens do thread especificado. |

## <a name="properties"></a>Propriedades
| Propriedade              | Tipo                                 | Descrição                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | Somente leitura. <br/><br/>Devolvido por padrão.                                                                                                                                                                                      |
| toRecipients          | Coleção [recipient](recipient.md) | Os destinatários Para: do thread. <br/><br/>Retornado apenas em $select.                                                                                                                                                               |
| ccRecipients          | Coleção [recipient](recipient.md) | Os destinatários Cc: do thread. <br/><br/>Retornado apenas em $select.                                                                                                                                                              |
| topic                 | String                               | O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada. <br/><br/>Retornado por padrão.                                                                              |
| hasAttachments        | Booliano                              | Indica se qualquer uma das postagens neste thread tem pelo menos um anexo. <br/><br/>Retornado por padrão.                                                                                                               |
| lastDeliveredDateTime | DateTimeOffset                       | O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br/><br/>Retornado por padrão. |
| uniqueSenders         | Coleção de cadeias de caracteres                    | Todos os usuários que enviaram uma mensagem para este thread. <br/><br/>Retornado por padrão.                                                                                                                                                |
| visualização               | String                               | Um breve resumo do corpo da postagem mais recente nesta conversa. <br/><br/>Retornado por padrão.                                                                                                                           |
| isLocked              | Booliano                              | Indica se o thread está bloqueado. <br/><br/>Retornado por padrão.                                                                                                                                                               |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|postagens|Coleção [post](post.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
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
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


