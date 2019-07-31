---
author: daspek
description: O recurso do Microsoft Analytics oferece análise sobre as atividades que ocorreram em um item. No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.
ms.date: 09/14/2017
title: O naanalytics
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d2be5c7665961248e989101a1a9bd21eb805e6e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967090"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="e235a-104">tipo de recurso do multianalytics</span><span class="sxs-lookup"><span data-stu-id="e235a-104">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e235a-105">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="e235a-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="e235a-106">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e235a-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="e235a-107">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="e235a-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="e235a-108">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="e235a-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e235a-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e235a-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e235a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e235a-110">Properties</span></span>

| <span data-ttu-id="e235a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e235a-111">Property</span></span>      | <span data-ttu-id="e235a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="e235a-112">Type</span></span>                 | <span data-ttu-id="e235a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e235a-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="e235a-114">Época</span><span class="sxs-lookup"><span data-stu-id="e235a-114">allTime</span></span>       | <span data-ttu-id="e235a-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="e235a-115">[itemActivityStat][]</span></span> | <span data-ttu-id="e235a-116">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="e235a-116">Analytics over the item's lifespan.</span></span>
| <span data-ttu-id="e235a-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="e235a-117">lastSevenDays</span></span> | <span data-ttu-id="e235a-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="e235a-118">[itemActivityStat][]</span></span> | <span data-ttu-id="e235a-119">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="e235a-119">Analytics for the last seven days.</span></span>

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
