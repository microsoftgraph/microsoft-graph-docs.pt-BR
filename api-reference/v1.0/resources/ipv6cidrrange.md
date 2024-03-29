---
title: Tipo de recurso iPv6CidrRange
description: Representa um intervalo IPv6 usando a notação CIDR.
ms.localizationpriority: medium
author: davidspooner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 545feee2df04be38c22853b96d19a81ef99d29ec
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162017"
---
# <a name="ipv6cidrrange-resource-type"></a>Tipo de recurso iPv6CidrRange

Namespace: microsoft.graph

Representa um intervalo IPv6 usando a notação CIDR (roteamento entre domínios sem classe).

Herda de [ipRange](../resources/iprange.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|cidrAddress|Cadeia de caracteres|Endereço IPv6 na notação CIDR. Não anulável.|

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
  "@odata.type": "#microsoft.graph.iPv6CidrRange", 
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
