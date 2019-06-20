---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno. Esse tipo complexo será preterido no futuro.
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083939"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="4edfa-104">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="4edfa-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="4edfa-105">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="4edfa-105">For internal use only.</span></span> <span data-ttu-id="4edfa-106">Esse tipo complexo será preterido no futuro.</span><span class="sxs-lookup"><span data-stu-id="4edfa-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4edfa-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4edfa-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4edfa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4edfa-108">Properties</span></span>
| <span data-ttu-id="4edfa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4edfa-109">Property</span></span>         | <span data-ttu-id="4edfa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4edfa-110">Type</span></span>       | <span data-ttu-id="4edfa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4edfa-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="4edfa-112">type</span><span class="sxs-lookup"><span data-stu-id="4edfa-112">type</span></span>             | <span data-ttu-id="4edfa-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4edfa-113">Int32</span></span>      | <span data-ttu-id="4edfa-114">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="4edfa-114">For internal use only</span></span>
| <span data-ttu-id="4edfa-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="4edfa-115">identityProvider</span></span> | <span data-ttu-id="4edfa-116">string</span><span class="sxs-lookup"><span data-stu-id="4edfa-116">string</span></span>     | <span data-ttu-id="4edfa-117">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="4edfa-117">For internal use only</span></span>
| <span data-ttu-id="4edfa-118">chave</span><span class="sxs-lookup"><span data-stu-id="4edfa-118">key</span></span>              | <span data-ttu-id="4edfa-119">EDM. Binary</span><span class="sxs-lookup"><span data-stu-id="4edfa-119">Edm.Binary</span></span> | <span data-ttu-id="4edfa-120">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="4edfa-120">For internal use only</span></span>
