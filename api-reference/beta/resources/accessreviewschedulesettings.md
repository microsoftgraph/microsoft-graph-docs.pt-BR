---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a uma série de revisão `accessReviewScheduleSettings` de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1b12647e650567a9855a5aed3f15ec657a9c62d1
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525971"
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
| defaultDecision|Cadeia de caracteres | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser um `Approve` dos `Deny` , ou `Recommendation` . |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. <br/><br/>**Observação:** Somente `weekly` e `absoluteMonthly` em **recorrênciaPattern** são suportados. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Booliano | Indica se as decisões são aplicadas automaticamente. Quando definido como , um administrador deve aplicar as decisões manualmente depois que o `false` revistor concluir a revisão de acesso. Quando definido como , as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os `true` revisadores responderam ou não. O valor padrão é `false`. |
| applyActions|[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a ser realizadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` . O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` . |
| recommendationsEnabled|Booliano | Indica se as recomendações de decisão estão habilitadas ou desabilitadas. |
| recommendationLookBackDuration | Duração| Campo opcional. Indica o período de inatividade (em relação à data de início da instância de revisão) de onde as recomendações serão configuradas. A recomendação será para `deny` se o usuário estiver inativo durante a duração de retorno. Para análises de grupos e funções do Azure AD, qualquer duração é aceita. Para análises de aplicativos, 30 dias é a duração máxima. Se não for especificado, a duração será de 30 dias. |

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
