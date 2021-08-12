---
title: Tipo de recurso physicalOfficeAddress
description: Representa o endereço comercial de um recurso, como um contato ou evento.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f632fab8d5859a72eff551bba35184face6e3869255687ad9758decf3b131d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243305"
---
# <a name="physicalofficeaddress-resource-type"></a>Tipo de recurso physicalOfficeAddress

Namespace: microsoft.graph

Representa o endereço comercial de um recurso, como um contato organizacional.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String|A cidade.|
|countryOrRegion|String|O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".|
|officeLocation  | String | Office local, como construção e número de escritório para um contato organizacional.  |
|postalCode|Cadeia de caracteres|O código de endereçamento postal, ou CEP.|
|state|Cadeia de caracteres|O estado.|
|street|Cadeia de caracteres|O tipo de logradouro (rua, alameda, avenida, etc.).|

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

