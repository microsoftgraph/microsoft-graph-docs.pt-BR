---
title: tipo de recurso de chatMessage
description: Representa uma mensagem de bate-papo individuais dentro de uma entidade de bate-papo ou de canal. A mensagem pode ser uma mensagem de raiz ou a parte de um segmento que é definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: ad381102f7e93a4dcccd7b68435d0687ed6b4837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855988"
---
# <a name="chatmessage-resource-type"></a>tipo de recurso de chatMessage

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma mensagem de bate-papo individuais dentro de uma entidade de bate-papo ou de [canal](channel.md) . A mensagem pode ser uma mensagem de raiz ou a parte de um segmento que é definido pela propriedade **replyToId** na mensagem.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Mensagens de canal de lista](../api/channel-list-messages.md) | coleção [chatmessage](chatmessage.md) | Obter a lista de todas as mensagens de raiz em um canal.|
|[Mensagem de canal Get](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Obtenha uma mensagem de raiz única de um canal.|
|[Lista de respostas a uma mensagem](../api/channel-list-messagereplies.md) | coleção [chatmessage](chatmessage.md)| Obter a lista de todas as respostas a uma mensagem no canal.|
|[Obtenha uma resposta a uma mensagem](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Obtenha uma única resposta a uma mensagem em um canal.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Somente leitura. Identificação exclusiva da mensagem.|
|replyToId| string | ID da mensagem pai mensagem/raiz do thread |
|from|[identitySet](identityset.md)| Detalhes do remetente da mensagem|
|etag| string | Número de versão da mensagem |
|messageType|Cadeia de caracteres|Os valores de tipo de mensagem, atual com suporte são: mensagem, chatEvent, digitando|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de hora de quando a mensagem foi criada|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Carimbo de hora de quando a mensagem foi editado/atualizado|
|isDeleted|booliano|Representa se uma mensagem tiver sido excluída soft|
|deletedDateTime|dateTimeOffset|Somente leitura. Carimbo de hora em que a mensagem foi excluída. |
|subject|string|Linha de assunto da mensagem. Opcional|
|body|[itemBody](itembody.md)|Representação em texto sem formatação/HTML do conteúdo da mensagem. Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta|
|Resumo|string|Texto da mensagem que poderia ser usada para notificações por push e modos de exibição de resumo ou regressivo queda de modos de exibição de resumo|
|menções|coleção [chatMessageMention](chatmention.md)| Lista de entidades mencionado na mensagem. Suporta atualmente o usuário, bot, equipe, de canal|
|importance| string | A importância da mensagem: Normal, alta|
|reações| coleção [chatMessageReaction](chatreaction.md) | Reações para esta mensagem (por exemplo,-Like)|
|localidade|string|Localidade da mensagem definida pelo cliente|
|attachments|coleção [chatMessageAttachment](chatattachment.md) |Arquivos anexados|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
