---
title: Tipo de recurso scheduleItem
description: Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário. Este item também se aplica a um recurso (sala ou equipamento).
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86dc2c44f93635bd38363984d7dda8debe21147f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035966"
---
# <a name="scheduleitem-resource-type"></a>Tipo de recurso scheduleItem

Namespace: microsoft.graph

Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário. Este item também se aplica a um recurso (sala ou equipamento).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |A data, hora e fuso horário que o evento correspondente termina. |
|isPrivate |Booliano |A sensibilidade do evento correspondente. True se o evento for marcado `private` , false caso contrário. Opcional.|
|location |Cadeia de caracteres | O local do qual o evento correspondente é realizado ou atendido. Opcional.|
|iniciar |[dateTimeTimeZone](datetimetimezone.md) |A data, a hora e o fuso horário que o evento correspondente inicia. |
|status |freeBusyStatus | O status de disponibilidade do usuário ou recurso durante o evento correspondente. Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|assunto |Cadeia de caracteres | A linha de assunto do evento correspondente. Opcional.|


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
  "tocPath": ""
}
-->

