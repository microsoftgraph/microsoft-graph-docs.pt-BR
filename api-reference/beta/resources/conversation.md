---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b3dd263a91552afc4db42cb2cc1791741dc24473
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721664"
---
# <a name="conversation-resource-type"></a>tipo de recurso conversation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|hasAttachments|Booliano|Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.|
|id|Cadeia de caracteres|Identificador exclusivo de conversas. Somente leitura.|
|lastDeliveredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|visualização|String|Um breve resumo do corpo da última postagem nesta conversa.|
|topic|String|O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.|
|uniqueSenders|Coleção de cadeias de caracteres|Todos os usuários que enviaram uma mensagem para esta conversa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|threads|Coleção [conversationThread](conversationthread.md)|Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


