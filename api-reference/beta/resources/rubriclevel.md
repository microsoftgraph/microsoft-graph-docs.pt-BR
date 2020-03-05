---
title: tipo de recurso rubricLevel
description: Um nível de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 24af9e9be6dc9b63934a02193958e0267dde8dea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521009"
---
# <a name="rubriclevel-resource-type"></a>tipo de recurso rubricLevel

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um nível de um amostra rubric. Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|A descrição desse nível de amostra rubric.|
|displayName|String|O nome desse nível de amostra rubric.|
|notas|[educationAssignmentGradeType](educationassignmentgradetype.md)|NULL se for um amostra rubric sem pontos; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) se for um ponto amostra rubric.|
|levelid|String|A ID desse recurso.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->