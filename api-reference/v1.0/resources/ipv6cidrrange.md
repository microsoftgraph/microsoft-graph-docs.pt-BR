---
title: Tipo de recurso iPv6CidrRange
description: Representa um intervalo IPv6 usando a notação CIDR.
localization_priority: Normal
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a8afeeed483b3610c5c1dde1afee5f4a24317ff4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760859"
---
# <a name="ipv6cidrrange-resource-type"></a>Tipo de recurso iPv6CidrRange

Namespace: microsoft.graph

Representa um intervalo IPv6 usando a notação CIDR.

Herda de [ipRange](../resources/iprange.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|cidrAddress|String|Endereço IPv6 na notação CIDR|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv6CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv6CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
