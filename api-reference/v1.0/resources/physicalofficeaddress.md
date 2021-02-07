---
title: Tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou evento.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6ba8e82f1ba8641a0b1966586744ffd4721b9b81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135713"
---
# <a name="physicalofficeaddress-resource-type"></a>Tipo de recurso physicalOfficeAddress

Namespace: microsoft.graph

Representa o endereço comercial de um recurso, como um contato organizacional.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String|A cidade.|
|countryOrRegion|String|O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".|
|officeLocation  | String | Local do escritório, como prédio e número de escritório para um contato organizacional.  |
|postalCode|String|O código de endereçamento postal, ou CEP.|
|estado|String|O estado.|
|street|String|O tipo de logradouro (rua, alameda, avenida, etc.).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

