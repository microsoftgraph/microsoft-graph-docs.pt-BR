---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso Azure AD revisões de acesso, representa `accessReviewScheduleSettings` as configurações associadas a uma série de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf56ecef7491c74de864f647b34086cf658f33e6
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697141"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | Indica se os emails estão habilitados ou desabilitados. O valor padrão é `false`.               |
| reminderNotificationsEnabled|Booliano  | Indica se os lembretes estão habilitados ou desabilitados. O valor padrão é `false`.  |
| justificationRequiredOnApproval|Booleano | Indica se os revisores são necessários para fornecer justificativa com sua decisão. O valor padrão é `false`. |
| defaultDecisionEnabled|Booleano | Indica se a decisão padrão está habilitada ou desabilitada quando os revisores não respondem. O valor padrão é `false`. |
| defaultDecision|Cadeia de Caracteres | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser um de `Approve`, `Deny`ou `Recommendation`. |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão (`accessReviewInstance`) em número de dias. <br/>**NOTA:** Se **o stageSettings** do objeto [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **durationInDays** será usada em vez do valor dessa propriedade. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto de recorrência padrão do Outlook. <br/><br/>**Nota:** Somente **as propriedades dayOfMonth**, **interval** e **type** (`weekly`, `absoluteMonthly`) têm suporte. Use a propriedade **startDate** **em recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Boolean | Indica se as decisões são aplicadas automaticamente. Quando definido como `false`, um administrador deve aplicar as decisões manualmente depois que o revisores concluir a revisão de acesso. Quando definido como `true`, as decisões são aplicadas automaticamente após o término da duração da instância de revisão de acesso, independentemente de os revisores responderem ou não. O valor padrão é `false`. |
| applyActions|[coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a serem tomadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction`. O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction`. |
| recommendationsEnabled|Booleano | Indica se as recomendações de decisão estão habilitadas ou desabilitadas. <br/>**NOTA:** Se **o stageSettings** do objeto [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **recommendationsEnabled** será usada em vez do valor dessa propriedade. |
| recommendationLookBackDuration | Duração| Campo opcional. Indica o período de inatividade (em relação à data de início da instância de revisão) do qual as recomendações serão configuradas. A recomendação será se `deny` o usuário estiver inativo durante a duração da pesquisa. Para revisões de grupos e Azure AD funções, qualquer duração é aceita. Para revisões de aplicativos, 30 dias é a duração máxima. Se não for especificado, a duração será de 30 dias. <br/><br/>**NOTA:** Se **o stageSettings** do objeto [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **recommendationLookBackDuration** será usada em vez do valor dessa propriedade. |
|decisionHistoriesForReviewersEnabled|Booleano| Indica se as decisões sobre estágios anteriores de revisão de acesso estão disponíveis para revisores em **um accessReviewInstance** com vários estágios subsequentes. Se não for fornecido, o padrão será desabilitado (`false`).|
| recommendationInsightSettings|[coleção accessReviewRecommendationInsightSetting](../resources/accessReviewRecommendationInsightSetting.md) | Opcional. Descreve os tipos de insights que auxiliam os revisores a tomar decisões de revisão de acesso. <br/><br/>**NOTA:** Se **o stageSettings** do objeto [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **recommendationInsightSettings** será usada em vez do valor dessa propriedade. |

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
  "recommendationsEnabled": "Boolean",
  "recommendationLookBackDuration": "Duration",
  "decisionHistoriesForReviewersEnabled": "Boolean",
  "recommendationInsightSettings": [
    {
      "@odata.type": "microsoft.graph.accessReviewRecommendationInsightSetting"
    }
  ]
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
