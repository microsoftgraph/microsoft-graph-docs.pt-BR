---
title: tipo de recurso iPv4CidrRange
description: Representa um intervalo IPv4 usando a notação CIDR.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 169be1976c57dc76ff85b5eaff5620b3938479d8
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384455"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="98cf5-103">tipo de recurso iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="98cf5-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="98cf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98cf5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98cf5-105">Representa um intervalo IPv4 usando a notação CIDR.</span><span class="sxs-lookup"><span data-stu-id="98cf5-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="98cf5-106">Herda de [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="98cf5-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98cf5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98cf5-107">Properties</span></span>

| <span data-ttu-id="98cf5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98cf5-108">Property</span></span>     | <span data-ttu-id="98cf5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="98cf5-109">Type</span></span>        | <span data-ttu-id="98cf5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="98cf5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98cf5-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="98cf5-111">cidrAddress</span></span>|<span data-ttu-id="98cf5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98cf5-112">String</span></span>|<span data-ttu-id="98cf5-113">Endereço IPv4 em notação CIDR</span><span class="sxs-lookup"><span data-stu-id="98cf5-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98cf5-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98cf5-114">JSON representation</span></span>

<span data-ttu-id="98cf5-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98cf5-115">The following is a JSON representation of the resource.</span></span>

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