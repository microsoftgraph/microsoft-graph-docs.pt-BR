---
title: tipo de recurso de educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments.grading** . Isso é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
ms.openlocfilehash: f00014eab1dbf7bc8eb78a8898c6abba9977e8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860967"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>tipo de recurso de educationAssignmentPointsGradeType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Usada com a propriedade **assignments.grading** . Isso é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).

Isso indica que a atribuição varie e armazena o número máximo de pontos que cada estudante pode alcançar este item de trabalho. Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada a ela para o armazenamento de pontos de cada student.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|maxPoints|Single| Max aponta possíveis para essa atribuição.  |

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
