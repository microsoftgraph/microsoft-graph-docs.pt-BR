---
title: Tipo de recurso bookingPerson
description: Esse é um tipo base para uma pessoa em uma empresa do Microsoft Bookings, que pode ser um bookingCustomer ou bookingStaffMember.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 0ad4cd1d587fb2ccd88727f24944bc4226e43b7f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526181"
---
# <a name="bookingperson-resource-type"></a>Tipo de recurso bookingPerson

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Esse é um tipo base para uma pessoa em uma empresa do Microsoft Bookings, que pode ser [um bookingCustomer](bookingcustomer.md) ou [bookingStaffMember](bookingstaffmember.md).

Herda de [bookingNamedEntity](bookingnamedentity.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|Um nome para a entidade derivada, que faz interface com os clientes. Herdado **de bookingNamedEntity**.|
|emailAddress|String|O endereço de email da pessoa.|
|id|Cadeia de caracteres| A ID da entidade derivada. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


