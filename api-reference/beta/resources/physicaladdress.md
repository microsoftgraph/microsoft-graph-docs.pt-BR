---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 53b1e18bd1e7b78e7afb479cac3c5f6cc7ecff88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521873"
---
# <a name="physicaladdress-resource-type"></a>Tipo de recurso physicalAddress

Namespace: Microsoft. Graph

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
