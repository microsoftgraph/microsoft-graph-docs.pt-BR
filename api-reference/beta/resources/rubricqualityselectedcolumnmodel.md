---
title: tipo de recurso rubricQualitySelectedColumnModel
description: Indica o rubricLevel selecionado pelo professor ao gradar um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9c8b6264a0373fb5b388cd95771d9360b867feb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520988"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a>tipo de recurso rubricQualitySelectedColumnModel

Namespace: Microsoft. Graph

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