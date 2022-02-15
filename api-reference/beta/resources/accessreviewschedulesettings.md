---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, `accessReviewScheduleSettings` as configurações associadas a uma série de revisão de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb7dbc40944d42f50b68b82cf2be8a2499020f8a
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816053"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Booliano | Indica se os emails estão habilitados ou desabilitados. O valor padrão é `false`.               |
| reminderNotificationsEnabled|Booliano  | Indica se os lembretes estão habilitados ou desabilitados. O valor padrão é `false`.  |
| justificationRequiredOnApproval|Booliano | Indica se os revisadores são necessários para fornecer justificativa com sua decisão. O valor padrão é `false`. |
| defaultDecisionEnabled|Booliano | Indica se a decisão padrão está habilitada ou desabilitada quando os revisadores não respondem. O valor padrão é `false`. |
| defaultDecision|String | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser um dos `Approve`, `Deny`ou `Recommendation`. |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão (`accessReviewInstance`) em número de dias. <br/>**OBSERVAÇÃO:** Se **o stageSettings** do [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **durationInDays** será usada em vez do valor dessa propriedade. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. <br/><br/>**Observação:** Somente **as propriedades dayOfMonth**, **interval** e **type** (`weekly`, `absoluteMonthly`) são suportadas. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Booliano | Indica se as decisões são aplicadas automaticamente. Quando definido como `false`, um administrador deve aplicar as decisões manualmente depois que o revistor concluir a revisão de acesso. Quando definido como `true`, as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os revisadores responderam ou não. O valor padrão é `false`. |
| applyActions|[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a ser realizadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction`. O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction`. |
| recommendationsEnabled|Booliano | Indica se as recomendações de decisão estão habilitadas ou desabilitadas. <br/>**OBSERVAÇÃO:** Se **o stageSettings** do [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **recommendationsEnabled** será usada em vez do valor dessa propriedade. |
| recommendationLookBackDuration | Duration| Campo opcional. Indica o período de inatividade (em relação à data de início da instância de revisão) de onde as recomendações serão configuradas. A recomendação será para se `deny` o usuário estiver inativo durante a duração do retorno. Para análises de grupos e funções do Azure AD, qualquer duração é aceita. Para análises de aplicativos, 30 dias é a duração máxima. Se não for especificado, a duração será de 30 dias. <br/><br/>**OBSERVAÇÃO:** Se **o stageSettings** do [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **recommendationLookBackDuration** será usada em vez do valor dessa propriedade. |
|decisionHistoriesForReviewersEnabled|Booliano| Indica se as decisões sobre estágios anteriores de revisão de acesso estão disponíveis para revisores em **um accessReviewInstance** com vários estágios subsequentes. Se não for fornecido, o padrão será desabilitado (`false`).|
| recommendationInsightSettings|[coleção accessReviewRecommendationInsightSetting](../resources/accessReviewRecommendationInsightSetting.md) | Opcional. Descreve os tipos de insights que ajudam os revisadores a tomar decisões de revisão de acesso. <br/><br/>**OBSERVAÇÃO:** Se **o stageSettings** do [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) for definido, sua configuração **recommendationInsightSettings** será usada em vez do valor dessa propriedade. |

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
