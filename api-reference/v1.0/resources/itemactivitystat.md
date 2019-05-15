---
author: daspek
ms.author: dspektor
title: tipo de recurso Entidadeitemactivitystat
description: O objeto Entidadeitemactivitystat fornece informações sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3af10bba565585341d04cdc47702e18e71d8accd
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970600"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="51c5a-103">tipo de recurso Entidadeitemactivitystat</span><span class="sxs-lookup"><span data-stu-id="51c5a-103">itemActivityStat resource type</span></span>

<span data-ttu-id="51c5a-104">O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="51c5a-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="51c5a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51c5a-105">Properties</span></span>

| <span data-ttu-id="51c5a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51c5a-106">Property</span></span>         | <span data-ttu-id="51c5a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51c5a-107">Type</span></span>                    | <span data-ttu-id="51c5a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51c5a-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="51c5a-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="51c5a-109">incompleteData</span></span>   | <span data-ttu-id="51c5a-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-110">[incompleteData][]</span></span>      | <span data-ttu-id="51c5a-111">Indica que as estatísticas neste intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="51c5a-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="51c5a-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-112">Read-only.</span></span>
| <span data-ttu-id="51c5a-113">istendência</span><span class="sxs-lookup"><span data-stu-id="51c5a-113">isTrending</span></span>       | <span data-ttu-id="51c5a-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="51c5a-114">Boolean</span></span>                 | <span data-ttu-id="51c5a-115">Indica se o item é "Trending".</span><span class="sxs-lookup"><span data-stu-id="51c5a-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="51c5a-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-116">Read-only.</span></span>
| <span data-ttu-id="51c5a-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="51c5a-117">startDateTime</span></span>    | <span data-ttu-id="51c5a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51c5a-118">DateTimeOffset</span></span>          | <span data-ttu-id="51c5a-119">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="51c5a-119">When the interval starts.</span></span> <span data-ttu-id="51c5a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-120">Read-only.</span></span>
| <span data-ttu-id="51c5a-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="51c5a-121">endDateTime</span></span>      | <span data-ttu-id="51c5a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51c5a-122">DateTimeOffset</span></span>          | <span data-ttu-id="51c5a-123">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="51c5a-123">When the interval ends.</span></span> <span data-ttu-id="51c5a-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-124">Read-only.</span></span>
| <span data-ttu-id="51c5a-125">create</span><span class="sxs-lookup"><span data-stu-id="51c5a-125">create</span></span>           | <span data-ttu-id="51c5a-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-126">[itemActionStat][]</span></span>      | <span data-ttu-id="51c5a-127">Estatísticas sobre as ações de **criação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="51c5a-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="51c5a-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-128">Read-only.</span></span>
| <span data-ttu-id="51c5a-129">edit</span><span class="sxs-lookup"><span data-stu-id="51c5a-129">edit</span></span>             | <span data-ttu-id="51c5a-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-130">[itemActionStat][]</span></span>      | <span data-ttu-id="51c5a-131">Estatísticas sobre as ações de **edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="51c5a-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="51c5a-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-132">Read-only.</span></span>
| <span data-ttu-id="51c5a-133">delete</span><span class="sxs-lookup"><span data-stu-id="51c5a-133">delete</span></span>           | <span data-ttu-id="51c5a-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-134">[itemActionStat][]</span></span>      | <span data-ttu-id="51c5a-135">Estatísticas sobre as ações de **exclusão** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="51c5a-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="51c5a-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-136">Read-only.</span></span>
| <span data-ttu-id="51c5a-137">move</span><span class="sxs-lookup"><span data-stu-id="51c5a-137">move</span></span>             | <span data-ttu-id="51c5a-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-138">[itemActionStat][]</span></span>      | <span data-ttu-id="51c5a-139">Estatísticas sobre as ações de **movimentação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="51c5a-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="51c5a-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-140">Read-only.</span></span>
| <span data-ttu-id="51c5a-141">Access</span><span class="sxs-lookup"><span data-stu-id="51c5a-141">access</span></span>           | <span data-ttu-id="51c5a-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-142">[itemActionStat][]</span></span>      | <span data-ttu-id="51c5a-143">Estatísticas sobre as ações de **acesso** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="51c5a-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="51c5a-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51c5a-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="51c5a-147">Relações</span><span class="sxs-lookup"><span data-stu-id="51c5a-147">Relationships</span></span>

| <span data-ttu-id="51c5a-148">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="51c5a-148">Relationship name</span></span> | <span data-ttu-id="51c5a-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="51c5a-149">Type</span></span>                        | <span data-ttu-id="51c5a-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="51c5a-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="51c5a-151">activities</span><span class="sxs-lookup"><span data-stu-id="51c5a-151">activities</span></span>        | <span data-ttu-id="51c5a-152">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="51c5a-152">[itemActivity][] collection</span></span> | <span data-ttu-id="51c5a-153">Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .</span><span class="sxs-lookup"><span data-stu-id="51c5a-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="51c5a-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51c5a-155">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": []
}
-->
