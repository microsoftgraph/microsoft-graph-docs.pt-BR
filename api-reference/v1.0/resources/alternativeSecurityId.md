---
title: Tipo de recurso alternativeSecurityId
description: Apenas para uso interno.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d86d5f07a957abe45b898be08744c7c93853d78e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533152"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="c4078-103">Tipo de recurso alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="c4078-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="c4078-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4078-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4078-105">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="c4078-105">For internal use only.</span></span> <span data-ttu-id="c4078-106">Esse tipo complexo será preterido no futuro.</span><span class="sxs-lookup"><span data-stu-id="c4078-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4078-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4078-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c4078-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4078-108">Properties</span></span>
| <span data-ttu-id="c4078-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4078-109">Property</span></span>         | <span data-ttu-id="c4078-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4078-110">Type</span></span>       | <span data-ttu-id="c4078-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4078-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="c4078-112">type</span><span class="sxs-lookup"><span data-stu-id="c4078-112">type</span></span>             | <span data-ttu-id="c4078-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c4078-113">Int32</span></span>      | <span data-ttu-id="c4078-114">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="c4078-114">For internal use only</span></span>
| <span data-ttu-id="c4078-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="c4078-115">identityProvider</span></span> | <span data-ttu-id="c4078-116">string</span><span class="sxs-lookup"><span data-stu-id="c4078-116">string</span></span>     | <span data-ttu-id="c4078-117">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="c4078-117">For internal use only</span></span>
| <span data-ttu-id="c4078-118">chave</span><span class="sxs-lookup"><span data-stu-id="c4078-118">key</span></span>              | <span data-ttu-id="c4078-119">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="c4078-119">Edm.Binary</span></span> | <span data-ttu-id="c4078-120">Apenas para uso interno</span><span class="sxs-lookup"><span data-stu-id="c4078-120">For internal use only</span></span>
