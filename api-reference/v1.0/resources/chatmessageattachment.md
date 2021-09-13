---
title: Tipo de recurso chatMessageAttachment
description: Representa um anexo a uma entidade de mensagem de chat.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: 1b02a5c034be39ee9eeb941b7fe875e8d4c9e8c1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094412"
---
# <a name="chatmessageattachment-resource-type"></a>Tipo de recurso chatMessageAttachment

Namespace: microsoft.graph

Representa um anexo a uma entidade de mensagem de chat.

Uma entidade de tipo é retornada como parte da API Obter mensagens `chatMessageAttachment` [de](../api/channel-list-messages.md) canal, como parte da [entidade chatMessage.](chatmessage.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres| Somente leitura. ID exclusiva do anexo.|
|contentType| cadeia de caracteres | O tipo de mídia do anexo de conteúdo. Ele pode ter os seguintes valores: <br><ul><li>`reference`: Attachment é um link para outro arquivo. Preencha o contentURL com o link para o objeto.</li><li>Quaisquer contentTypes suportados pelo objeto Attachment da Estrutura de [Bot](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</li><li>`application/vnd.microsoft.card.codesnippet`: Um trecho de código. </li><li>`application/vnd.microsoft.card.announcement`: Um header de comunicado. </li>|
|contentUrl|string|URL do conteúdo do anexo. Protocolos com suporte: http, https, arquivo e dados.|
|conteúdo|cadeia de caracteres|O conteúdo do anexo. Se o anexo for um [cartão rich ,](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)de definir a propriedade como o objeto rich card. Essa propriedade e contentUrl são mutuamente exclusivos.|
|nome|string|Nome do anexo.|
|thumbnailUrl| cadeia de caracteres |URL para uma imagem em miniatura que o canal pode usar se for compatível com o uso de uma forma alternativa, menor de conteúdo ou contentUrl. Por exemplo, se você definir contentType como aplicativo/word e definir contentUrl como o local do documento do Word, poderá incluir uma imagem em miniatura que representa o documento. O canal poderia exibir a imagem em miniatura em vez do documento. Quando o usuário clica na imagem, o canal abriria o documento.|

## <a name="json-representation"></a>Representação JSON
 Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

