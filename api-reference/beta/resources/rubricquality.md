---
title: tipo de recurso rubricQuality
description: Uma qualidade de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fd8ad7aa7d0a19fe1774e18bba5d59af52140
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173304"
---
# <a name="rubricquality-resource-type"></a>tipo de recurso rubricQuality

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma qualidade de um amostra rubric. Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|criteria|coleção [rubricCriterion](rubriccriterion.md)|O conjunto de critérios para esta qualidade de amostra rubric.|
|descrição|[itemBody](itembody.md)|A descrição dessa qualidade de amostra rubric.|
|displayName|String|O nome dessa qualidade de amostra rubric.|
|qualityid|String|A ID desse recurso.|
|weight|Único|Se presente, um peso numérico para essa qualidade.  Os pesos devem adicionar até 100.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->