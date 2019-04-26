---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: a0e3bc3f217308d96eaadf6ab367431c7f1b8c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345428"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="cd975-102">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="cd975-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd975-103">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="cd975-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd975-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd975-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cd975-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd975-105">Properties</span></span>

| <span data-ttu-id="cd975-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd975-106">Property</span></span>    | <span data-ttu-id="cd975-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd975-107">Type</span></span>  | <span data-ttu-id="cd975-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd975-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="cd975-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="cd975-109">actionCount</span></span> | <span data-ttu-id="cd975-110">Int32</span><span class="sxs-lookup"><span data-stu-id="cd975-110">Int32</span></span> | <span data-ttu-id="cd975-111">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="cd975-111">The number of times the action took place.</span></span> <span data-ttu-id="cd975-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd975-112">Read-only.</span></span>
| <span data-ttu-id="cd975-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="cd975-113">actorCount</span></span>  | <span data-ttu-id="cd975-114">Int32</span><span class="sxs-lookup"><span data-stu-id="cd975-114">Int32</span></span> | <span data-ttu-id="cd975-115">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="cd975-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="cd975-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd975-116">Read-only.</span></span>

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
