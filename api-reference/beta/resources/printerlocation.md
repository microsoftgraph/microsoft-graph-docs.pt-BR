---
title: tipo de recurso printerLocation
description: Representa o local físico e hierárquico de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfb082571ab1c5ddf2b46a06c6e66b9e31e47309
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664055"
---
# <a name="printerlocation-resource-type"></a>tipo de recurso printerLocation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o local físico e hierárquico de uma impressora.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|latitude|Double|O Latitude em que a impressora está localizada.|
|longitude|Double|A longitude em que a impressora está localizada.|
|altitudeInMeters|Int32|A altitude, em metros, em que a impressora está localizada em.|
|streetAddress|String|O endereço de rua onde a impressora está localizada.|
|subunidade|String collection|A hierarquia de subunidade onde a impressora está localizada. Os elementos devem estar em ordem hierárquica. Por exemplo, se um campus for dividido em seções diferentes, a hierarquia poderá ter a seguinte aparência: `["East Wing", "Block A"]`|
|city|String|A cidade na qual a impressora está localizada.|
|postalCode|String|O CEP em que a impressora está localizada.|
|countryOrRegion|String|O país ou a região em que a impressora está localizada.|
|site|String|O site no qual a impressora está localizada.|
|Build|String|O edifício em que a impressora está localizada.|
|base|String|O piso em que a impressora está localizada. Há suporte apenas para valores numéricos no momento.|
|floorDescription|String|A descrição do piso em que a impressora está localizada.|
|roomname|String|A sala na qual a impressora está localizada. Há suporte apenas para valores numéricos no momento.|
|roomDescription|String|A descrição da sala em que a impressora está localizada.|
|organization|String collection|A hierarquia organizacional à qual a impressora pertence. Os elementos devem estar em ordem hierárquica.|
|subdivisão|String collection|A subdivisão em que a impressora está localizada. Os elementos devem estar em ordem hierárquica.|
|stateOrProvince|String|O estado ou província em que a impressora está localizada.|

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

