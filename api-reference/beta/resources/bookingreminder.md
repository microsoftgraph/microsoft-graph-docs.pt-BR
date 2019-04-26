---
title: tipo de recurso bookingReminder
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 18265a9d9e86b79706b6a268df3b8512b7b65111
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328195"
---
# <a name="bookingreminder-resource-type"></a>tipo de recurso bookingReminder

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa quando e para quem enviar um lembrete de email.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|mensagem|String|A mensagem no lembrete.|
|partida|Duração|O período de tempo antes do início de um compromisso para o qual o lembrete deve ser enviado. Ele é indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|destinatários|String| As pessoas que shouold receberão o lembrete. Os valores possíveis são: `allAttendees`, `staff`, `customer`.|

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
  "recipients": "String"
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
