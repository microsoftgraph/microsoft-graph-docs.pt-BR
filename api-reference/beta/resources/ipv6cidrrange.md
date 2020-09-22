---
title: tipo de recurso iPv6CidrRange
description: Representa um intervalo IPv6 usando a notação CIDR.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 353c06222003893ccec787590d59f02b046d843d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075688"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="0a860-103">tipo de recurso iPv6CidrRange</span><span class="sxs-lookup"><span data-stu-id="0a860-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="0a860-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a860-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a860-105">Representa um intervalo IPv6 usando a notação CIDR.</span><span class="sxs-lookup"><span data-stu-id="0a860-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="0a860-106">Herda de [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0a860-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a860-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a860-107">Properties</span></span>

| <span data-ttu-id="0a860-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a860-108">Property</span></span>     | <span data-ttu-id="0a860-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a860-109">Type</span></span>        | <span data-ttu-id="0a860-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a860-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a860-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="0a860-111">cidrAddress</span></span>|<span data-ttu-id="0a860-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a860-112">String</span></span>|<span data-ttu-id="0a860-113">Endereço IPv6 na notação CIDR</span><span class="sxs-lookup"><span data-stu-id="0a860-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a860-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a860-114">JSON representation</span></span>

<span data-ttu-id="0a860-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a860-115">The following is a JSON representation of the resource.</span></span>

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

