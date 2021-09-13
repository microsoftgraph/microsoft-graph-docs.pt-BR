---
title: tipo de recurso educationAssignmentPointsGradeType
description: Tipo de recurso usado com a **propriedade assignments.grading.** Esta é uma subclasse de educationAssignmentGradeType.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5c2a59a9f34d2be02415021ece777021dacb34bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036743"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>tipo de recurso educationAssignmentPointsGradeType

Namespace: microsoft.graph

Tipo de recurso usado com a **propriedade assignments.grading.** Esta é uma subclasse [de educationAssignmentGradeType](educationassignmentgradetype.md).

Isso indica que a atribuição é gradeada e armazena o número máximo de pontos que cada aluno pode alcançar neste item de trabalho. Quando isso for definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada a ela para o armazenamento dos pontos de cada aluno.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|maxPoints|Simples| Pontos máximos possíveis para essa atribuição.  |

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
  "maxPoints": "Double"
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


