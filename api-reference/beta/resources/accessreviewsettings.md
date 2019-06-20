---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084065"
---
# <a name="accessreviewsettings-resource-type"></a>tipo de recurso accessReviewSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| mailNotificationsEnabled | booliano |  |
| remindersEnabled | booliano |  |
| justificationRequiredOnApproval | booliano |  |
| recurrenceSettings | accessReviewRecurrenceSettings |  |
| autoReviewEnabled | booliano |  |
| activityDurationInDays | Int32 |  |
| autoReviewSettings | autoReviewSettings |  |
| autoApplyReviewResultsEnabled | booliano |  |
| accessRecommendationsEnabled | booliano |  |


## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



