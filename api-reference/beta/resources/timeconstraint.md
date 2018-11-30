---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.
ms.openlocfilehash: 092133d34e12fe5c06bfd8a76e8a33afb33892f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034364"
---
# <a name="timeconstraint-resource-type"></a>Tipo de recurso timeConstraint

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
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
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->