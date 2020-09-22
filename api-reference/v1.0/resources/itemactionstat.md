---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1be83bef880b967758a803e694b068df9bfaebf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041264"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="377e2-103">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="377e2-103">itemActionStat resource type</span></span>

<span data-ttu-id="377e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="377e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="377e2-105">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="377e2-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="377e2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="377e2-106">Properties</span></span>

| <span data-ttu-id="377e2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="377e2-107">Property</span></span>    | <span data-ttu-id="377e2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="377e2-108">Type</span></span>  | <span data-ttu-id="377e2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="377e2-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="377e2-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="377e2-110">actionCount</span></span> | <span data-ttu-id="377e2-111">Int32</span><span class="sxs-lookup"><span data-stu-id="377e2-111">Int32</span></span> | <span data-ttu-id="377e2-112">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="377e2-112">The number of times the action took place.</span></span> <span data-ttu-id="377e2-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="377e2-113">Read-only.</span></span>
| <span data-ttu-id="377e2-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="377e2-114">actorCount</span></span>  | <span data-ttu-id="377e2-115">Int32</span><span class="sxs-lookup"><span data-stu-id="377e2-115">Int32</span></span> | <span data-ttu-id="377e2-116">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="377e2-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="377e2-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="377e2-117">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="377e2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="377e2-118">JSON representation</span></span>

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

