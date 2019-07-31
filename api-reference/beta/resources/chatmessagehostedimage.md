---
title: tipo de recurso chatMessageHostedImage
description: Representa uma imagem hospedada dentro de um chat.
localization_priority: Normal
author: clearab
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e217234b8ea6c6510b85af1bf1002e589e4366e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974000"
---
# <a name="chatmessagehostedimage-resource-type"></a>tipo de recurso chatMessageHostedImage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma imagem hospedada dentro de um [chat](../resources/chatmessage.md).

Imagens hospedadas são as imagens que aparecem no corpo da mensagem **. o conteúdo** em \<uma marca img> com um atributo src que começa `https://graph.microsoft.com`com.

Nem todas as imagens em uma mensagem são hospedadas, o Microsoft Teams também oferece suporte a imagens públicas (onde o atributo img src aponta para um site público).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar chatMessageHostedImages em um chat](../api/chatmessagehostedimage-list-hostedimages.md) | coleção [chatMessageHostedImage](chatmessagehostedimage.md) | Lista de todas as imagens hospedadas em um **chat**.|
|[Obter chatMessageHostedImage](../api/chatmessagehostedimage-get.md) | [chatMessageHostedImage](chatmessagehostedimage.md) | Obtenha uma única imagem hospedada.|
|[chatMessageHostedImage: GetBytes](../api/chatmessagehostedimage-getbytes.md) | Tipo de conteúdo: image/jpeg | Obtenha os bytes brutos da imagem hospedada.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID única da mensagem.|
|URL| string | A URL da qual recuperar o conteúdo da imagem.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
