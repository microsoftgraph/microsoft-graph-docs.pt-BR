---
title: tipo de recurso de networkLocationDetail
description: Indica detalhes associadas ao local de rede. .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037625"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="33453-104">tipo de recurso de networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="33453-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="33453-105">Indica detalhes associadas ao local de rede.</span><span class="sxs-lookup"><span data-stu-id="33453-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="33453-106">.</span><span class="sxs-lookup"><span data-stu-id="33453-106"></span></span>



## <a name="properties"></a><span data-ttu-id="33453-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33453-107">Properties</span></span>
| <span data-ttu-id="33453-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33453-108">Property</span></span>     | <span data-ttu-id="33453-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="33453-109">Type</span></span>   |<span data-ttu-id="33453-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33453-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33453-111">networkType</span><span class="sxs-lookup"><span data-stu-id="33453-111">networkType</span></span>|<span data-ttu-id="33453-112">String</span><span class="sxs-lookup"><span data-stu-id="33453-112">String</span></span>|<span data-ttu-id="33453-113">Fornece o tipo da rede.</span><span class="sxs-lookup"><span data-stu-id="33453-113">Provides the type of the network.</span></span> <span data-ttu-id="33453-114">Os valores possíveis são `intranet`, `extranet`, `namedNetwork`, e `trusted`.</span><span class="sxs-lookup"><span data-stu-id="33453-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="33453-115">networkName</span><span class="sxs-lookup"><span data-stu-id="33453-115">networkName</span></span>|<span data-ttu-id="33453-116">String</span><span class="sxs-lookup"><span data-stu-id="33453-116">String</span></span>|<span data-ttu-id="33453-117">Nome da rede.</span><span class="sxs-lookup"><span data-stu-id="33453-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="33453-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33453-118">JSON representation</span></span>

<span data-ttu-id="33453-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33453-119">Here is a JSON representation of the resource.</span></span>

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