---
title: Tipo de recurso timeConstraint
description: Restringe sugestões de hora de reunião a determinados horários e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo de abertura.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7b5ed13c523fca24d9b8fad79f6271d4333177c7d2d0f2eece5354423ba370d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221176"
---
# <a name="timeconstraint-resource-type"></a>Tipo de recurso timeConstraint

Namespace: microsoft.graph

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
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

