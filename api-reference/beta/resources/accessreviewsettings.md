---
title: Tipo de recurso accessReviewSettings
description: Fornece configurações adicionais ao criar uma revisão de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdc8d22639d098619ef7183ebe22fc9da7bc0287
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293082"
---
# <a name="accessreviewsettings-resource-type"></a>Tipo de recurso accessReviewSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Fornece configurações adicionais ao criar uma revisão de acesso, para controlar o comportamento do recurso ao iniciar uma revisão de acesso.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Booliano | Indica se o envio de emails aos revisadores e ao criador da crítica está habilitado. |
| remindersEnabled | Booliano | Indica se o envio de emails de lembrete para revisadores está habilitado. |
| justificationRequiredOnApproval | Booliano | Indica se os revisadores devem fornecer uma justificativa ao revisar o acesso. |
| activityDurationInDays | Int64 | O número de dias de atividades do usuário para mostrar aos revisadores. |
| autoReviewEnabled | Booliano | Indica se uma decisão deve ser definida se o revistor não forneceu uma. Para uso quando a aplicação automática estiver habilitada. Se você não quiser ter uma decisão de revisão registrada, a menos que o revistor faça uma escolha explícita, de definida como `false` .|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | Configurações detalhadas sobre como o recurso deve definir a decisão de revisão. Para uso quando a aplicação automática estiver habilitada. |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | Configurações detalhadas de recorrência. |
| autoApplyReviewResultsEnabled | Booliano | Indica se a funcionalidade de aplicação automática, para alterar automaticamente o recurso de acesso ao objeto de destino, está habilitada.  Se não estiver habilitado, um usuário deverá, após a conclusão da revisão, aplicar a revisão de acesso. |
| accessRecommendationsEnabled | Booliano | Indica se a exibição de recomendações para revisadores está habilitada. |

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
