---
title: Tipo de recurso bookingReminder
description: Representa quando e quem enviar um lembrete de email.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: e17a8da313c3e445a4af4fb2369d67cb7b11365c
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526445"
---
# <a name="bookingreminder-resource-type"></a>Tipo de recurso bookingReminder

Namespace: microsoft.graph

Representa quando e quem enviar um lembrete de email.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|mensagem|String|A mensagem no lembrete.|
|offset|Duração|A quantidade de tempo antes do início de um compromisso que o lembrete deve ser enviado. Ele é denotado no formato [ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|destinatários|bookingReminderRecipients|As pessoas que devem receber o lembrete. Os valores possíveis são: `allAttendees`, `staff`, `customer`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": {"@odata.type": "microsoft.graph.bookingReminderRecipients"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


