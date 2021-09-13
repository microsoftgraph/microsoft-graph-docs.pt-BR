---
title: Tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a login aconteceu.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 826daa833829b8ca9da9f4844827b308c8843044
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139594"
---
# <a name="signinlocation-resource-type"></a>Tipo de recurso signInLocation

Namespace: microsoft.graph

Fornece a cidade, o estado e o país/região de onde a login aconteceu.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|Cadeia de caracteres|Fornece a cidade de origem do login. Isso é calculado usando informações de latitude/longitude da atividade de login.|
|countryOrRegion|String|Fornece as informações do código do país (código de 2 letras) de onde a assinatura se originou.  Isso é calculado usando informações de latitude/longitude da atividade de login.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Fornece a latitude, longitude e altitude de onde o login se originou.|
|state|String|Fornece o Estado de origem do sign-in. Isso é calculado usando informações de latitude/longitude da atividade de login.|

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

