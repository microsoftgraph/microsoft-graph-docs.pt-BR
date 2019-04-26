---
title: tipo de recurso networkLocationDetail
description: Indica detalhes associados ao local de rede. .
localization_priority: Normal
ms.openlocfilehash: c4a5323099258d9670b970b1bb85bd0d01f3cf8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342174"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="a8117-104">tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="a8117-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="a8117-105">Indica detalhes associados ao local de rede.</span><span class="sxs-lookup"><span data-stu-id="a8117-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="a8117-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8117-106">Properties</span></span>
| <span data-ttu-id="a8117-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8117-107">Property</span></span>     | <span data-ttu-id="a8117-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8117-108">Type</span></span>   |<span data-ttu-id="a8117-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8117-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8117-110">NetworkType</span><span class="sxs-lookup"><span data-stu-id="a8117-110">networkType</span></span>|<span data-ttu-id="a8117-111">NetworkType</span><span class="sxs-lookup"><span data-stu-id="a8117-111">networkType</span></span>|<span data-ttu-id="a8117-112">Fornece o tipo da rede.</span><span class="sxs-lookup"><span data-stu-id="a8117-112">Provides the type of the network.</span></span> <span data-ttu-id="a8117-113">Os valores possíveis são `intranet`: `extranet` `namedNetwork`,, e `trusted`.</span><span class="sxs-lookup"><span data-stu-id="a8117-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="a8117-114">networknames</span><span class="sxs-lookup"><span data-stu-id="a8117-114">networkNames</span></span>|<span data-ttu-id="a8117-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a8117-115">String collection</span></span>|<span data-ttu-id="a8117-116">Nomes da rede.</span><span class="sxs-lookup"><span data-stu-id="a8117-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a8117-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8117-117">JSON representation</span></span>

<span data-ttu-id="a8117-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8117-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail"
}-->

```json
{
  "networkType": "string",
  "networkNames": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
