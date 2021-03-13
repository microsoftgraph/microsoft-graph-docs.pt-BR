---
title: Tipo de recurso iPv4CidrRange
description: Representa um intervalo IPv4 usando a notação CIDR.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6251c06678c811a4553cdc28a76422d75d494284
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760711"
---
# <a name="ipv4cidrrange-resource-type"></a>Tipo de recurso iPv4CidrRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um intervalo IPv4 usando a notação CIDR.

Herda de [ipRange](../resources/iprange.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|cidrAddress|String|Endereço IPv4 na notação CIDR|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv4CidrRange",
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
  "description": "iPv4CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

