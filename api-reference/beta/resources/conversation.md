---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7d489a75f72a705a77231af940094b7aa2d18fe1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528645"
---
# <a name="conversation-resource-type"></a>tipo de recurso conversation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.

Este recurso oferece suporte a assinatura de [notificações de alteração](/graph/webhooks).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar conversas](../api/group-list-conversations.md) | Coleção [conversation](conversation.md) |Obtenha a lista de conversas desse grupo.|
|[Create](../api/group-post-conversations.md) |[conversation](conversation.md)| Crie uma nova conversa incluindo um thread e uma postagem.|
|[Obter conversa](../api/conversation-get.md) | [conversation](conversation.md) |Leia as propriedades e os relacionamentos do objeto conversation.|
|[Delete](../api/conversation-delete.md) | Nenhum |Exclua um objeto conversation. |
|[Listar threads de conversas](../api/conversation-list-threads.md) |Coleção [conversationThread](conversationthread.md)| Obtenha todos os threads em uma conversa de grupo.|
|[Criar thread de conversas](../api/conversation-post-threads.md) |Coleção [conversationThread](conversationthread.md)| Crie um thread na conversa especificada.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|hasAttachments|Booliano|Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.|
|id|String|Identificador exclusivo de conversas. Somente leitura.|
|lastDeliveredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/conversation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
