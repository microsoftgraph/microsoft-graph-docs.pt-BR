---
title: Tipo de recurso ipRange
description: Classe base de intervalo IP para representar intervalos de endereçoS IPV4 e IPV6.
ms.localizationpriority: medium
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b0bb1aba5e0a8f26e12aa8d8f1e273dd58617f68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089379"
---
# <a name="iprange-resource-type"></a>Tipo de recurso ipRange

Namespace: microsoft.graph

Um tipo abstrato de intervalo IP do qual os tipos de recursos [iPv4CidrRange](ipv4cidrrange.md) e [iPv6CidrRange](ipv6cidrrange.md) para configurar objetos [ipNamedLocation](ipnamedlocation.md) são derivados.

O tipo derivado [iPv4CidrRange](ipv4cidrrange.md) é usado para configurar intervalos de endereços IPv4 enquanto o tipo derivado [iPv6CidrRange](ipv6cidrrange.md) é usado para configurar intervalos de endereços IPv6.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipRange"
}-->

```json
{
    "@odata.type": "#microsoft.graph.ipRange"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

