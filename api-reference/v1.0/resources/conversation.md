---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b15d4fd7d3ed1688fd27fed7a101fb0d9aed37ba
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513605"
---
# <a name="conversation-resource-type"></a>tipo de recurso conversation

Namespace: microsoft.graph

Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.

Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar conversas](../api/group-list-conversations.md) | Coleção [conversation](conversation.md) |Obtenha a lista de conversas desse grupo.|
|[Create](../api/group-post-conversations.md) |[conversation](conversation.md)| Crie uma nova conversa incluindo um thread e uma postagem.|
|[Obter conversa](../api/conversation-get.md) | [conversation](conversation.md) |Leia as propriedades e os relacionamentos do objeto conversation.|
|[Delete](../api/conversation-delete.md) | Nenhum |Excluir objeto conversation. |
|[Listar threads de conversas](../api/conversation-list-threads.md) |Coleção [conversationThread](conversationthread.md)| Obtenha todos os threads em uma conversa de grupo.|
|[Criar thread de conversas](../api/conversation-post-threads.md) |Coleção [conversationThread](conversationthread.md)| Crie um thread na conversa especificada.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|hasAttachments|Booliano|Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo. Suporta `$filter` ( , ) e `eq` `ne` `$search` .|
|id|Cadeia de caracteres|Identificador exclusivo de conversas. Somente leitura.|
|lastDeliveredDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|visualização|String|Um breve resumo do corpo da postagem mais recente nesta conversa. Suporta `$filter` (`eq`, `ne`, `le`, `ge`).|
|topic|String|O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.|
|uniqueSenders|Coleção de cadeias de caracteres|Todos os usuários que enviaram uma mensagem para esta conversa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|threads|Coleção [conversationThread](conversationthread.md)|Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

