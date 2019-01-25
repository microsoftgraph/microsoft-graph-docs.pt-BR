---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514961"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="8c90b-102">tipo de recurso de itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="8c90b-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c90b-103">O recurso de **itemAnalytics** fornece análise sobre atividades realizadas em um item.</span><span class="sxs-lookup"><span data-stu-id="8c90b-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="8c90b-104">Este recurso só está disponível no SharePoint e o OneDrive for Business no momento.</span><span class="sxs-lookup"><span data-stu-id="8c90b-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="8c90b-105">Você também pode usar [getActivitiesByInterval][] API para recuperar o analytics sobre um intervalo de tempo personalizado ou um intervalo.</span><span class="sxs-lookup"><span data-stu-id="8c90b-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="8c90b-106">**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="8c90b-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c90b-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c90b-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8c90b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c90b-108">Properties</span></span>

| <span data-ttu-id="8c90b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c90b-109">Property</span></span>      | <span data-ttu-id="8c90b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c90b-110">Type</span></span>                 | <span data-ttu-id="8c90b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c90b-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="8c90b-112">allTime</span><span class="sxs-lookup"><span data-stu-id="8c90b-112">allTime</span></span>       | <span data-ttu-id="8c90b-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8c90b-113">[itemActivityStat][]</span></span> | <span data-ttu-id="8c90b-114">Análise sobre o tempo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="8c90b-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="8c90b-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="8c90b-115">lastSevenDays</span></span> | <span data-ttu-id="8c90b-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8c90b-116">[itemActivityStat][]</span></span> | <span data-ttu-id="8c90b-117">Análise nos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="8c90b-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
