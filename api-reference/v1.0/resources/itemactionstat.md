---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7eda0f6ddbed16dadf1eac4a3ea737cdd7fd2c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036754"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="b67ea-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="b67ea-103">itemActionStat resource type</span></span>

<span data-ttu-id="b67ea-104">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="b67ea-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="b67ea-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b67ea-105">Properties</span></span>

| <span data-ttu-id="b67ea-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b67ea-106">Property</span></span>    | <span data-ttu-id="b67ea-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b67ea-107">Type</span></span>  | <span data-ttu-id="b67ea-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b67ea-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="b67ea-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="b67ea-109">actionCount</span></span> | <span data-ttu-id="b67ea-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b67ea-110">Int32</span></span> | <span data-ttu-id="b67ea-111">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="b67ea-111">The number of times the action took place.</span></span> <span data-ttu-id="b67ea-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b67ea-112">Read-only.</span></span>
| <span data-ttu-id="b67ea-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="b67ea-113">actorCount</span></span>  | <span data-ttu-id="b67ea-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b67ea-114">Int32</span></span> | <span data-ttu-id="b67ea-115">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="b67ea-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="b67ea-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b67ea-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b67ea-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b67ea-117">JSON representation</span></span>

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
