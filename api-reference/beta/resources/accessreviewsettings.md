---
title: tipo de recurso accessReviewSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 21915811da771bd0eebdb5fb2c16df5cfbdea096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508454"
---
# <a name="accessreviewsettings-resource-type"></a>tipo de recurso accessReviewSettings

Namespace: Microsoft. Graph

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



