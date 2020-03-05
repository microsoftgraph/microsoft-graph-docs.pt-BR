---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4e3dfae11009000fa89eccb7c0263867fe2a1562
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508328"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="9830b-104">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="9830b-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="9830b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9830b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9830b-106">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="9830b-106">For internal use only.</span></span> <span data-ttu-id="9830b-107">Esse tipo complexo será preterido no futuro.</span><span class="sxs-lookup"><span data-stu-id="9830b-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9830b-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9830b-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9830b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9830b-109">Properties</span></span>
| <span data-ttu-id="9830b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9830b-110">Property</span></span>         | <span data-ttu-id="9830b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9830b-111">Type</span></span>       | <span data-ttu-id="9830b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9830b-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="9830b-113">type</span><span class="sxs-lookup"><span data-stu-id="9830b-113">type</span></span>             | <span data-ttu-id="9830b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9830b-114">Int32</span></span>      | <span data-ttu-id="9830b-115">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="9830b-115">For internal use only</span></span>
| <span data-ttu-id="9830b-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="9830b-116">identityProvider</span></span> | <span data-ttu-id="9830b-117">string</span><span class="sxs-lookup"><span data-stu-id="9830b-117">string</span></span>     | <span data-ttu-id="9830b-118">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="9830b-118">For internal use only</span></span>
| <span data-ttu-id="9830b-119">chave</span><span class="sxs-lookup"><span data-stu-id="9830b-119">key</span></span>              | <span data-ttu-id="9830b-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="9830b-120">Edm.Binary</span></span> | <span data-ttu-id="9830b-121">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="9830b-121">For internal use only</span></span>
