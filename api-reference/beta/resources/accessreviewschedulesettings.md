---
title: Tipo de recurso accessReviewScheduleSettings
description: No recurso de revisões de acesso do Azure AD, as configurações associadas a `accessReviewScheduleSettings` uma série de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a58ba9a682e443efbc159befaea61b15e3fdc81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133440"
---
# <a name="accessreviewschedulesettings-resource-type"></a>Tipo de recurso accessReviewScheduleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AccessReviewScheduleSettings** define as configurações de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). 

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | Sinalizador para indicar se os emails estão habilitados/desabilitados.                |
| reminderNotificationsEnabled|Boolean  | Sinalizador para indicar se os lembretes estão habilitados/desabilitados.   |
| justificationRequiredOnApproval|Boolean | Sinalizador para indicar se os revisadores são obrigados a fornecer justificativa com sua decisão. |
| defaultDecisionEnabled|Boolean | Sinalizador para indicar se a decisão padrão está habilitada/desabilitada quando os revisadores não respondem. |
| defaultDecision|String | Decisão escolhida se `defaultDecisionEnabled` estiver habilitada. Pode ser "Aprovar", "Negar" ou "Recomendação". |
| instanceDurationInDays|Int32 | Duração de cada recorrência de revisão ( `accessReviewInstance` ) em número de dias. |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | Configurações detalhadas de recorrência. Usando o objeto de recorrência padrão do Outlook.  |
| autoApplyDecisionsEnabled|Boolean | Sinalizador para indicar se o recurso de aplicação automática está habilitado. |
| applyActions|[Coleção accessReviewApplyAction](../resources/accessreviewapplyaction.md) | Campo opcional. Descreve as ações a tomar depois que uma revisão é concluída. Há dois tipos com suporte no momento: `removeAccessApplyAction` (padrão) e `disableAndDeleteUserApplyAction` . O campo só precisa ser especificado no caso de `disableAndDeleteUserApplyAction` . Consulte [accessReviewApplyAction](accessreviewapplyaction.md). |
| recommendationsEnabled|Boolean | Sinalizador para indicar se as recomendações de decisão estão habilitadas/desabilitadas. |

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
