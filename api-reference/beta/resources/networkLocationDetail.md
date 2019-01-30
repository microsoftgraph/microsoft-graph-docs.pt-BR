---
title: tipo de recurso de networkLocationDetail
description: Indica detalhes associadas ao local de rede. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643759"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="a7234-104">tipo de recurso de networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="a7234-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="a7234-105">Indica detalhes associadas ao local de rede.</span><span class="sxs-lookup"><span data-stu-id="a7234-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="a7234-106">.</span><span class="sxs-lookup"><span data-stu-id="a7234-106"></span></span>



## <a name="properties"></a><span data-ttu-id="a7234-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7234-107">Properties</span></span>
| <span data-ttu-id="a7234-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7234-108">Property</span></span>     | <span data-ttu-id="a7234-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7234-109">Type</span></span>   |<span data-ttu-id="a7234-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7234-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7234-111">networkType</span><span class="sxs-lookup"><span data-stu-id="a7234-111">networkType</span></span>|<span data-ttu-id="a7234-112">String</span><span class="sxs-lookup"><span data-stu-id="a7234-112">String</span></span>|<span data-ttu-id="a7234-113">Fornece o tipo da rede.</span><span class="sxs-lookup"><span data-stu-id="a7234-113">Provides the type of the network.</span></span> <span data-ttu-id="a7234-114">Os valores possíveis são `intranet`, `extranet`, `namedNetwork`, e `trusted`.</span><span class="sxs-lookup"><span data-stu-id="a7234-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="a7234-115">networkName</span><span class="sxs-lookup"><span data-stu-id="a7234-115">networkName</span></span>|<span data-ttu-id="a7234-116">String</span><span class="sxs-lookup"><span data-stu-id="a7234-116">String</span></span>|<span data-ttu-id="a7234-117">Nome da rede.</span><span class="sxs-lookup"><span data-stu-id="a7234-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a7234-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7234-118">JSON representation</span></span>

<span data-ttu-id="a7234-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7234-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
