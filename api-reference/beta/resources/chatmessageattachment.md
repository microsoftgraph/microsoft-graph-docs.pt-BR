---
title: tipo de recurso chatMessageAttachment
description: Representa um anexo a uma entidade de mensagem de chat.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1b9ddbb0b8dac124370b1d20ac42e3ab1da7d1e3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791080"
---
# <a name="chatmessageattachment-resource-type"></a>tipo de recurso chatMessageAttachment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um anexo a uma entidade de mensagem de chat.

Uma entidade do tipo `chatMessageAttachment` é retornada como parte da API [Get Channel messages](../api/channel-list-messages.md) , como parte da entidade [chat](chatmessage.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres| Somente leitura. ID exclusiva do anexo.|
|contentType| string | O tipo de mídia do anexo de conteúdo. Ele pode ter os seguintes valores: <br><ul><li>`reference`: O anexo é um link para outro arquivo. Preencha o contentURL com o link para o objeto.</li><li>Quaisquer contentTypes compatíveis com o [objeto Attachment](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object) da estrutura de bot</li><li>`application/vnd.microsoft.card.codesnippet`: Um trecho de código. </li><li>`application/vnd.microsoft.card.announcement`: Um cabeçalho de comunicado. </li>|
|contentUrl|string|URL para o conteúdo do anexo. Protocolos suportados: http, HTTPS, File e data.|
|conteúdo|string|O conteúdo do anexo. Se o anexo for um [cartão rico](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), defina a propriedade com o objeto ficha avançada. Essa propriedade e contentUrl são mutuamente exclusivas.|
|nome|string|Nome do anexo.|
|thumbnailUrl| string |URL para uma imagem em miniatura que o canal pode usar se oferecer suporte ao uso de um formato de conteúdo ou de uma alternativa menor ou contentUrl. Por exemplo, se você definir contentType como Application/Word e definir contentUrl como o local do documento do Word, você pode incluir uma imagem em miniatura que representa o documento. O canal pode exibir a imagem em miniatura em vez do documento. Quando o usuário clica na imagem, o canal abre o documento.|

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
