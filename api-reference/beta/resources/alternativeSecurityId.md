---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348330"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="b411e-104">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="b411e-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="b411e-105">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="b411e-105">For internal use only.</span></span> <span data-ttu-id="b411e-106">Esse tipo complexo será preterido no futuro.</span><span class="sxs-lookup"><span data-stu-id="b411e-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b411e-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b411e-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b411e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b411e-108">Properties</span></span>
| <span data-ttu-id="b411e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b411e-109">Property</span></span>         | <span data-ttu-id="b411e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b411e-110">Type</span></span>       | <span data-ttu-id="b411e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b411e-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="b411e-112">type</span><span class="sxs-lookup"><span data-stu-id="b411e-112">type</span></span>             | <span data-ttu-id="b411e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b411e-113">Int32</span></span>      | <span data-ttu-id="b411e-114">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="b411e-114">For internal use only</span></span>
| <span data-ttu-id="b411e-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b411e-115">identityProvider</span></span> | <span data-ttu-id="b411e-116">string</span><span class="sxs-lookup"><span data-stu-id="b411e-116">string</span></span>     | <span data-ttu-id="b411e-117">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="b411e-117">For internal use only</span></span>
| <span data-ttu-id="b411e-118">chave</span><span class="sxs-lookup"><span data-stu-id="b411e-118">key</span></span>              | <span data-ttu-id="b411e-119">EDM. Binary</span><span class="sxs-lookup"><span data-stu-id="b411e-119">Edm.Binary</span></span> | <span data-ttu-id="b411e-120">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="b411e-120">For internal use only</span></span>
