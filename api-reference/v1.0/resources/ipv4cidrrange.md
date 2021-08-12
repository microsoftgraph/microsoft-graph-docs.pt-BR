---
title: Tipo de recurso iPv4CidrRange
description: Representa um intervalo IPv4 usando a notação CIDR.
localization_priority: Normal
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fcdbc795c67d40a34ab0a56f875b028a35b06d0a4d51276e199e4c07bed04a09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192275"
---
# <a name="ipv4cidrrange-resource-type"></a>Tipo de recurso iPv4CidrRange

Namespace: microsoft.graph

Representa um intervalo IPv4 usando a notação CIDR.

Herda de [ipRange](../resources/iprange.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|cidrAddress|Cadeia de caracteres|Endereço IPv4 na notação CIDR|

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
