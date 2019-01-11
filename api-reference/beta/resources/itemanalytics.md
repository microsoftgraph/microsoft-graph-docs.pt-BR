---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842410"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="9aea3-102">tipo de recurso de itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="9aea3-102">itemAnalytics resource type</span></span>

> <span data-ttu-id="9aea3-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9aea3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aea3-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9aea3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9aea3-105">O recurso de **itemAnalytics** fornece análise sobre atividades realizadas em um item.</span><span class="sxs-lookup"><span data-stu-id="9aea3-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="9aea3-106">Este recurso só está disponível no SharePoint e o OneDrive for Business no momento.</span><span class="sxs-lookup"><span data-stu-id="9aea3-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="9aea3-107">Você também pode usar [getActivitiesByInterval][] API para recuperar o analytics sobre um intervalo de tempo personalizado ou um intervalo.</span><span class="sxs-lookup"><span data-stu-id="9aea3-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="9aea3-108">**Observação:** O recurso de **itemAnalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="9aea3-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aea3-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9aea3-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9aea3-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9aea3-110">Properties</span></span>

| <span data-ttu-id="9aea3-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aea3-111">Property</span></span>      | <span data-ttu-id="9aea3-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aea3-112">Type</span></span>                 | <span data-ttu-id="9aea3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aea3-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="9aea3-114">allTime</span><span class="sxs-lookup"><span data-stu-id="9aea3-114">allTime</span></span>       | <span data-ttu-id="9aea3-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="9aea3-115">[itemActivityStat][]</span></span> | <span data-ttu-id="9aea3-116">Análise sobre o tempo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="9aea3-116">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="9aea3-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="9aea3-117">lastSevenDays</span></span> | <span data-ttu-id="9aea3-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="9aea3-118">[itemActivityStat][]</span></span> | <span data-ttu-id="9aea3-119">Análise nos últimos sete dias.</span><span class="sxs-lookup"><span data-stu-id="9aea3-119">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
