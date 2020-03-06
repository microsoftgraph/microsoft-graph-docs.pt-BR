---
title: tipo de recurso automaticRepliesMailTips
description: Dicas de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7d7c5c6a3560435c4e61a8953887f5b6b61324
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532045"
---
# <a name="automaticrepliesmailtips-resource-type"></a>tipo de recurso automaticRepliesMailTips

Namespace: microsoft.graph


[Dicas](../resources/mailtips.md) de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-----|:-----|:-----|
| mensagem | String | A mensagem de resposta automática. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | O idioma em que a mensagem de resposta automática está. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas estão definidas para terminar. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas estão definidas para começar. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
