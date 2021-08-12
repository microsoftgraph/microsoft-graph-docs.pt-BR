---
title: Tipo de recurso signInLocation
description: Fornece a cidade, o estado e o país/região de onde a login aconteceu.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fb22cf430ec3bffd04150398600beae5af4c41579f00f3cf49196587efb9f44b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124154"
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
|state|Cadeia de caracteres|Fornece o Estado de origem do sign-in. Isso é calculado usando informações de latitude/longitude da atividade de login.|

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

