---
title: tipo de recurso de networkLocationDetail
description: Indica detalhes associadas ao local de rede. .
localization_priority: Normal
ms.openlocfilehash: 62bdb23c63beb89b85386e6bea67face097cf1ae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570936"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="9037e-104">tipo de recurso de networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="9037e-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="9037e-105">Indica detalhes associadas ao local de rede.</span><span class="sxs-lookup"><span data-stu-id="9037e-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="9037e-106">.</span><span class="sxs-lookup"><span data-stu-id="9037e-106"></span></span>



## <a name="properties"></a><span data-ttu-id="9037e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9037e-107">Properties</span></span>
| <span data-ttu-id="9037e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9037e-108">Property</span></span>     | <span data-ttu-id="9037e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9037e-109">Type</span></span>   |<span data-ttu-id="9037e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9037e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9037e-111">networkType</span><span class="sxs-lookup"><span data-stu-id="9037e-111">networkType</span></span>| <span data-ttu-id="9037e-112">cadeia de caracteres de enum</span><span class="sxs-lookup"><span data-stu-id="9037e-112">enum-string</span></span> |<span data-ttu-id="9037e-113">Fornece o tipo da rede.</span><span class="sxs-lookup"><span data-stu-id="9037e-113">Provides the type of the network.</span></span> <span data-ttu-id="9037e-114">Os valores possíveis são `intranet`, `extranet`, `namedNetwork`, e `trusted`.</span><span class="sxs-lookup"><span data-stu-id="9037e-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="9037e-115">networkName</span><span class="sxs-lookup"><span data-stu-id="9037e-115">networkName</span></span>|<span data-ttu-id="9037e-116">String</span><span class="sxs-lookup"><span data-stu-id="9037e-116">String</span></span>|<span data-ttu-id="9037e-117">Nome da rede.</span><span class="sxs-lookup"><span data-stu-id="9037e-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9037e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9037e-118">JSON representation</span></span>

<span data-ttu-id="9037e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9037e-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": " intranet | extranet | namedNetwork | trusted ",
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
