---
title: Tipo de recurso staffAvailabilityItem
description: Representa os intervalos de tempo disponíveis e ocupados de um Microsoft Bookings da equipe.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fa6a7e856060209f274c0503d3c0c27f567ae910
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917763"
---
# <a name="staffavailabilityitem-resource-type"></a>Tipo de recurso staffAvailabilityItem

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os intervalos de tempo disponíveis e ocupados de um Microsoft Bookings [da equipe](bookingstaffmember.md).

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo |Descrição|
|:---------------|:--------|:----------|
|availabilityItems |[coleção availabilityItem](availabilityitem.md) |Cada item nesta coleção indica um slot e o status do membro da equipe.|
|staffId |Cadeia de Caracteres |A ID do membro da equipe.|

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
