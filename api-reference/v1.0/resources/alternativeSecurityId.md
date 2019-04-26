---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno.
localization_priority: Normal
ms.openlocfilehash: 60e45c6d914c64f92b9f15f78fda22372a23e91f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345838"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="015fc-103">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="015fc-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="015fc-104">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="015fc-104">For internal use only.</span></span> <span data-ttu-id="015fc-105">Esse tipo complexo será preterido no futuro.</span><span class="sxs-lookup"><span data-stu-id="015fc-105">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="015fc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="015fc-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="015fc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="015fc-107">Properties</span></span>
| <span data-ttu-id="015fc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="015fc-108">Property</span></span>         | <span data-ttu-id="015fc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="015fc-109">Type</span></span>       | <span data-ttu-id="015fc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="015fc-110">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="015fc-111">type</span><span class="sxs-lookup"><span data-stu-id="015fc-111">type</span></span>             | <span data-ttu-id="015fc-112">Int32</span><span class="sxs-lookup"><span data-stu-id="015fc-112">Int32</span></span>      | <span data-ttu-id="015fc-113">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="015fc-113">For internal use only</span></span>
| <span data-ttu-id="015fc-114">identityProvider</span><span class="sxs-lookup"><span data-stu-id="015fc-114">identityProvider</span></span> | <span data-ttu-id="015fc-115">string</span><span class="sxs-lookup"><span data-stu-id="015fc-115">string</span></span>     | <span data-ttu-id="015fc-116">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="015fc-116">For internal use only</span></span>
| <span data-ttu-id="015fc-117">chave</span><span class="sxs-lookup"><span data-stu-id="015fc-117">key</span></span>              | <span data-ttu-id="015fc-118">EDM. Binary</span><span class="sxs-lookup"><span data-stu-id="015fc-118">Edm.Binary</span></span> | <span data-ttu-id="015fc-119">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="015fc-119">For internal use only</span></span>
