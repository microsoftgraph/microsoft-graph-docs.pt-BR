---
title: tipo de recurso educationAssignmentPointsGradeType
description: Tipo de recurso usado com a **propriedade assignments.grading.** Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 344ee57fcf08cad2c39020a60f5264b75f23404863c2709e3706eda2fd3e234f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231814"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>tipo de recurso educationAssignmentPointsGradeType

Namespace: microsoft.graph

Tipo de recurso usado com a **propriedade assignments.grading.** Esta é uma subclasse [de educationAssignmentGradeType](educationassignmentgradetype.md).

Isso indica que a atribuição é gradeada e armazena o número máximo de pontos que cada aluno pode alcançar neste item de trabalho. Quando isso for definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada a ela para o armazenamento dos pontos de cada aluno.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|maxPoints|Único| Pontos máximos possíveis para essa atribuição.  |

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


