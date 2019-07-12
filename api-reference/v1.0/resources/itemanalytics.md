---
author: daspek
ms.author: dspektor
title: tipo de recurso do multianalytics
description: O objeto PostItem fornece análises sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a18d12bd2b431d147f2d23ea2c958cd75078c9a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620413"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="8a93e-103">tipo de recurso do multianalytics</span><span class="sxs-lookup"><span data-stu-id="8a93e-103">itemAnalytics resource type</span></span>

<span data-ttu-id="8a93e-104">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="8a93e-104">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="8a93e-105">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="8a93e-105">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="8a93e-106">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="8a93e-106">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="8a93e-107">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="8a93e-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="properties"></a><span data-ttu-id="8a93e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a93e-108">Properties</span></span>

| <span data-ttu-id="8a93e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a93e-109">Property</span></span>      | <span data-ttu-id="8a93e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a93e-110">Type</span></span>                 | <span data-ttu-id="8a93e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a93e-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="8a93e-112">Época</span><span class="sxs-lookup"><span data-stu-id="8a93e-112">allTime</span></span>       | <span data-ttu-id="8a93e-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8a93e-113">[itemActivityStat][]</span></span> | <span data-ttu-id="8a93e-114">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="8a93e-114">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="8a93e-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="8a93e-115">lastSevenDays</span></span> | <span data-ttu-id="8a93e-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8a93e-116">[itemActivityStat][]</span></span> | <span data-ttu-id="8a93e-117">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="8a93e-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="json-representation"></a><span data-ttu-id="8a93e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a93e-120">JSON representation</span></span>

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
