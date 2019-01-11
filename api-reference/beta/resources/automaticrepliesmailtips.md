---
title: tipo de recurso de automaticRepliesMailTips
description: Dicas de email sobre qualquer respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
ms.openlocfilehash: 80ecaaa9fced0bcb00494b0414a86f0a11fd8996
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833226"
---
# <a name="automaticrepliesmailtips-resource-type"></a>tipo de recurso de automaticRepliesMailTips

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

[Dicas de email](../resources/mailtips.md) sobre qualquer respostas automáticas que foram configurados em uma caixa de correio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-----|:-----|:-----|
| mensagem | String | A mensagem de resposta automática. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | O idioma em que a mensagem de resposta automática está em. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e hora em que as respostas automáticas estão definidas para encerrar. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e hora em que as respostas automáticas estão definidas para começar. |

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
