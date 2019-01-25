---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517628"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="e1fbc-102">tipo de recurso de itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="e1fbc-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1fbc-103">O recurso de **itemActivityStat** fornece informações sobre atividades realizadas dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1fbc-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1fbc-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a><span data-ttu-id="e1fbc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1fbc-105">Properties</span></span>

| <span data-ttu-id="e1fbc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1fbc-106">Property</span></span>         | <span data-ttu-id="e1fbc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1fbc-107">Type</span></span>                    | <span data-ttu-id="e1fbc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1fbc-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="e1fbc-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="e1fbc-109">incompleteData</span></span>   | <span data-ttu-id="e1fbc-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-110">[incompleteData][]</span></span>      | <span data-ttu-id="e1fbc-111">Indica que as estatísticas nesse intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="e1fbc-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-112">Read-only.</span></span>
| <span data-ttu-id="e1fbc-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="e1fbc-113">isTrending</span></span>       | <span data-ttu-id="e1fbc-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1fbc-114">Boolean</span></span>                 | <span data-ttu-id="e1fbc-115">Indica se o item é "tendências".</span><span class="sxs-lookup"><span data-stu-id="e1fbc-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="e1fbc-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-116">Read-only.</span></span>
| <span data-ttu-id="e1fbc-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e1fbc-117">startDateTime</span></span>    | <span data-ttu-id="e1fbc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1fbc-118">DateTimeOffset</span></span>          | <span data-ttu-id="e1fbc-119">Quando o intervalo for iniciado.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-119">When the interval starts.</span></span> <span data-ttu-id="e1fbc-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-120">Read-only.</span></span>
| <span data-ttu-id="e1fbc-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e1fbc-121">endDateTime</span></span>      | <span data-ttu-id="e1fbc-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1fbc-122">DateTimeOffset</span></span>          | <span data-ttu-id="e1fbc-123">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-123">When the interval ends.</span></span> <span data-ttu-id="e1fbc-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-124">Read-only.</span></span>
| <span data-ttu-id="e1fbc-125">create</span><span class="sxs-lookup"><span data-stu-id="e1fbc-125">create</span></span>           | <span data-ttu-id="e1fbc-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-126">[itemActionStat][]</span></span>      | <span data-ttu-id="e1fbc-127">Estatísticas sobre as ações **criar** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="e1fbc-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-128">Read-only.</span></span>
| <span data-ttu-id="e1fbc-129">edit</span><span class="sxs-lookup"><span data-stu-id="e1fbc-129">edit</span></span>             | <span data-ttu-id="e1fbc-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-130">[itemActionStat][]</span></span>      | <span data-ttu-id="e1fbc-131">Estatísticas sobre as ações de **Editar** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="e1fbc-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-132">Read-only.</span></span>
| <span data-ttu-id="e1fbc-133">delete</span><span class="sxs-lookup"><span data-stu-id="e1fbc-133">delete</span></span>           | <span data-ttu-id="e1fbc-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-134">[itemActionStat][]</span></span>      | <span data-ttu-id="e1fbc-135">Estatísticas sobre as ações **Excluir** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="e1fbc-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-136">Read-only.</span></span>
| <span data-ttu-id="e1fbc-137">move</span><span class="sxs-lookup"><span data-stu-id="e1fbc-137">move</span></span>             | <span data-ttu-id="e1fbc-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-138">[itemActionStat][]</span></span>      | <span data-ttu-id="e1fbc-139">Estatísticas sobre as ações de **Mover** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="e1fbc-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-140">Read-only.</span></span>
| <span data-ttu-id="e1fbc-141">Access</span><span class="sxs-lookup"><span data-stu-id="e1fbc-141">access</span></span>           | <span data-ttu-id="e1fbc-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-142">[itemActionStat][]</span></span>      | <span data-ttu-id="e1fbc-143">Estatísticas sobre as ações de **acesso** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="e1fbc-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1fbc-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="e1fbc-147">Relações</span><span class="sxs-lookup"><span data-stu-id="e1fbc-147">Relationships</span></span>

| <span data-ttu-id="e1fbc-148">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="e1fbc-148">Relationship name</span></span> | <span data-ttu-id="e1fbc-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1fbc-149">Type</span></span>                        | <span data-ttu-id="e1fbc-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1fbc-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="e1fbc-151">activities</span><span class="sxs-lookup"><span data-stu-id="e1fbc-151">activities</span></span>        | <span data-ttu-id="e1fbc-152">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="e1fbc-152">[itemActivity][] collection</span></span> | <span data-ttu-id="e1fbc-153">Expõe **itemActivities** representados neste recurso **itemActivityStat** .</span><span class="sxs-lookup"><span data-stu-id="e1fbc-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="e1fbc-155">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1fbc-155">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
