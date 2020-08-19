---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: af6f91233fde070888a4f7d74e277232c34fd64a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808351"
---
# <a name="attendeebase-resource-type"></a>Tipo de recurso attendeeBase

Namespace: microsoft.graph

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
|type|articipantetype| O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.|
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
