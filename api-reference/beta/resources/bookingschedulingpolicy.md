---
title: Tipo de recurso bookingSchedulingPolicy
description: Representa o conjunto de políticas que determinam como os compromissos devem ser criados em um calendário do Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c6244c573fb60e13a5419ad89cee407dfd3a497b
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526139"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Tipo de recurso bookingSchedulingPolicy

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa o conjunto de políticas que determinam como os compromissos devem ser criados em um calendário do Microsoft Bookings.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowStaffSelection|Booliano|True se permitir que os clientes escolham uma pessoa específica para a reserva.|
|maximumAdvance|Duração|Número máximo de dias de antecedência que uma reserva pode ser feita. Ele segue o formato [ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|minimumLeadTime|Duração|O tempo mínimo antes do qual as reservas e cancelamentos devem ser feitos. Ele segue o formato [ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|sendConfirmationsToOwner|Booliano| True para notificar a empresa por email quando uma reserva for criada ou alterada. Use o endereço de email especificado na propriedade **de email** da **entidade bookingBusiness** para a empresa. |
|timeSlotInterval|Duração|Duração de cada intervalo de tempo, denotado no [formato ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


