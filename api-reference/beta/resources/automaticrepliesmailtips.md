---
title: Tipo de recurso automaticRepliesMailTips
description: Dicas de Email sobre as respostas automáticas que foram configuradas em uma caixa de correio.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: abheek-das
ms.openlocfilehash: 48051faa398fcbaf6e894ca2d67b394950c27522
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944966"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Tipo de recurso automaticRepliesMailTips

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Dicas de Email](../resources/mailtips.md) sobre as respostas automáticas que foram configuradas em uma caixa de correio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-----|:-----|:-----|
| mensagem | String | A mensagem de resposta automática. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | O idioma em que a mensagem de resposta automática está. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas são definidas como terminadas. |
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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


