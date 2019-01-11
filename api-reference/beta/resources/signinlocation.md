---
title: tipo de recurso de signInLocation
description: Fornece a cidade, estado e país/região de onde a entrar aconteceu.
localization_priority: Normal
ms.openlocfilehash: 49d6dfb07c635ac3754b3e873d75911a43593a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839134"
---
# <a name="signinlocation-resource-type"></a>tipo de recurso de signInLocation
Fornece a cidade, estado e país/região de onde a entrar aconteceu.



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|Cadeia de caracteres|Fornece a cidade onde o sign-in se originou. Isso é calculado usando informações de latitude/longitude da atividade de entrada.|
|countryOrRegion|Cadeia de caracteres|Fornece as informações de código de país (código de carta 2) onde o sign-in se originou.  Isso é calculado usando informações de latitude/longitude da atividade de entrada.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Fornece o latitude, longitude e altitude onde a entrar se originou.|
|estado|Cadeia de caracteres|Fornece o estado em que a entrada se originou. Isso é calculado usando informações de latitude/longitude da atividade de entrada.|

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
