---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d5531fc969762219f4e2404787190649ecdaf11
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970596"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="80fd9-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="80fd9-103">itemActionStat resource type</span></span>

<span data-ttu-id="80fd9-104">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="80fd9-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="80fd9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80fd9-105">Properties</span></span>

| <span data-ttu-id="80fd9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80fd9-106">Property</span></span>    | <span data-ttu-id="80fd9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="80fd9-107">Type</span></span>  | <span data-ttu-id="80fd9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="80fd9-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="80fd9-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="80fd9-109">actionCount</span></span> | <span data-ttu-id="80fd9-110">Int32</span><span class="sxs-lookup"><span data-stu-id="80fd9-110">Int32</span></span> | <span data-ttu-id="80fd9-111">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="80fd9-111">The number of times the action took place.</span></span> <span data-ttu-id="80fd9-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80fd9-112">Read-only.</span></span>
| <span data-ttu-id="80fd9-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="80fd9-113">actorCount</span></span>  | <span data-ttu-id="80fd9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="80fd9-114">Int32</span></span> | <span data-ttu-id="80fd9-115">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="80fd9-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="80fd9-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80fd9-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80fd9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80fd9-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->
