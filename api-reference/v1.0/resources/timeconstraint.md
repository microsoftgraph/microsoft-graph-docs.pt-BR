---
title: Tipo de recurso timeConstraint
description: Restringe sugestões de hora de reunião a determinados horários e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo de abertura.
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6822aab3521464842278f80fa323da039506afa9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122926"
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

