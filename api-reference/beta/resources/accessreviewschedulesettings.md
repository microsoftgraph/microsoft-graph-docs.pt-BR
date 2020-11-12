---
title: tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões do Azure AD Access, o `accessReviewScheduleSettings` representa as configurações associadas a uma série de análise do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cca1fa7fd0da05719c22728dd472087d9737d4e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000769"
---
# <a name="accessreviewschedulesettings-resource-type"></a>tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **accessReviewScheduleSettings** define as configurações de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Booliano | Sinalizador para indicar se os emails estão habilitados/desabilitados.                |
| reminderNotificationsEnabled|Booliano  | Sinalizador para indicar se lembretes estão habilitados/desabilitados.   |
| justificationRequiredOnApproval|Booliano | Sinalizador para indicar se os revisores são necessários para fornecer justificação à sua decisão. |
| defaultDecisionEnabled|Booliano | Sinalizador para indicar se a decisão padrão será habilitada/desabilitada quando os revisores não responderem. |
| decisão|Cadeia de caracteres | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser uma das "aprovar", "negar" ou "recomendação". |
| instanceDurationInDays|Int32 | Duração de cada recorrência de Review ( `accessReviewInstance` ) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Definições detalhadas de recorrência. Usando o objeto recorrência padrão do Outlook.  |
| autoApplyDecisionsEnabled|Booliano | Sinalizador para indicar se o recurso de aplicação automática está habilitado. |
| applyActions|coleção [accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a serem tomadas após a conclusão da revisão. Há dois tipos suportados atualmente: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` . Field só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` . Consulte [accessReviewApplyAction](accessreviewapplyaction.md). |
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
