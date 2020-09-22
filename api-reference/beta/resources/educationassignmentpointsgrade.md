---
title: tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade **enmisse.** Isso cria uma subclasse de educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bcce2fc6445c465defb2d795f3bfab9545838643
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013711"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>tipo de recurso educationAssignmentPointsGrade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade **enmisse.** Isso cria uma subclasse de [educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade. O máximo de pontos é armazenado na propriedade **assignments. Grading** .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|points|Único|Número de pontos que um professor está dando este objeto de envio.|

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


