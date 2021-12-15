---
title: Tipo de recurso bookingCustomerBase
description: Tipo de base abstrata para clientes do Bookings.
author: davisjms
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3eca954718608223977018b82f005001be269ba9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524996"
---
# <a name="bookingcustomerbase-resource-type"></a>Tipo de recurso bookingCustomerBase

Namespace: microsoft.graph

Tipo de base abstrata para clientes do Bookings.

Tipo base [de bookingCustomer](bookingcustomer.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do cliente. Herdado da [entidade](../resources/entity.md).|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomerBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomerBase",
  "id": "String (identifier)"
}
```

