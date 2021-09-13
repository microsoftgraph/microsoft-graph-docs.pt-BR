---
title: Tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grau de pontos, cada envio terá esse objeto associado à **propriedade submission.grade.**
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 91dbdc6a6a94a296dffafe32d6d6021dd23d3371
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109147"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Tipo de recurso educationAssignmentPointsGrade

Namespace: microsoft.graph

Quando uma atribuição é definida como um tipo de grau de pontos, cada envio terá esse objeto associado à **propriedade submission.grade.** Isso cria uma subclasse [de educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade. Os pontos máximos são armazenados na **propriedade assignments.grading.**


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|points|Simples|Número de pontos que um professor está dando a esse objeto de envio.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


