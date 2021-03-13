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
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="613a6-103">Tipo de recurso iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="613a6-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="613a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="613a6-105">Representa um intervalo IPv4 usando a notação CIDR.</span><span class="sxs-lookup"><span data-stu-id="613a6-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="613a6-106">Herda de [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="613a6-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="613a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="613a6-107">Properties</span></span>

| <span data-ttu-id="613a6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="613a6-108">Property</span></span>     | <span data-ttu-id="613a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="613a6-109">Type</span></span>        | <span data-ttu-id="613a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="613a6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="613a6-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="613a6-111">cidrAddress</span></span>|<span data-ttu-id="613a6-112">String</span><span class="sxs-lookup"><span data-stu-id="613a6-112">String</span></span>|<span data-ttu-id="613a6-113">Endereço IPv4 na notação CIDR</span><span class="sxs-lookup"><span data-stu-id="613a6-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="613a6-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="613a6-114">JSON representation</span></span>

<span data-ttu-id="613a6-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="613a6-115">The following is a JSON representation of the resource.</span></span>

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

