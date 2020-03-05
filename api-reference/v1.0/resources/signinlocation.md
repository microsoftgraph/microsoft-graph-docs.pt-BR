---
title: tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a entrada ocorreu.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 58c3dc2b25b85963e6a0f6f88552dbf2a121d5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446853"
---
# <a name="signinlocation-resource-type"></a>tipo de recurso signInLocation

Namespace: Microsoft. Graph

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
