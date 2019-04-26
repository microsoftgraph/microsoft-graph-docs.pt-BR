---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: O naAnalytics
localization_priority: Normal
ms.openlocfilehash: 2869655b3b645fc8d30ceec3867c28ca81ac9d51
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345447"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="5347b-102">tipo de recurso do multiAnalytics</span><span class="sxs-lookup"><span data-stu-id="5347b-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5347b-103">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="5347b-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="5347b-104">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="5347b-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="5347b-105">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="5347b-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="5347b-106">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="5347b-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5347b-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5347b-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a><span data-ttu-id="5347b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5347b-108">Properties</span></span>

| <span data-ttu-id="5347b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5347b-109">Property</span></span>      | <span data-ttu-id="5347b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5347b-110">Type</span></span>                 | <span data-ttu-id="5347b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5347b-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="5347b-112">Época</span><span class="sxs-lookup"><span data-stu-id="5347b-112">allTime</span></span>       | <span data-ttu-id="5347b-113">[Entidadeitemactivitystat][]</span><span class="sxs-lookup"><span data-stu-id="5347b-113">[itemActivityStat][]</span></span> | <span data-ttu-id="5347b-114">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="5347b-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="5347b-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="5347b-115">lastSevenDays</span></span> | <span data-ttu-id="5347b-116">[Entidadeitemactivitystat][]</span><span class="sxs-lookup"><span data-stu-id="5347b-116">[itemActivityStat][]</span></span> | <span data-ttu-id="5347b-117">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="5347b-117">Analytics for the last seven days.</span></span>

[Entidadeitemactivitystat]: itemactivitystat.md
[itemActivityStat]: itemactivitystat.md


[Funçãogetactivitiesbyinterval]: ../api/itemactivity-getbyinterval.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": []
}
-->
