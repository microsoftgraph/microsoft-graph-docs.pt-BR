---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a57155a880e9ba4e00dd9a4d17ddae3742bbaa8e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807476"
---
# <a name="imageinfo-resource-type"></a>tipo de recurso imageInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|iconUrl | String | Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade|
|alternateText | String | Opcion Alt-conteúdo de texto acessível para a imagem|
|addImageQuery | Booliano | Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização. Por exemplo, uma imagem de alto contraste|

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
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
