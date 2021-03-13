---
title: Tipo de recurso iPv6CidrRange
description: Representa um intervalo IPv6 usando a notação CIDR.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4a3d3419b786ec1b6186b1eef5403145fcef8ceb
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761167"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="df867-103">Tipo de recurso iPv6CidrRange</span><span class="sxs-lookup"><span data-stu-id="df867-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="df867-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df867-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df867-105">Representa um intervalo IPv6 usando a notação CIDR.</span><span class="sxs-lookup"><span data-stu-id="df867-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="df867-106">Herda de [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="df867-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df867-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df867-107">Properties</span></span>

| <span data-ttu-id="df867-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df867-108">Property</span></span>     | <span data-ttu-id="df867-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df867-109">Type</span></span>        | <span data-ttu-id="df867-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df867-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df867-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="df867-111">cidrAddress</span></span>|<span data-ttu-id="df867-112">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="df867-112">String</span></span>|<span data-ttu-id="df867-113">Endereço IPv6 na notação CIDR</span><span class="sxs-lookup"><span data-stu-id="df867-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df867-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df867-114">JSON representation</span></span>

<span data-ttu-id="df867-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df867-115">The following is a JSON representation of the resource.</span></span>

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

