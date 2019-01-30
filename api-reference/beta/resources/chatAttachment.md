---
title: tipo de recurso de chatMessageAttachment
description: Representa um anexo para uma entidade de mensagem de chat.
localization_priority: Normal
ms.openlocfilehash: 12682ee090a2dc7976db46629cd26df9e5b1595e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640914"
---
# <a name="chatmessageattachment-resource-type"></a>tipo de recurso de chatMessageAttachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um anexo para uma entidade de mensagem de chat.

Uma entidade do tipo `chatMessageAttachment` é retornado como parte de [receber mensagens de canal](../api/channel-list-messages.md) API, como parte da entidade [chatMessage](chatmessage.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string| Somente leitura. Id exclusiva do anexo.|
|contentType| string | O tipo de mídia do conteúdo anexo. Ele pode ter os seguintes valores: <br><ul><li>referência: anexo é um link para outro arquivo. Preencha o contentURL com o link para o objeto.<br></li><li>arquivo: anexo de arquivo Raw. Preencher o campo contenturl com a codificação base64 do arquivo de dados: formato.<br></li><li>imagem /: tipo de imagem com o tipo da imagem especificada ex.: image/png, image/jpeg, image/gif. Preencher o campo contentUrl com a codificação base64 do arquivo de dados: formato.<br></li><li>vídeo /: tipo de vídeo com o formato especificado. Ex.: vídeo/mp4. Preencher o campo contentUrl com a codificação base64 do arquivo de dados: formato.<br></li><li>áudio /: tipo de áudio com o formato especificado. Ex.: áudio/wmw. Preencher o campo contentUrl com a codificação base64 do arquivo de dados: formato.<br></li><li>tipo de aplicativo/cartão: tipo de anexo com o tipo de cartão especificando o formato de cartão exato usar de cartão de Rich. Defina o conteúdo com o formato json do cartão. Valores suportados para o tipo de cartão incluem:<br><ul><li>application/vnd.microsoft.Card.Adaptive: um cartão avançado que pode conter qualquer combinação de texto, fala, imagens, botões e campos de entrada. Defina a propriedade de conteúdo, para um objeto AdaptiveCard.</li><li>application/vnd.microsoft.Card.Animation: um cartão avançado que reproduz a animação. Defina a propriedade de conteúdo, como um AnimationCardobject.</li><li>application/vnd.microsoft.Card.Audio: um cartão avançado que reproduz arquivos de áudio. Defina a propriedade de conteúdo, como um objeto AudioCard.</li><li>application/vnd.microsoft.Card.Video: um cartão avançado que reproduz vídeos. Defina a propriedade de conteúdo, como um objeto de placa de vídeo.</li><li>application/vnd.microsoft.Card.Hero: um cartão herói. Defina a propriedade de conteúdo a um objeto HeroCard.</li><li>application/vnd.microsoft.Card.Thumbnail: um cartão de miniatura. Defina a propriedade de conteúdo a um objeto ThumbnailCard.</li><li>application/vnd.microsoft.com.Card.Receipt: um cartão de recebimento. Defina a propriedade de conteúdo a um objeto ReceiptCard.</li><li>application/vnd.microsoft.com.Card.signin: um cartão de logon do usuário. Defina a propriedade de conteúdo a um objeto SignInCard.</ul></ul>|
|contentUrl|string|URL para o conteúdo do anexo. Suporte para protocolos: http, https, arquivos e dados.|
|content|string|O conteúdo do anexo. Se o anexo é um cartão de rich, defina a propriedade ao objeto rich cartão. Essa propriedade e contentUrl são mutuamente exclusivos.|
|name|string|Nome do anexo.|
|thumbnailUrl| string |URL para um uma imagem em miniatura que o canal pode usar se ele suporta o uso de um formulário alternativo, menor de conteúdo ou contentUrl. Por exemplo, se você definir contentType para o aplicativo/word e defina contentUrl até o local do documento do Word, você pode incluir uma imagem em miniatura que representa o documento. O canal pode exibir a imagem em miniatura, em vez do documento. Quando o usuário clica na imagem, o canal abria o documento.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatAttachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
