---
title: tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade **enmisse.** Isso cria uma subclasse de educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c2ef014c3e9e2954dba5fb759fcf3f86b3681b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502505"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>tipo de recurso educationAssignmentPointsGrade

Namespace: Microsoft. Graph

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
