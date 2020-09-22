---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: d4ed317b987d461c9ef6816e9d05aae0de358ec7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037196"
---
# <a name="imageinfo-resource-type"></a>tipo de recurso imageInfo

Namespace: microsoft.graph

Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|iconUrl | String | Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade|
|alternateText | String | Opcion Alt-conteúdo de texto acessível para a imagem|
|addImageQuery | Boolean | Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização. Por exemplo, uma imagem de alto contraste|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

