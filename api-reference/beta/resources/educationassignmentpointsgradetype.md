---
title: tipo de recurso educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 61e6e425730685d4447875cdb074526e7ebc0a17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334427"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>tipo de recurso educationAssignmentPointsGradeType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).

Isso indica que a atribuição foi classificada e armazena o número máximo de pontos que cada aluno pode obter nesse item de trabalho. Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada ao armazenamento dos pontos de cada aluno.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|maxPoints|Único| Máximo de pontos possíveis para esta atribuição.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
