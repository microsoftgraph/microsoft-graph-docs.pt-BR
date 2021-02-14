---
author: daspek
title: Tipo de recurso itemAnalytics
description: O objeto ItemAnalytics fornece análises sobre atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96ad65ef5cc8907663a9ca67e5ea2b7546b8fa03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238656"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="40692-103">Tipo de recurso itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="40692-103">itemAnalytics resource type</span></span>

<span data-ttu-id="40692-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40692-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40692-105">O **recurso itemAnalytics** fornece análises sobre atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="40692-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="40692-106">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="40692-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="40692-107">Você também pode usar a API [getActivitiesByInterval][] para recuperar a análise em um intervalo de tempo ou intervalo personalizado.</span><span class="sxs-lookup"><span data-stu-id="40692-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="40692-108">**Observação:** O **recurso itemAnalytics** ainda não está disponível em todas as [implantações nacionais.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="40692-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="40692-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40692-109">Properties</span></span>

| <span data-ttu-id="40692-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40692-110">Property</span></span>      | <span data-ttu-id="40692-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="40692-111">Type</span></span>                 | <span data-ttu-id="40692-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="40692-112">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="40692-113">allTime</span><span class="sxs-lookup"><span data-stu-id="40692-113">allTime</span></span>       | <span data-ttu-id="40692-114">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="40692-114">[itemActivityStat][]</span></span> | <span data-ttu-id="40692-115">Análise sobre o tempo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="40692-115">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="40692-116">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="40692-116">lastSevenDays</span></span> | <span data-ttu-id="40692-117">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="40692-117">[itemActivityStat][]</span></span> | <span data-ttu-id="40692-118">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="40692-118">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="40692-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40692-121">JSON representation</span></span>

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

