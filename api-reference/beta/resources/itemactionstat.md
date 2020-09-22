---
author: daspek
description: O recurso itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8316239a7e00cdc74921c42b70431eba60cdc2d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075669"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="f01c5-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="f01c5-103">itemActionStat resource type</span></span>

<span data-ttu-id="f01c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f01c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f01c5-105">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="f01c5-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f01c5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f01c5-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f01c5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f01c5-107">Properties</span></span>

| <span data-ttu-id="f01c5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f01c5-108">Property</span></span>    | <span data-ttu-id="f01c5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f01c5-109">Type</span></span>  | <span data-ttu-id="f01c5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f01c5-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="f01c5-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="f01c5-111">actionCount</span></span> | <span data-ttu-id="f01c5-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f01c5-112">Int32</span></span> | <span data-ttu-id="f01c5-113">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f01c5-113">The number of times the action took place.</span></span> <span data-ttu-id="f01c5-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f01c5-114">Read-only.</span></span>
| <span data-ttu-id="f01c5-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="f01c5-115">actorCount</span></span>  | <span data-ttu-id="f01c5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f01c5-116">Int32</span></span> | <span data-ttu-id="f01c5-117">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="f01c5-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="f01c5-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f01c5-118">Read-only.</span></span>

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


