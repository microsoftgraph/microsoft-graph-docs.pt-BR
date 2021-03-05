---
title: Tipo de recurso timeConstraint
description: Restringe sugestões de hora de reunião a determinados horários e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo de abertura.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d79fc1630522c30abea6ac5ec6f51d0f5a15e437
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472101"
---
# <a name="timeconstraint-resource-type"></a>Tipo de recurso timeConstraint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Restringe sugestões de hora de reunião a determinados horários e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo de abertura.


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
|activityDomain|activityDomain|A natureza da atividade, opcional. Os valores possíveis são: `work` `personal` , , ou `unrestricted` `unknown` .|
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
  "suppressions": []
}
-->


