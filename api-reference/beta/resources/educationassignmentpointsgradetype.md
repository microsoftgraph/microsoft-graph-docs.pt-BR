---
title: tipo de recurso de educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments.grading** . Isso é uma subclasse de educationAssignmentGradeType.
ms.openlocfilehash: 5c170540e99003a78df0550d4d6542c07df8f1ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040151"
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