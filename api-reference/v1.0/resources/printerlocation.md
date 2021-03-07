---
title: Tipo de recurso printerLocation
description: Representa o local físico e hierárquico de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f357ab3b33182ac6ffb2f8ae705a359a0e955eed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516831"
---
# <a name="printerlocation-resource-type"></a>Tipo de recurso printerLocation

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa o local físico e hierárquico de uma impressora.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|latitude|Double|A latitude em que a impressora está localizada.|
|longitude|Double|A longitude em que a impressora está localizada.|
|altitudeInMeters|Int32|A altitude, em metros, em que a impressora está localizada.|
|streetAddress|String|O endereço de rua onde a impressora está localizada.|
|subUnit|Coleção de cadeias de caracteres|A hierarquia de subunidades onde a impressora está localizada. Os elementos devem estar em ordem hierárquica. Por exemplo, se um campus for dividido em seções diferentes, a hierarquia poderá ter esta aparência: `["East Wing", "Block A"]`|
|city|Cadeia de caracteres|A cidade em que a impressora está localizada.|
|postalCode|Cadeia de caracteres|O código postal em que a impressora está localizada.|
|countryOrRegion|String|O país ou a região em que a impressora está localizada.|
|site|Cadeia de caracteres|O site em que a impressora está localizada.|
|building|Cadeia de caracteres|O edifício em que a impressora está localizada.|
|base|Cadeia de caracteres|O piso no que a impressora está localizada. Somente valores numéricos são suportados no momento.|
|floorDescription|Cadeia de caracteres|A descrição do piso em que a impressora está localizada.|
|roomName|Cadeia de caracteres|A sala em que a impressora está localizada. Somente valores numéricos são suportados no momento.|
|roomDescription|Cadeia de caracteres|A descrição da sala em que a impressora está localizada.|
|organização|Coleção de cadeias de caracteres|A hierarquia organizacional à que a impressora pertence. Os elementos devem estar em ordem hierárquica.|
|subdivisão|Coleção de cadeias de caracteres|A subdivisão em que a impressora está localizada. Os elementos devem estar em ordem hierárquica.|
|stateOrProvince|Cadeia de caracteres|O estado ou província em que a impressora está localizada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Double",
  "longitude": "Double",
  "altitudeInMeters": "Integer",
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floor": "String",
  "floorDescription": "String",
  "roomName": "String",
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```

