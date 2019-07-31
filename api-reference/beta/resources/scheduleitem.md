---
title: tipo de recurso scheduleItem
description: Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário. Esse item também se aplica a um recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008639"
---
# <a name="scheduleitem-resource-type"></a>tipo de recurso scheduleItem

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário. Este item se aplica a um recurso (sala ou equipamento) também.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |A data, a hora e o fuso horário em que o evento correspondente termina. |
|IsPrivate |Booliano |A sensibilidade do evento correspondente. True se o evento estiver marcado `private`; caso contrário, false. Opcional. |
|location |String | O local onde o evento correspondente é mantido ou participado. Opcional.|
|iniciar |[dateTimeTimeZone](datetimetimezone.md) |A data, a hora e o fuso horário em que o evento correspondente é iniciado. |
|status |freeBusyStatus | O status de disponibilidade do usuário ou recurso durante o evento correspondente. Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | A linha de assunto do evento correspondente. Opcional.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
