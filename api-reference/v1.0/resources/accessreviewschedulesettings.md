---
title: Tipo de recurso accessReviewScheduleSettings
description: Representa as configurações associadas a uma série de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77c566f959241ed88f44e43399bda58c29cfc3beb929c58564c2044a6875022e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218839"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| mailNotificationsEnabled|Booliano | Indica se os emails estão habilitados ou desabilitados. O valor padrão é `false`.               |
| reminderNotificationsEnabled|Booliano  | Indica se os lembretes estão habilitados ou desabilitados. O valor padrão é `false`.  |
| justificationRequiredOnApproval|Booliano | Indica se os revisadores são necessários para fornecer justificativa com sua decisão. O valor padrão é `false`. |
| defaultDecisionEnabled|Booliano | Indica se a decisão padrão está habilitada ou desabilitada quando os revisadores não respondem. O valor padrão é `false`. |
| defaultDecision|Cadeia de caracteres | Decisão escolhida se **defaultDecisionEnabled** for `true` . Pode ser um `Approve` dos `Deny` , ou `Recommendation` . |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão (**accessReviewInstance**) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. Somente `weekly` e `absoluteMonthly` em **recorrênciaPattern** são suportados. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Booliano | Indica se as decisões são aplicadas automaticamente. Quando definido como , um usuário deve aplicar as decisões manualmente depois que o `false` revistor concluir a revisão de acesso. Quando definido como , as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os `true` revisadores responderam ou não. O valor padrão é `false`. |
| applyActions|[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a ser realizadas depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` . O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` . Consulte [accessReviewApplyAction](accessreviewapplyaction.md). |
| recommendationsEnabled|Booliano | Indica se as recomendações de decisão estão habilitadas ou desabilitadas. |

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
