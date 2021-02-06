---
title: Tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a login aconteceu.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: bc45d94896cbd822cdad4e3451f471bc3b540888
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134677"
---
# <a name="signinlocation-resource-type"></a>Tipo de recurso signInLocation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece a cidade, o estado e o país/região de onde a login aconteceu.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String|Fornece a cidade de origem do login. Isso é calculado usando informações de latitude/longitude da atividade de login.|
|countryOrRegion|String|Fornece as informações de código do país (código de 2 letras) onde a login se originou.  Isso é calculado usando informações de latitude/longitude da atividade de login.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Fornece a latitude, longitude e altitude de onde a login se originou.|
|estado|String|Fornece o estado de origem do login. Isso é calculado usando informações de latitude/longitude da atividade de login.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


