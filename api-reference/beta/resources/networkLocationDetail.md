---
title: tipo de recurso networkLocationDetail
description: Indica detalhes associados ao local de rede. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581440"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="e2292-104">tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="e2292-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="e2292-105">Indica detalhes associados ao local de rede.</span><span class="sxs-lookup"><span data-stu-id="e2292-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="e2292-106">.</span><span class="sxs-lookup"><span data-stu-id="e2292-106"></span></span>



## <a name="properties"></a><span data-ttu-id="e2292-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2292-107">Properties</span></span>
| <span data-ttu-id="e2292-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2292-108">Property</span></span>     | <span data-ttu-id="e2292-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2292-109">Type</span></span>   |<span data-ttu-id="e2292-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2292-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2292-111">NetworkType</span><span class="sxs-lookup"><span data-stu-id="e2292-111">networkType</span></span>|<span data-ttu-id="e2292-112">String</span><span class="sxs-lookup"><span data-stu-id="e2292-112">String</span></span>|<span data-ttu-id="e2292-113">Fornece o tipo da rede.</span><span class="sxs-lookup"><span data-stu-id="e2292-113">Provides the type of the network.</span></span> <span data-ttu-id="e2292-114">Os valores possíveis `intranet`são `extranet`: `namedNetwork`,, `trusted`e.</span><span class="sxs-lookup"><span data-stu-id="e2292-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="e2292-115">NetworkName</span><span class="sxs-lookup"><span data-stu-id="e2292-115">networkName</span></span>|<span data-ttu-id="e2292-116">String</span><span class="sxs-lookup"><span data-stu-id="e2292-116">String</span></span>|<span data-ttu-id="e2292-117">Nome da rede.</span><span class="sxs-lookup"><span data-stu-id="e2292-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e2292-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2292-118">JSON representation</span></span>

<span data-ttu-id="e2292-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2292-119">Here is a JSON representation of the resource.</span></span>

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
