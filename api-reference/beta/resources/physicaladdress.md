---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d6081f21069cef6014c8a028898f11ea9a3f4f3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344967"
---
# <a name="physicaladdress-resource-type"></a>Tipo de recurso physicalAddress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o endereço físico de um recurso, como um contato ou evento.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String|A cidade.|
|countryOrRegion|String|O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".|
|postalCode|String|O código de endereçamento postal, ou CEP.|
|postOfficeBox|String|O número da caixa postal.|
|state|Cadeia de caracteres|O estado.|
|street|String|O tipo de logradouro (rua, alameda, avenida, etc.).|
|type|physicalAddressType|O tipo de endereço. Os valores possíveis são: `unknown`, `home`, `business`, `other`.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
