---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a uma série de revisão `accessReviewScheduleSettings` de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77ea7d8601df36525aad7a3448aa3b6f031d98d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469315"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Booliano | Sinalizador para indicar se os emails estão habilitados/desabilitados.                |
| reminderNotificationsEnabled|Booliano  | Sinalizador para indicar se os lembretes estão habilitados/desabilitados.   |
| justificationRequiredOnApproval|Booliano | Sinalizador para indicar se os revisadores são necessários para fornecer justificativa com sua decisão. |
| defaultDecisionEnabled|Booliano | Sinalizador para indicar se a decisão padrão está habilitada/desabilitada quando os revisadores não respondem. |
| defaultDecision|String | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser um de "Aprovar", "Negar" ou "Recomendação". |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias. |
| recorrência|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência. Usando o objeto de recorrência padrão do Outlook. Observe que dayOfMonth não tem suporte - use a propriedade startDate em recurrenceRange para determinar o dia em que a revisão será iniciada. |
| autoApplyDecisionsEnabled|Booliano | Sinalizador para indicar se o recurso de aplicação automática está habilitado. |
| applyActions|[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a ser realizadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` . O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` . Consulte [accessReviewApplyAction](accessreviewapplyaction.md). |
| recommendationsEnabled|Booliano | Sinalizador para indicar se as recomendações de decisão estão habilitadas/desabilitadas. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
