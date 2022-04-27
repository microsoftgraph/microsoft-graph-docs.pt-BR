---
title: Tipo de recurso chatMessageAttachment
description: Representa um anexo a uma entidade de mensagem de chat.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: caf7d1693395d9272a8999910dcaa29a9bef11da
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060755"
---
# <a name="chatmessageattachment-resource-type"></a>Tipo de recurso chatMessageAttachment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um anexo a uma entidade de mensagem de chat.

Uma entidade de tipo `chatMessageAttachment` é retornada como parte da API Obter mensagens [de](../api/channel-list-messages.md) canal, como parte da [entidade chatMessage](chatmessage.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres| Somente leitura. ID exclusiva do anexo.|
|contentType| string | O tipo de mídia do anexo de conteúdo. Ele pode ter os seguintes valores: <br><ul><li>`reference`: o anexo é um link para outro arquivo. Preencha a contentURL com o link para o objeto.</li><li>Qualquer contentTypes compatível com o objeto [Attachment](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object) do Bot Framework</li><li>`application/vnd.microsoft.card.codesnippet`: um snippet de código. </li><li>`application/vnd.microsoft.card.announcement`: um cabeçalho de comunicado. </li>|
|contentUrl|string|URL para o conteúdo do anexo. Protocolos com suporte: http, https, arquivo e dados.|
|conteúdo|string|O conteúdo do anexo. Se o anexo for um [cartão avançado](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), defina a propriedade como o objeto rich card. Essa propriedade e contentUrl são mutuamente exclusivos.|
|nome|string|Nome do anexo.|
|teamsAppId| string |A ID do Teams que está associado ao anexo. A propriedade é usada especificamente para atribuir um Teams de mensagem ao aplicativo especificado.|
|thumbnailUrl| string |URL para uma imagem em miniatura que o canal pode usar se der suporte ao uso de uma forma alternativa e menor de conteúdo ou contentUrl. Por exemplo, se você definir contentType como application/word e definir contentUrl como o local do documento do Word, poderá incluir uma imagem em miniatura que representa o documento. O canal pode exibir a imagem em miniatura em vez do documento. Quando o usuário clica na imagem, o canal abre o documento.|


## <a name="json-representation"></a>Representação JSON
 Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl",
    "teamsAppId"
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
  "teamsAppId": "string",
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


