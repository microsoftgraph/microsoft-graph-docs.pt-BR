---
title: Tipo de recurso attendee
description: Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a518a39aa507173f0190a14bc947e11c3f7a90ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067553"
---
# <a name="attendee-resource-type"></a>Tipo de recurso attendee

Namespace: microsoft.graph

Um participante do evento. Pode ser uma pessoa ou recurso, como uma sala de reunião ou equipamento, que seja configurado como um recurso no Exchange Server para o locatário.

Derivado de [attendeeBase](attendeebase.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|emailAddress|[emailAddress](emailaddress.md)|Inclui o nome e endereço SMTP do participante.|
|proposedNewTime|[timeSlot](timeslot.md)|Uma data/hora alternativa proposta pelo participante para que uma solicitação de reunião seja inicial e final. Se o participante não tiver proposto outra hora, essa propriedade não será incluída em uma resposta de um evento GET.|
|status|[ResponseStatus](responsestatus.md)|A resposta do participante (nenhum, aceito, recusado, etc.) para o evento e a data e a hora em que a resposta foi enviada.|
|tipo|Cadeia de caracteres|O tipo de participante: `required`, `optional` ou `resource`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [
   "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

