---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a7eaf030413e576721bd672fc63111a62742c163
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532073"
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
