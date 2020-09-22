---
author: daspek
ms.author: dspektor
title: tipo de recurso do multianalytics
description: O objeto PostItem fornece análises sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 879fad9ae77f065a7235a6adbfde5f742a1970f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009293"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="92303-103">tipo de recurso do multianalytics</span><span class="sxs-lookup"><span data-stu-id="92303-103">itemAnalytics resource type</span></span>

<span data-ttu-id="92303-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92303-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92303-105">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="92303-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="92303-106">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="92303-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="92303-107">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="92303-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="92303-108">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="92303-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="92303-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92303-109">Properties</span></span>

| <span data-ttu-id="92303-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92303-110">Property</span></span>      | <span data-ttu-id="92303-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="92303-111">Type</span></span>                 | <span data-ttu-id="92303-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="92303-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="92303-113">Época</span><span class="sxs-lookup"><span data-stu-id="92303-113">allTime</span></span>       | <span data-ttu-id="92303-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="92303-114">[itemActivityStat][]</span></span> | <span data-ttu-id="92303-115">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="92303-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="92303-116">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="92303-116">lastSevenDays</span></span> | <span data-ttu-id="92303-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="92303-117">[itemActivityStat][]</span></span> | <span data-ttu-id="92303-118">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="92303-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="92303-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92303-121">JSON representation</span></span>

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

