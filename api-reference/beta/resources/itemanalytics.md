---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: O naAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581628"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="f4450-102">tipo de recurso do multiAnalytics</span><span class="sxs-lookup"><span data-stu-id="f4450-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4450-103">O recurso do Microsoft **Analytics** oferece análise sobre as atividades que ocorreram em um item.</span><span class="sxs-lookup"><span data-stu-id="f4450-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="f4450-104">No momento, esse recurso só está disponível no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f4450-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="f4450-105">Você também pode usar a API [funçãogetactivitiesbyinterval][] para recuperar a análise por um intervalo ou intervalo de tempo personalizado.</span><span class="sxs-lookup"><span data-stu-id="f4450-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="f4450-106">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="f4450-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4450-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4450-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4450-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4450-108">Properties</span></span>

| <span data-ttu-id="f4450-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4450-109">Property</span></span>      | <span data-ttu-id="f4450-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4450-110">Type</span></span>                 | <span data-ttu-id="f4450-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4450-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="f4450-112">Época</span><span class="sxs-lookup"><span data-stu-id="f4450-112">allTime</span></span>       | <span data-ttu-id="f4450-113">[Entidadeitemactivitystat][]</span><span class="sxs-lookup"><span data-stu-id="f4450-113">[itemActivityStat][]</span></span> | <span data-ttu-id="f4450-114">Análise sobre o ciclo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="f4450-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="f4450-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="f4450-115">lastSevenDays</span></span> | <span data-ttu-id="f4450-116">[Entidadeitemactivitystat][]</span><span class="sxs-lookup"><span data-stu-id="f4450-116">[itemActivityStat][]</span></span> | <span data-ttu-id="f4450-117">Análise dos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="f4450-117">Analytics for the last seven days.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
