---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno.
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853799"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="cb554-103">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="cb554-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="cb554-104">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="cb554-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb554-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb554-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cb554-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb554-106">Properties</span></span>
| <span data-ttu-id="cb554-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb554-107">Property</span></span>         | <span data-ttu-id="cb554-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb554-108">Type</span></span>       | <span data-ttu-id="cb554-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb554-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="cb554-110">type</span><span class="sxs-lookup"><span data-stu-id="cb554-110">type</span></span>             | <span data-ttu-id="cb554-111">Int32</span><span class="sxs-lookup"><span data-stu-id="cb554-111">Int32</span></span>      | <span data-ttu-id="cb554-112">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="cb554-112">For internal use only</span></span>
| <span data-ttu-id="cb554-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="cb554-113">identityProvider</span></span> | <span data-ttu-id="cb554-114">string</span><span class="sxs-lookup"><span data-stu-id="cb554-114">string</span></span>     | <span data-ttu-id="cb554-115">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="cb554-115">For internal use only</span></span>
| <span data-ttu-id="cb554-116">key</span><span class="sxs-lookup"><span data-stu-id="cb554-116">key</span></span>              | <span data-ttu-id="cb554-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="cb554-117">Edm.Binary</span></span> | <span data-ttu-id="cb554-118">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="cb554-118">For internal use only</span></span>
