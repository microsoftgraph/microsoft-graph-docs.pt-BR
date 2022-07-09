---
title: Tipo de recurso accessReviewScheduleSettings
description: Representa as configurações associadas a uma série de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb647faa01fe5dcc296f18c9dcc1ad00957c2253
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698433"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| mailNotificationsEnabled|Boolean | Indica se os emails estão habilitados ou desabilitados. O valor padrão é `false`.               |
| reminderNotificationsEnabled|Booliano  | Indica se os lembretes estão habilitados ou desabilitados. O valor padrão é `false`.  |
| justificationRequiredOnApproval|Booleano | Indica se os revisores são necessários para fornecer justificativa com sua decisão. O valor padrão é `false`. |
| defaultDecisionEnabled|Booleano | Indica se a decisão padrão está habilitada ou desabilitada quando os revisores não respondem. O valor padrão é `false`. |
| defaultDecision|Cadeia de Caracteres | Decisão escolhida se **defaultDecisionEnabled** for `true`. Pode ser um de `Approve`, `Deny`ou `Recommendation`. |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão (**accessReviewInstance**) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto de recorrência padrão do Outlook.  <br/><br/>**Nota:** Somente **as propriedades dayOfMonth**, **interval** e **type** (`weekly`, `absoluteMonthly`) têm suporte. Use a propriedade **startDate** **em recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Boolean | Indica se as decisões são aplicadas automaticamente. Quando definido como `false`, um administrador deve aplicar as decisões manualmente depois que o revisores concluir a revisão de acesso. Quando definido como `true`, as decisões são aplicadas automaticamente após o término da duração da instância de revisão de acesso, independentemente de os revisores responderem ou não. O valor padrão é `false`. |
| applyActions|[coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a serem tomadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction`. O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction`. |
| recommendationsEnabled|Booleano | Indica se as recomendações de decisão estão habilitadas ou desabilitadas. |

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
