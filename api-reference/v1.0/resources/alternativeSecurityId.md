---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno.
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003451"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="23c7f-103">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="23c7f-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="23c7f-104">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="23c7f-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23c7f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23c7f-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="23c7f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23c7f-106">Properties</span></span>
| <span data-ttu-id="23c7f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23c7f-107">Property</span></span>         | <span data-ttu-id="23c7f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="23c7f-108">Type</span></span>       | <span data-ttu-id="23c7f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23c7f-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="23c7f-110">type</span><span class="sxs-lookup"><span data-stu-id="23c7f-110">type</span></span>             | <span data-ttu-id="23c7f-111">Int32</span><span class="sxs-lookup"><span data-stu-id="23c7f-111">Int32</span></span>      | <span data-ttu-id="23c7f-112">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="23c7f-112">For internal use only</span></span>
| <span data-ttu-id="23c7f-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="23c7f-113">identityProvider</span></span> | <span data-ttu-id="23c7f-114">string</span><span class="sxs-lookup"><span data-stu-id="23c7f-114">string</span></span>     | <span data-ttu-id="23c7f-115">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="23c7f-115">For internal use only</span></span>
| <span data-ttu-id="23c7f-116">key</span><span class="sxs-lookup"><span data-stu-id="23c7f-116">key</span></span>              | <span data-ttu-id="23c7f-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="23c7f-117">Edm.Binary</span></span> | <span data-ttu-id="23c7f-118">Somente para uso interno</span><span class="sxs-lookup"><span data-stu-id="23c7f-118">For internal use only</span></span>
