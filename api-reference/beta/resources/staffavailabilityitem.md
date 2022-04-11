---
title: Tipo de recurso staffAvailabilityItem
description: Representa os intervalos de tempo disponíveis e ocupados de um Bookings da equipe.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5c130388ce2b728c22c467689b998ffe8673c718
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755723"
---
# <a name="staffavailabilityitem-resource-type"></a>Tipo de recurso staffAvailabilityItem

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os intervalos de tempo disponíveis e ocupados de um Bookings [da equipe](bookingstaffmember.md).

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo |Descrição|
|:---------------|:--------|:----------|
|availabilityItems |[coleção availabilityItem](availabilityitem.md) |Cada item nesta coleção indica um slot e o status do membro da equipe.|
|staffId |Cadeia de caracteres |A ID do membro da equipe.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.staffAvailabilityItem"
}-->

``` json
{
  "availabilityItems": "availabilityItem",
  "staffId": "String"
}
```
