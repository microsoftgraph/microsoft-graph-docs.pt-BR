---
title: tipo de recurso de automaticRepliesMailTips
description: Dicas de email sobre qualquer respostas automáticas que foram configuradas em uma caixa de correio.
ms.openlocfilehash: 51657578474710d40cfc3feabdf41e50e7105942
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040888"
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