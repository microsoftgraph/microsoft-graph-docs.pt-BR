---
author: daspek
description: O recurso do Microsoft Analytics oferece análise sobre as atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.
ms.date: 09/14/2017
title: O naanalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4035ff821927d520ed457c3040be01bd9368240c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523097"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="4a401-104">tipo de recurso do multianalytics</span><span class="sxs-lookup"><span data-stu-id="4a401-104">itemAnalytics resource type</span></span>

<span data-ttu-id="4a401-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4a401-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a401-106">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="4a401-106">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="4a401-107">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4a401-107">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="4a401-108">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="4a401-108">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="4a401-109">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="4a401-109">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a401-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a401-110">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4a401-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a401-111">Properties</span></span>

| <span data-ttu-id="4a401-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a401-112">Property</span></span>      | <span data-ttu-id="4a401-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a401-113">Type</span></span>                 | <span data-ttu-id="4a401-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a401-114">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="4a401-115">Época</span><span class="sxs-lookup"><span data-stu-id="4a401-115">allTime</span></span>       | <span data-ttu-id="4a401-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4a401-116">[itemActivityStat][]</span></span> | <span data-ttu-id="4a401-117">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="4a401-117">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="4a401-118">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="4a401-118">lastSevenDays</span></span> | <span data-ttu-id="4a401-119">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="4a401-119">[itemActivityStat][]</span></span> | <span data-ttu-id="4a401-120">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="4a401-120">Analytics for the last seven days.</span></span>

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
