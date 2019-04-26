---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 39209671b63b991a8fb3ccf1c830c8557fce27c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569974"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="c7e38-102">tipo de recurso itemActionStat</span><span class="sxs-lookup"><span data-stu-id="c7e38-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7e38-103">O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="c7e38-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7e38-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7e38-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c7e38-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7e38-105">Properties</span></span>

| <span data-ttu-id="c7e38-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7e38-106">Property</span></span>    | <span data-ttu-id="c7e38-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7e38-107">Type</span></span>  | <span data-ttu-id="c7e38-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7e38-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="c7e38-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="c7e38-109">actionCount</span></span> | <span data-ttu-id="c7e38-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c7e38-110">Int32</span></span> | <span data-ttu-id="c7e38-111">O número de vezes que a ação ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c7e38-111">The number of times the action took place.</span></span> <span data-ttu-id="c7e38-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7e38-112">Read-only.</span></span>
| <span data-ttu-id="c7e38-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="c7e38-113">actorCount</span></span>  | <span data-ttu-id="c7e38-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c7e38-114">Int32</span></span> | <span data-ttu-id="c7e38-115">O número de atores distintos que executaram a ação.</span><span class="sxs-lookup"><span data-stu-id="c7e38-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="c7e38-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7e38-116">Read-only.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactionstat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
