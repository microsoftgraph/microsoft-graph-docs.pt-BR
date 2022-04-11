---
title: Tipo de recurso availabilityItem
description: Indica o status de um membro da equipe para um determinado intervalo de tempo.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2b51fe3644fc6ca884d1eb4435a6b874f2293fa2
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755727"
---
# <a name="availabilityitem-resource-type"></a>Tipo de recurso availabilityItem

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica o status de um membro [da equipe](bookingstaffmember.md) para um determinado intervalo de tempo.

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo |Descrição|
|:---------------|:--------|:----------|
|endDateTime |dateTimeTimeZone |A hora de término do intervalo de tempo.|
|serviceId |Cadeia de caracteres |Indica a ID do serviço no caso de compromissos 1:n. Se o compromisso for do tipo 1:n, este campo estará presente, caso contrário, `null`.|
|status |bookingsAvailabilityStatus |O status do membro da equipe. Os valores possíveis são: `available`, `busy`, `slotsAvailable`, `outOfOffice`, `unknownFutureValue`.|
|startDateTime |dateTimeTimeZone |A hora de início do intervalo de tempo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.availabilityItem"
}-->

``` json
{
  "endDateTime": "DateTimeInfo",
  "serviceId": "String",
  "status": "String",
  "startDateTime": "DateTimeInfo"
}
```
