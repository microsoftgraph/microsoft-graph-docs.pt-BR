---
author: daspek
title: Tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação durante um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 13bc306a1b14d7d59ec8eddda5b02a5cba84e649
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238523"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="bc5ed-103">Tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="bc5ed-103">itemActionStat resource type</span></span>

<span data-ttu-id="bc5ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc5ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc5ed-105">O **recurso itemActionStat** fornece detalhes agregados sobre uma ação durante um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="bc5ed-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="bc5ed-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc5ed-106">Properties</span></span>

| <span data-ttu-id="bc5ed-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc5ed-107">Property</span></span>    | <span data-ttu-id="bc5ed-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc5ed-108">Type</span></span>  | <span data-ttu-id="bc5ed-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5ed-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="bc5ed-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="bc5ed-110">actionCount</span></span> | <span data-ttu-id="bc5ed-111">Int32</span><span class="sxs-lookup"><span data-stu-id="bc5ed-111">Int32</span></span> | <span data-ttu-id="bc5ed-112">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="bc5ed-112">The number of times the action took place.</span></span> <span data-ttu-id="bc5ed-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc5ed-113">Read-only.</span></span>
| <span data-ttu-id="bc5ed-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="bc5ed-114">actorCount</span></span>  | <span data-ttu-id="bc5ed-115">Int32</span><span class="sxs-lookup"><span data-stu-id="bc5ed-115">Int32</span></span> | <span data-ttu-id="bc5ed-116">O número de atores distintos que realizaram a ação.</span><span class="sxs-lookup"><span data-stu-id="bc5ed-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="bc5ed-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc5ed-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc5ed-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc5ed-118">JSON representation</span></span>

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

