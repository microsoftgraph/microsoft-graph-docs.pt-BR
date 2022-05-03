---
title: Tipo de recurso printerLocation
description: Representa o local físico e hierárquico de uma impressora.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53eeee6e135276ff43e5cd360fbc6615d2df649f
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176606"
---
# <a name="printerlocation-resource-type"></a>Tipo de recurso printerLocation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o local físico e hierárquico de uma impressora.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|latitude|Double|A latitude em que a impressora está localizada.|
|longitude|Double|A longitude em que a impressora está localizada.|
|altitudeInMeters|Int32|A altitude, em metros, em que a impressora está localizada.|
|streetAddress|String|O endereço da rua onde a impressora está localizada.|
|Subunit|Conjunto de cadeias de caracteres|A hierarquia de subunidades em que a impressora está localizada. Os elementos devem estar em ordem hierárquica. Por exemplo, se um campus for dividido em seções diferentes, a hierarquia poderá ter esta aparência: `["East Wing", "Block A"]`|
|city|Cadeia de caracteres|A cidade em que a impressora está localizada.|
|postalCode|Cadeia de caracteres|O CÓDIGO POSTAL no qual a impressora está localizada.|
|countryOrRegion|String|O país ou região em que a impressora está localizada.|
|site|Cadeia de Caracteres|O site no qual a impressora está localizada.|
|Edifício|Cadeia de Caracteres|O prédio no qual a impressora está localizada.|
|base|Cadeia de Caracteres|O chão no qual a impressora está localizada. Somente valores numéricos têm suporte no momento.|
|floorDescription|Cadeia de Caracteres|A descrição do piso no qual a impressora está localizada.|
|roomName|Cadeia de Caracteres|A sala na qual a impressora está localizada. Somente valores numéricos têm suporte no momento.|
|roomDescription|Cadeia de Caracteres|A descrição da sala na qual a impressora está localizada.|
|organization|Coleção String|A hierarquia organizacional à qual a impressora pertence. Os elementos devem estar em ordem hierárquica.|
|Subdivisão|Conjunto de cadeias de caracteres|A subdivisão na qual a impressora está localizada. Os elementos devem estar em ordem hierárquica.|
|Stateorprovince|Cadeia de Caracteres|O estado ou província em que a impressora está localizada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerLocation"
}-->

```json
{
    "latitude": 80.1,
    "longitude": -170.1,
    "altitudeInMeters": 123456,
    "streetAddress": "String",
    "subUnit": ["String"],
    "city": "String",
    "postalCode": "String",
    "countryOrRegion": "String",
    "site": "String",
    "building": "String",
    "floor": "123456",
    "floorDescription": "String",
    "roomName": "123456",
    "roomDescription": "String",
    "organization": ["String"],
    "subdivision": ["String"],
    "stateOrProvince": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

