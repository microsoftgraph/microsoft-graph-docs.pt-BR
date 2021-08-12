---
title: Tipo de recurso rubricLevel
description: Um nível de rubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef944854949e590abc5a3455cc9683d18f069ebb932be337eb6351d64899fd09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249129"
---
# <a name="rubriclevel-resource-type"></a>Tipo de recurso rubricLevel

Namespace: microsoft.graph

Um nível de rubric. 

Consulte [educationRubric](educationrubric.md) para ver uma descrição da relação entre as qualidades *rubricas,* níveis e *critérios.*

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|A descrição desse nível rubrico.|
|displayName|Cadeia de caracteres|O nome desse nível rubrico.|
|grading|[educationAssignmentGradeType](educationassignmentgradetype.md)|Null se for uma rubrica sem pontos; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) se for uma rubrica de pontos.|
|levelId|Cadeia de caracteres|A ID desse recurso.|

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

