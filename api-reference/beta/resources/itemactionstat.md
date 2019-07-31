---
author: daspek
description: O recurso itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 719a443af65fd9642feee3bc8ddbc832eb3964c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010109"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="db3e4-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="db3e4-103">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db3e4-104">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="db3e4-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db3e4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db3e4-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="db3e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db3e4-106">Properties</span></span>

| <span data-ttu-id="db3e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db3e4-107">Property</span></span>    | <span data-ttu-id="db3e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="db3e4-108">Type</span></span>  | <span data-ttu-id="db3e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db3e4-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="db3e4-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="db3e4-110">actionCount</span></span> | <span data-ttu-id="db3e4-111">Int32</span><span class="sxs-lookup"><span data-stu-id="db3e4-111">Int32</span></span> | <span data-ttu-id="db3e4-112">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="db3e4-112">The number of times the action took place.</span></span> <span data-ttu-id="db3e4-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db3e4-113">Read-only.</span></span>
| <span data-ttu-id="db3e4-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="db3e4-114">actorCount</span></span>  | <span data-ttu-id="db3e4-115">Int32</span><span class="sxs-lookup"><span data-stu-id="db3e4-115">Int32</span></span> | <span data-ttu-id="db3e4-116">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="db3e4-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="db3e4-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db3e4-117">Read-only.</span></span>

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
