---
author: daspek
description: O recurso do Microsoft Analytics oferece análise sobre as atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.
ms.date: 09/14/2017
title: O naanalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0ef1fd6778b9ed31c0cd6dcd5ac14316675d697f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075627"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="fd721-104">tipo de recurso do multianalytics</span><span class="sxs-lookup"><span data-stu-id="fd721-104">itemAnalytics resource type</span></span>

<span data-ttu-id="fd721-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd721-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd721-106">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="fd721-106">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="fd721-107">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="fd721-107">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="fd721-108">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="fd721-108">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="fd721-109">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="fd721-109">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd721-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd721-110">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fd721-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd721-111">Properties</span></span>

| <span data-ttu-id="fd721-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd721-112">Property</span></span>      | <span data-ttu-id="fd721-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd721-113">Type</span></span>                 | <span data-ttu-id="fd721-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd721-114">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="fd721-115">Época</span><span class="sxs-lookup"><span data-stu-id="fd721-115">allTime</span></span>       | <span data-ttu-id="fd721-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="fd721-116">[itemActivityStat][]</span></span> | <span data-ttu-id="fd721-117">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="fd721-117">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="fd721-118">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="fd721-118">lastSevenDays</span></span> | <span data-ttu-id="fd721-119">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="fd721-119">[itemActivityStat][]</span></span> | <span data-ttu-id="fd721-120">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="fd721-120">Analytics for the last seven days.</span></span>

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


