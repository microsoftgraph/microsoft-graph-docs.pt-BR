---
title: Tipo de recurso iPv4CidrRange
description: Representa um intervalo IPv4 usando a notação CIDR.
ms.localizationpriority: medium
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b11286b1de310b4d95f6f323a7c0a94b468a75a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134749"
---
# <a name="ipv4cidrrange-resource-type"></a>Tipo de recurso iPv4CidrRange

Namespace: microsoft.graph

Representa um intervalo IPv4 usando a notação CIDR (roteamento entre domínios sem classe).

Herda de [ipRange](../resources/iprange.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|cidrAddress|String|Endereço IPv4 na notação CIDR. Não anulável.|

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
  "@odata.type": "#microsoft.graph.iPv4CidrRange",  
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
