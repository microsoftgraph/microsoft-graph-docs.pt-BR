---
title: Tipo de recurso physicalAddress
description: Representa o endereço físico de um recurso, como um contato ou evento.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e5abc3dbeebb53935b1cdb77e8ef6038670c6b66e2e96658564957eb4fb24ba9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196569"
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
|state|Cadeia de caracteres|O estado.|
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

