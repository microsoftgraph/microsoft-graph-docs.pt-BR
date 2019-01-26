---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno.
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579839"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="58f8a-103">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="58f8a-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="58f8a-104">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="58f8a-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="58f8a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58f8a-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="58f8a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58f8a-106">Properties</span></span>
| <span data-ttu-id="58f8a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58f8a-107">Property</span></span>         | <span data-ttu-id="58f8a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="58f8a-108">Type</span></span>       | <span data-ttu-id="58f8a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f8a-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="58f8a-110">type</span><span class="sxs-lookup"><span data-stu-id="58f8a-110">type</span></span>             | <span data-ttu-id="58f8a-111">Int32</span><span class="sxs-lookup"><span data-stu-id="58f8a-111">Int32</span></span>      | <span data-ttu-id="58f8a-112">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="58f8a-112">For internal use only</span></span>
| <span data-ttu-id="58f8a-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="58f8a-113">identityProvider</span></span> | <span data-ttu-id="58f8a-114">string</span><span class="sxs-lookup"><span data-stu-id="58f8a-114">string</span></span>     | <span data-ttu-id="58f8a-115">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="58f8a-115">For internal use only</span></span>
| <span data-ttu-id="58f8a-116">key</span><span class="sxs-lookup"><span data-stu-id="58f8a-116">key</span></span>              | <span data-ttu-id="58f8a-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="58f8a-117">Edm.Binary</span></span> | <span data-ttu-id="58f8a-118">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="58f8a-118">For internal use only</span></span>
