---
title: Tipo de recurso staffAvailabilityItem
description: Representa os intervalos de tempo disponíveis e ocupados de um membro da equipe do Bookings.
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2737d50eb65d0cdf4d0e44f3df76038968399f93
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856420"
---
# <a name="staffavailabilityitem-resource-type"></a>Tipo de recurso staffAvailabilityItem

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os intervalos de tempo disponíveis e ocupados de um Microsoft Bookings [da equipe](bookingstaffmember.md).

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
  "availabilityItems": [{"@odata.type": "microsoft.graph.availabilityItem"}],
  "staffId": "String"
}
```