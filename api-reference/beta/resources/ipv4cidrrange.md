---
title: tipo de recurso iPv4CidrRange
description: Representa um intervalo IPv4 usando a notação CIDR.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4864388492f3dedec4add271904f2e07a3e85419
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653822"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="bfe96-103">tipo de recurso iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="bfe96-103">iPv4CidrRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfe96-104">Representa um intervalo IPv4 usando a notação CIDR.</span><span class="sxs-lookup"><span data-stu-id="bfe96-104">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="bfe96-105">Herda de [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="bfe96-105">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bfe96-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfe96-106">Properties</span></span>

| <span data-ttu-id="bfe96-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfe96-107">Property</span></span>     | <span data-ttu-id="bfe96-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfe96-108">Type</span></span>        | <span data-ttu-id="bfe96-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe96-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bfe96-110">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="bfe96-110">cidrAddress</span></span>|<span data-ttu-id="bfe96-111">String</span><span class="sxs-lookup"><span data-stu-id="bfe96-111">String</span></span>|<span data-ttu-id="bfe96-112">Endereço IPv4 em notação CIDR</span><span class="sxs-lookup"><span data-stu-id="bfe96-112">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfe96-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfe96-113">JSON representation</span></span>

<span data-ttu-id="bfe96-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfe96-114">The following is a JSON representation of the resource.</span></span>

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