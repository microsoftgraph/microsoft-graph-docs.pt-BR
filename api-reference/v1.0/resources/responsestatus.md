---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e1b2861386fc32589d35d6354345b1ba24471d98
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108867"
---
# <a name="responsestatus-resource-type"></a>Tipo de recurso responseStatus

Namespace: microsoft.graph

O status de resposta de um participante ou organizador de uma solicitação de reunião.

Você pode obter o status de resposta de um participante [](event.md) ou organizador por meio da propriedade **responseStatus** de um evento ou da propriedade **status** de [um participante](attendee.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo           | Descrição |
|:---------|:---------------|:------------|
| response | responseType   | O tipo de resposta. Os valores possíveis são: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.<br><br>Para diferenciar entre e : como exemplo, se o participante Alex não tiver respondido a uma solicitação de reunião, obter o status de resposta de Alex para esse evento no calendário de `none` `notResponded` Alex retornará `notResponded` . Obter a resposta de Alex do calendário de qualquer outro participante ou os retornos do organizador `none` . Obter a resposta do organizador para o evento no calendário de qualquer pessoa também retorna `none` . 
| time     | DateTimeOffset | A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`

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

