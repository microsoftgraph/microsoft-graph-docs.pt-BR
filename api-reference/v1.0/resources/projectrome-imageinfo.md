---
title: Tipo de recurso imageInfo
description: Um tipo complexo para representar **a propriedade de atribuição** na parte visualInfo do objeto activity.
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: cf76bd7e81f913f9641568bbd20c62a1c3ed16a8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019192"
---
# <a name="imageinfo-resource-type"></a>Tipo de recurso imageInfo

Namespace: microsoft.graph

Um tipo complexo para representar **a propriedade de atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do [objeto activity.](../resources/projectrome-activity.md)

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|iconUrl | Cadeia de caracteres | Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade|
|alternateText | Cadeia de caracteres | Opcional; alt-text accessible content for the image|
|addImageQuery | Boolean | Opcional; usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização. Por exemplo: uma imagem de alto contraste|

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

