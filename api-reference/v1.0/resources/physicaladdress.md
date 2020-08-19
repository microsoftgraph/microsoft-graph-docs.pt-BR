---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e7729762a93e5185d45289b2377ecd961d894552
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808855"
---
# <a name="physicaladdress-resource-type"></a>Tipo de recurso physicalAddress

Namespace: microsoft.graph

Representa o endereço físico de um recurso, como um contato ou evento.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|Cadeia de caracteres|A cidade.|
|countryOrRegion|String|O país ou a região. É um valor de cadeia de caracteres de formato livre, por exemplo, "Brasil".|
|postalCode|Cadeia de caracteres|O código de endereçamento postal, ou CEP.|
|estado|Cadeia de caracteres|O estado.|
|street|Cadeia de caracteres|O tipo de logradouro (rua, alameda, avenida, etc.).|

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
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
