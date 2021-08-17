---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a uma série de revisão `accessReviewScheduleSettings` de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23174a0286220175104973290fd00c39bbbaa941
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262449"
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
| reminderNotificationsEnabled|Boolean  | Indica se os lembretes estão habilitados ou desabilitados. O valor padrão é `false`.  |
| justificationRequiredOnApproval|Boolean | Indica se os revisadores são necessários para fornecer justificativa com sua decisão. O valor padrão é `false`. |
| defaultDecisionEnabled|Boolean | Indica se a decisão padrão está habilitada ou desabilitada quando os revisadores não respondem. O valor padrão é `false`. |
| defaultDecision|Cadeia de caracteres | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser um `Approve` dos `Deny` , ou `Recommendation` . |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. Somente `weekly` e `absoluteMonthly` em **recorrênciaPattern** são suportados. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Boolean | Indica se as decisões são aplicadas automaticamente. Quando definido como , um usuário deve aplicar as decisões manualmente depois que o `false` revistor concluir a revisão de acesso. Quando definido como , as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os `true` revisadores responderam ou não. O valor padrão é `false`. |
| applyActions|[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a ser realizadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` . O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` . Consulte [accessReviewApplyAction](accessreviewapplyaction.md). |
| recommendationsEnabled|Boolean | Indica se as recomendações de decisão estão habilitadas/desabilitadas. |
| recommendationLookBackDuration | Duration| Campo opcional. Indica o período de inatividade (em relação à data de início da instância de revisão) de onde as recomendações serão configuradas. A recomendação será para `deny` se o usuário estiver inativo durante a duração de retorno. As durações suportadas são 30, 60 ou 90 dias.  |

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
  "recommendationLookBackDuration": "Duration"
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
