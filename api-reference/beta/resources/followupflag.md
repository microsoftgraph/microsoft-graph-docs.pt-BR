---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
ms.openlocfilehash: a996bc05e5297149e587d7372e989580146c1fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037343"
---
# <a name="followupflag-resource-type"></a>Tipo de recurso followupFlag

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem [message](message.md) e [contact](contact.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Data e hora em que o acompanhamento foi concluído.|
|dueDateTime|**dateTimeTimeZone**|Data e hora em que o acompanhamento deve ser concluído.|
|flagStatus|Cadeia de caracteres|O status de acompanhamento de um item. Os valores possíveis são: `notFlagged`, `complete` e `flagged`.|
|startDateTime|**dateTimeTimeZone**|Data e hora em que o acompanhamento deve começar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
