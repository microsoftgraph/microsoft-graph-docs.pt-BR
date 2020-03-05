---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 532cf48f59b94fefe8aa1c25546c066db0126e85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446965"
---
# <a name="responsestatus-resource-type"></a>Tipo de recurso responseStatus

Namespace: Microsoft. Graph

O status de resposta de uma solicitação de reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo           | Descrição |
|:---------|:---------------|:------------|
| response | responseType   | O tipo de resposta. Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.
| time     | DateTimeOffset | A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
