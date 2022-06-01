---
title: Tipo de recurso accessReviewSettings (preterido)
description: Fornece configurações adicionais ao criar uma revisão de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f197ca69132252a58508aa57b2c192eaae34077f
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821201"
---
# <a name="accessreviewsettings-resource-type-deprecated"></a>Tipo de recurso accessReviewSettings (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Fornece configurações adicionais ao criar uma revisão de acesso para controlar o comportamento do recurso ao iniciar uma revisão de acesso.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Boolean | Indica se o envio de emails para revisores e o criador da revisão está habilitado. |
| remindersEnabled | Booliano | Indica se o envio de emails de lembrete para revisores está habilitado. |
| justificationRequiredOnApproval | Boolean | Indica se os revisores devem fornecer uma justificativa ao revisar o acesso. |
| activityDurationInDays | Int64 | O número de dias de atividades do usuário a serem mostradas aos revisores. |
| autoReviewEnabled | Booliano | Indica se uma decisão deve ser definida se o revistor não forneceu uma. Para uso quando a aplicação automática estiver habilitada. Se você não quiser ter uma decisão de revisão registrada, a menos que o revisores faça uma escolha explícita, defina-a como `false`.|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | Configurações detalhadas de como o recurso deve definir a decisão de revisão. Para uso quando a aplicação automática estiver habilitada. |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | Configurações detalhadas para recorrência. |
| autoApplyReviewResultsEnabled | Boolean | Indica se a funcionalidade de aplicação automática, para alterar automaticamente o recurso de acesso ao objeto de destino, está habilitada.  Se não estiver habilitado, um usuário deverá, após a conclusão da revisão, aplicar a revisão de acesso. |
| accessRecommendationsEnabled | Booliano | Indica se a exibição de recomendações para revisores está habilitada. |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
```json
{
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,  
  "justificationRequiredOnApproval": true,
  "activityDurationInDays": 1024,
  "autoReviewEnabled": false,
  "autoReviewSettings": {"@odata.type": "microsoft.graph.autoReviewSettings"},
  "recurrenceSettings": {"@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"},
  "autoApplyReviewResultsEnabled": false,
  "accessRecommendationsEnabled": false
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
