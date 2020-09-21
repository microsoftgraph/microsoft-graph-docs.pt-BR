---
title: tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 1bbfb01e07b5ccde134933490b06ae3ab1da53af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067136"
---
# <a name="signinlocation-resource-type"></a>tipo de recurso signInLocation

Namespace: o Microsoft. Graph fornece a cidade, o estado e o país/região de onde a entrada ocorreu.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|Cadeia de caracteres|Fornece a cidade onde a entrada se originou. Isso é calculado usando informações de latitude/longitude da atividade de entrada.|
|countryOrRegion|String|Fornece as informações do código do país (código de 2 letras) em que a entrada se originou.  Isso é calculado usando informações de latitude/longitude da atividade de entrada.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Fornece a latitude, longitude e altitude onde a entrada se originou.|
|state|Cadeia de caracteres|Fornece o estado em que a entrada se originou. Isso é calculado usando informações de latitude/longitude da atividade de entrada.|

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


