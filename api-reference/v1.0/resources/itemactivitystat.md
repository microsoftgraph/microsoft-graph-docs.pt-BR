---
author: daspek
title: Tipo de recurso itemActivityStat
description: O objeto ItemActivityStat fornece informações sobre atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a33453fc884fc6dba7bd5b8fbcf4edc0261c11cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238677"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="706bb-103">Tipo de recurso itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="706bb-103">itemActivityStat resource type</span></span>

<span data-ttu-id="706bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="706bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="706bb-105">O **recurso itemActivityStat** fornece informações sobre atividades que ocorreram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="706bb-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="706bb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="706bb-106">Properties</span></span>

| <span data-ttu-id="706bb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="706bb-107">Property</span></span>         | <span data-ttu-id="706bb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="706bb-108">Type</span></span>                    | <span data-ttu-id="706bb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="706bb-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="706bb-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="706bb-110">incompleteData</span></span>   | <span data-ttu-id="706bb-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="706bb-111">[incompleteData][]</span></span>      | <span data-ttu-id="706bb-112">Indica que as estatísticas nesse intervalo se baseiam em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="706bb-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="706bb-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-113">Read-only.</span></span>
| <span data-ttu-id="706bb-114">isTrending</span><span class="sxs-lookup"><span data-stu-id="706bb-114">isTrending</span></span>       | <span data-ttu-id="706bb-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="706bb-115">Boolean</span></span>                 | <span data-ttu-id="706bb-116">Indica se o item é "trending".</span><span class="sxs-lookup"><span data-stu-id="706bb-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="706bb-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-117">Read-only.</span></span>
| <span data-ttu-id="706bb-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="706bb-118">startDateTime</span></span>    | <span data-ttu-id="706bb-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="706bb-119">DateTimeOffset</span></span>          | <span data-ttu-id="706bb-120">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="706bb-120">When the interval starts.</span></span> <span data-ttu-id="706bb-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-121">Read-only.</span></span>
| <span data-ttu-id="706bb-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="706bb-122">endDateTime</span></span>      | <span data-ttu-id="706bb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="706bb-123">DateTimeOffset</span></span>          | <span data-ttu-id="706bb-124">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="706bb-124">When the interval ends.</span></span> <span data-ttu-id="706bb-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-125">Read-only.</span></span>
| <span data-ttu-id="706bb-126">create</span><span class="sxs-lookup"><span data-stu-id="706bb-126">create</span></span>           | <span data-ttu-id="706bb-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="706bb-127">[itemActionStat][]</span></span>      | <span data-ttu-id="706bb-128">Estatísticas sobre as ações **de** criação nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="706bb-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="706bb-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-129">Read-only.</span></span>
| <span data-ttu-id="706bb-130">edit</span><span class="sxs-lookup"><span data-stu-id="706bb-130">edit</span></span>             | <span data-ttu-id="706bb-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="706bb-131">[itemActionStat][]</span></span>      | <span data-ttu-id="706bb-132">Estatísticas sobre as ações **de edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="706bb-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="706bb-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-133">Read-only.</span></span>
| <span data-ttu-id="706bb-134">delete</span><span class="sxs-lookup"><span data-stu-id="706bb-134">delete</span></span>           | <span data-ttu-id="706bb-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="706bb-135">[itemActionStat][]</span></span>      | <span data-ttu-id="706bb-136">Estatísticas sobre as ações **de exclusão** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="706bb-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="706bb-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-137">Read-only.</span></span>
| <span data-ttu-id="706bb-138">move</span><span class="sxs-lookup"><span data-stu-id="706bb-138">move</span></span>             | <span data-ttu-id="706bb-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="706bb-139">[itemActionStat][]</span></span>      | <span data-ttu-id="706bb-140">Estatísticas sobre as ações **de** movimentação nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="706bb-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="706bb-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-141">Read-only.</span></span>
| <span data-ttu-id="706bb-142">access</span><span class="sxs-lookup"><span data-stu-id="706bb-142">access</span></span>           | <span data-ttu-id="706bb-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="706bb-143">[itemActionStat][]</span></span>      | <span data-ttu-id="706bb-144">Estatísticas sobre as ações **de** acesso neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="706bb-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="706bb-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706bb-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="706bb-148">Relações</span><span class="sxs-lookup"><span data-stu-id="706bb-148">Relationships</span></span>

| <span data-ttu-id="706bb-149">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="706bb-149">Relationship name</span></span> | <span data-ttu-id="706bb-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="706bb-150">Type</span></span>                        | <span data-ttu-id="706bb-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="706bb-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="706bb-152">activities</span><span class="sxs-lookup"><span data-stu-id="706bb-152">activities</span></span>        | <span data-ttu-id="706bb-153">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="706bb-153">[itemActivity][] collection</span></span> | <span data-ttu-id="706bb-154">Expõe o **itemActivities** representado neste **recurso itemActivityStat.**</span><span class="sxs-lookup"><span data-stu-id="706bb-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="706bb-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="706bb-156">JSON representation</span></span>

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

