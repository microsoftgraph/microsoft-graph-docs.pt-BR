---
title: Tipo de recurso automaticRepliesMailTips
description: Dicas de Email sobre as respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cc7f65a526d4550182f1e6dc0c5ea25a12ee182
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135748"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Tipo de recurso automaticRepliesMailTips

Namespace: microsoft.graph


[Dicas de Email](../resources/mailtips.md) sobre as respostas automáticas que foram configuradas em uma caixa de correio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-----|:-----|:-----|
| mensagem | String | A mensagem de resposta automática. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | O idioma em que a mensagem de resposta automática está. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas são definidas para terminar. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas são definidas para começar. |

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

