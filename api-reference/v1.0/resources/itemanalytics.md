---
author: daspek
ms.author: dspektor
title: tipo de recurso do multianalytics
description: O objeto PostItem fornece análises sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0b4ee2bba6cff84a99cf5a0e20dddc09ad87ee59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447651"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="91feb-103">tipo de recurso do multianalytics</span><span class="sxs-lookup"><span data-stu-id="91feb-103">itemAnalytics resource type</span></span>

<span data-ttu-id="91feb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91feb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91feb-105">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="91feb-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="91feb-106">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="91feb-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="91feb-107">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="91feb-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="91feb-108">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="91feb-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="91feb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91feb-109">Properties</span></span>

| <span data-ttu-id="91feb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91feb-110">Property</span></span>      | <span data-ttu-id="91feb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="91feb-111">Type</span></span>                 | <span data-ttu-id="91feb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="91feb-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="91feb-113">Época</span><span class="sxs-lookup"><span data-stu-id="91feb-113">allTime</span></span>       | <span data-ttu-id="91feb-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="91feb-114">[itemActivityStat][]</span></span> | <span data-ttu-id="91feb-115">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="91feb-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="91feb-116">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="91feb-116">lastSevenDays</span></span> | <span data-ttu-id="91feb-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="91feb-117">[itemActivityStat][]</span></span> | <span data-ttu-id="91feb-118">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="91feb-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="91feb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91feb-121">JSON representation</span></span>

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
