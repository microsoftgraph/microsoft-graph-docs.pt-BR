---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.
localization_priority: Normal
ms.openlocfilehash: 45469211aa4925834fd9d20da6a9905ac87d221e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577232"
---
# <a name="timeconstraint-resource-type"></a>Tipo de recurso timeConstraint

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activityDomain|String|A natureza da atividade, opcional. Os valores possíveis são: `work`, `personal`, `unrestricted` ou `unknown`.|
|intervalos de tempo|Coleção [timeSlot](timeslot.md)|Uma matriz de períodos de tempo.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
