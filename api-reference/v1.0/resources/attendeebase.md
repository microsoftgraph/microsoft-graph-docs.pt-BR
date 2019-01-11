---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878670"
---
# <a name="attendeebase-resource-type"></a>Tipo de recurso attendeeBase

O tipo de participante.

Derivado do [destinatário](recipient.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|type|attendeeType| O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Se o nome do participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera atualmente a pessoa é do `Required` tipo.|
|emailAddress|[emailAddress](emailaddress.md)|Inclui o nome e endereço SMTP do participante.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
