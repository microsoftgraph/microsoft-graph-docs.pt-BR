---
title: Tipo de recurso accessReviewScheduleSettings
description: Representa as configurações associadas a uma série de revisão de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fa090e7e51a9df31ce5a988fc6f79167e106b800
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084703"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

O **accessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| mailNotificationsEnabled|Booliano | Indica se os emails estão habilitados ou desabilitados. O valor padrão é `false`.               |
| reminderNotificationsEnabled|Boolean  | Indica se os lembretes estão habilitados ou desabilitados. O valor padrão é `false`.  |
| justificationRequiredOnApproval|Booliano | Indica se os revisadores são necessários para fornecer justificativa com sua decisão. O valor padrão é `false`. |
| defaultDecisionEnabled|Booliano | Indica se a decisão padrão está habilitada ou desabilitada quando os revisadores não respondem. O valor padrão é `false`. |
| defaultDecision|String | Decisão escolhida se **defaultDecisionEnabled** for `true` . Pode ser um `Approve` dos `Deny` , ou `Recommendation` . |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão (**accessReviewInstance**) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. Somente `weekly` e `absoluteMonthly` em **recorrênciaPattern** são suportados. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. |
| autoApplyDecisionsEnabled|Boolean | Indica se as decisões são aplicadas automaticamente. Quando definido como , um usuário deve aplicar as decisões manualmente depois que o `false` revistor concluir a revisão de acesso. Quando definido como , as decisões são aplicadas automaticamente após o fim da duração da instância de revisão de acesso, se os `true` revisadores responderam ou não. O valor padrão é `false`. |
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
