---
title: tipo de recurso rubricQualitySelectedColumnModel
description: Indica o rubricLevel selecionado pelo professor ao gradar um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6fd6ff5d9def23a6a6fb180c8d12398437e5dce0
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173290"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a>tipo de recurso rubricQualitySelectedColumnModel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica o [rubricLevel](rubriclevel.md) selecionado pelo professor ao gradar um [educationRubric](educationrubric.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|columnId|String|ID do nível selecionado para essa qualidade.|
|qualityid|String|ID da qualidade associada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->