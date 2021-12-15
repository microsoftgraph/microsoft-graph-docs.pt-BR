---
title: Tipo de recurso bookingStaffMemberBase
description: Tipo de base abstrata para membros da equipe do Bookings.
author: davisjms
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 17d13e80cf61e1cc885b07666708c9f8f479a385
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526444"
---
# <a name="bookingstaffmemberbase-resource-type"></a>Tipo de recurso bookingStaffMemberBase

Namespace: microsoft.graph

Tipo de base abstrata para membros da equipe do Bookings.

Tipo base [de bookingStaffMember](bookingstaffmember.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID do membro da equipe. Herdado da [entidade](../resources/entity.md).|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingStaffMemberBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingStaffMemberBase",
  "id": "String (identifier)"
}
```

