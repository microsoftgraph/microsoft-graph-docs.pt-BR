---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4207c85185281ec9944aa08dfce088739116bb8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447679"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="3ad8f-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="3ad8f-103">itemActionStat resource type</span></span>

<span data-ttu-id="3ad8f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3ad8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ad8f-105">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="3ad8f-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="3ad8f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ad8f-106">Properties</span></span>

| <span data-ttu-id="3ad8f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ad8f-107">Property</span></span>    | <span data-ttu-id="3ad8f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ad8f-108">Type</span></span>  | <span data-ttu-id="3ad8f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ad8f-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="3ad8f-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="3ad8f-110">actionCount</span></span> | <span data-ttu-id="3ad8f-111">Int32</span><span class="sxs-lookup"><span data-stu-id="3ad8f-111">Int32</span></span> | <span data-ttu-id="3ad8f-112">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3ad8f-112">The number of times the action took place.</span></span> <span data-ttu-id="3ad8f-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ad8f-113">Read-only.</span></span>
| <span data-ttu-id="3ad8f-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="3ad8f-114">actorCount</span></span>  | <span data-ttu-id="3ad8f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3ad8f-115">Int32</span></span> | <span data-ttu-id="3ad8f-116">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="3ad8f-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="3ad8f-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ad8f-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ad8f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ad8f-118">JSON representation</span></span>

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
