---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: spunukol
ms.openlocfilehash: 9aa6802dcf077ffd78ae29a73d45a4046d35cb71
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807546"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="400f4-104">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="400f4-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="400f4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="400f4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="400f4-106">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="400f4-106">For internal use only.</span></span> <span data-ttu-id="400f4-107">Esse tipo complexo será preterido no futuro.</span><span class="sxs-lookup"><span data-stu-id="400f4-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="400f4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="400f4-108">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a><span data-ttu-id="400f4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="400f4-109">Properties</span></span>
| <span data-ttu-id="400f4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="400f4-110">Property</span></span>         | <span data-ttu-id="400f4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="400f4-111">Type</span></span>       | <span data-ttu-id="400f4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="400f4-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="400f4-113">type</span><span class="sxs-lookup"><span data-stu-id="400f4-113">type</span></span>             | <span data-ttu-id="400f4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="400f4-114">Int32</span></span>      | <span data-ttu-id="400f4-115">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="400f4-115">For internal use only</span></span>
| <span data-ttu-id="400f4-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="400f4-116">identityProvider</span></span> | <span data-ttu-id="400f4-117">string</span><span class="sxs-lookup"><span data-stu-id="400f4-117">string</span></span>     | <span data-ttu-id="400f4-118">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="400f4-118">For internal use only</span></span>
| <span data-ttu-id="400f4-119">chave</span><span class="sxs-lookup"><span data-stu-id="400f4-119">key</span></span>              | <span data-ttu-id="400f4-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="400f4-120">Edm.Binary</span></span> | <span data-ttu-id="400f4-121">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="400f4-121">For internal use only</span></span>
