---
title: tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35c6511b7dba69a362b44a9390974913c46b73ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034213"
---
# <a name="signinlocation-resource-type"></a>tipo de recurso signInLocation

Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String|Fornece a cidade onde a entrada se originou. Isso é calculado usando informações de latitude/longitude da atividade de entrada.|
|countryOrRegion|String|Fornece as informações do código do país (código de 2 letras) em que a entrada se originou.  Isso é calculado usando informações de latitude/longitude da atividade de entrada.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Fornece a latitude, longitude e altitude onde a entrada se originou.|
|state|String|Fornece o estado em que a entrada se originou. Isso é calculado usando informações de latitude/longitude da atividade de entrada.|

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
