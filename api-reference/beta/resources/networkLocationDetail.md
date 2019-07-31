---
title: tipo de recurso networkLocationDetail
description: Indica detalhes associados ao local de rede. .
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b7e12a87889909737cac9a52fadf64231f7f2a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009605"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="d1955-104">tipo de recurso networkLocationDetail</span><span class="sxs-lookup"><span data-stu-id="d1955-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="d1955-105">Indica detalhes associados ao local de rede.</span><span class="sxs-lookup"><span data-stu-id="d1955-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="d1955-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1955-106">Properties</span></span>
| <span data-ttu-id="d1955-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1955-107">Property</span></span>     | <span data-ttu-id="d1955-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1955-108">Type</span></span>   |<span data-ttu-id="d1955-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1955-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1955-110">NetworkType</span><span class="sxs-lookup"><span data-stu-id="d1955-110">networkType</span></span>|<span data-ttu-id="d1955-111">NetworkType</span><span class="sxs-lookup"><span data-stu-id="d1955-111">networkType</span></span>|<span data-ttu-id="d1955-112">Fornece o tipo da rede.</span><span class="sxs-lookup"><span data-stu-id="d1955-112">Provides the type of the network.</span></span> <span data-ttu-id="d1955-113">Os valores possíveis são `intranet`: `extranet` `namedNetwork`,, e `trusted`.</span><span class="sxs-lookup"><span data-stu-id="d1955-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="d1955-114">networknames</span><span class="sxs-lookup"><span data-stu-id="d1955-114">networkNames</span></span>|<span data-ttu-id="d1955-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1955-115">String collection</span></span>|<span data-ttu-id="d1955-116">Nomes da rede.</span><span class="sxs-lookup"><span data-stu-id="d1955-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d1955-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1955-117">JSON representation</span></span>

<span data-ttu-id="d1955-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1955-118">Here is a JSON representation of the resource.</span></span>

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
