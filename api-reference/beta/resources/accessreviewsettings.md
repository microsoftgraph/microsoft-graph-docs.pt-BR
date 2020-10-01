---
title: tipo de recurso accessReviewSettings
description: Fornece configurações adicionais ao criar uma revisão do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4de925ecb2fac65e3ab339ba8d4e602fcdc2af3
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330351"
---
# <a name="accessreviewsettings-resource-type"></a>tipo de recurso accessReviewSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações adicionais ao criar uma revisão do Access, para controlar o comportamento do recurso ao iniciar uma revisão do Access.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Booleano | Indica se o envio de emails para revisores e o criador de revisão está habilitado. |
| remindersEnabled | Booleano | Indica se o envio de emails de lembrete aos revisores está habilitado. |
| justificationRequiredOnApproval | Booleano | Indica se os revisores são necessários para fornecer uma justificativa ao revisar o acesso. |
| activityDurationInDays | Int64 | O número de dias de atividades do usuário para mostrar aos revisores. |
| autoReviewEnabled | Booleano | Indica se uma decisão deverá ser definida se o revisor não fornecer um. Para uso quando a aplicação automática está habilitada. Se você não quiser ter uma decisão de revisão registrada, a menos que o revisor faça uma escolha explícita, defina-a como `false` .|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | Configurações detalhadas de como o recurso deve definir a decisão de revisão. Para uso quando a aplicação automática está habilitada. |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | Definições detalhadas de recorrência. |
| autoApplyReviewResultsEnabled | Booleano | Indica se o recurso de aplicação automática, para alterar automaticamente o recurso de acesso ao objeto de destino, está habilitado.  Se não habilitado, um usuário deve, após a conclusão da revisão, aplicar a revisão do Access. |
| accessRecommendationsEnabled | Booleano | Indica se a exibição de recomendações para revisores está habilitada. |

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