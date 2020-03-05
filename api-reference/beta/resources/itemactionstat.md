---
author: daspek
description: O recurso itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6ab31d8a155e0b9fd54b3f2185e7d05969291ec1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523125"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="44e2e-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="44e2e-103">itemActionStat resource type</span></span>

<span data-ttu-id="44e2e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44e2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44e2e-105">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="44e2e-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44e2e-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44e2e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="44e2e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44e2e-107">Properties</span></span>

| <span data-ttu-id="44e2e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44e2e-108">Property</span></span>    | <span data-ttu-id="44e2e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="44e2e-109">Type</span></span>  | <span data-ttu-id="44e2e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44e2e-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="44e2e-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="44e2e-111">actionCount</span></span> | <span data-ttu-id="44e2e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="44e2e-112">Int32</span></span> | <span data-ttu-id="44e2e-113">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="44e2e-113">The number of times the action took place.</span></span> <span data-ttu-id="44e2e-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44e2e-114">Read-only.</span></span>
| <span data-ttu-id="44e2e-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="44e2e-115">actorCount</span></span>  | <span data-ttu-id="44e2e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="44e2e-116">Int32</span></span> | <span data-ttu-id="44e2e-117">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="44e2e-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="44e2e-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44e2e-118">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->
