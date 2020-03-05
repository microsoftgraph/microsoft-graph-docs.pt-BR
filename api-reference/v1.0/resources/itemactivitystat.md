---
author: daspek
ms.author: dspektor
title: tipo de recurso Entidadeitemactivitystat
description: O objeto Entidadeitemactivitystat fornece informações sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 11b19e4b953d4353382aec15071c6589b5bb23c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447665"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="0d9f8-103">tipo de recurso Entidadeitemactivitystat</span><span class="sxs-lookup"><span data-stu-id="0d9f8-103">itemActivityStat resource type</span></span>

<span data-ttu-id="0d9f8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0d9f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d9f8-105">O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="0d9f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d9f8-106">Properties</span></span>

| <span data-ttu-id="0d9f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d9f8-107">Property</span></span>         | <span data-ttu-id="0d9f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d9f8-108">Type</span></span>                    | <span data-ttu-id="0d9f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d9f8-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="0d9f8-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="0d9f8-110">incompleteData</span></span>   | <span data-ttu-id="0d9f8-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-111">[incompleteData][]</span></span>      | <span data-ttu-id="0d9f8-112">Indica que as estatísticas neste intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="0d9f8-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-113">Read-only.</span></span>
| <span data-ttu-id="0d9f8-114">istendência</span><span class="sxs-lookup"><span data-stu-id="0d9f8-114">isTrending</span></span>       | <span data-ttu-id="0d9f8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d9f8-115">Boolean</span></span>                 | <span data-ttu-id="0d9f8-116">Indica se o item é "Trending".</span><span class="sxs-lookup"><span data-stu-id="0d9f8-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="0d9f8-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-117">Read-only.</span></span>
| <span data-ttu-id="0d9f8-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d9f8-118">startDateTime</span></span>    | <span data-ttu-id="0d9f8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d9f8-119">DateTimeOffset</span></span>          | <span data-ttu-id="0d9f8-120">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-120">When the interval starts.</span></span> <span data-ttu-id="0d9f8-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-121">Read-only.</span></span>
| <span data-ttu-id="0d9f8-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d9f8-122">endDateTime</span></span>      | <span data-ttu-id="0d9f8-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d9f8-123">DateTimeOffset</span></span>          | <span data-ttu-id="0d9f8-124">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-124">When the interval ends.</span></span> <span data-ttu-id="0d9f8-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-125">Read-only.</span></span>
| <span data-ttu-id="0d9f8-126">create</span><span class="sxs-lookup"><span data-stu-id="0d9f8-126">create</span></span>           | <span data-ttu-id="0d9f8-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-127">[itemActionStat][]</span></span>      | <span data-ttu-id="0d9f8-128">Estatísticas sobre as ações de **criação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="0d9f8-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-129">Read-only.</span></span>
| <span data-ttu-id="0d9f8-130">edit</span><span class="sxs-lookup"><span data-stu-id="0d9f8-130">edit</span></span>             | <span data-ttu-id="0d9f8-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-131">[itemActionStat][]</span></span>      | <span data-ttu-id="0d9f8-132">Estatísticas sobre as ações de **edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="0d9f8-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-133">Read-only.</span></span>
| <span data-ttu-id="0d9f8-134">delete</span><span class="sxs-lookup"><span data-stu-id="0d9f8-134">delete</span></span>           | <span data-ttu-id="0d9f8-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-135">[itemActionStat][]</span></span>      | <span data-ttu-id="0d9f8-136">Estatísticas sobre as ações de **exclusão** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="0d9f8-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-137">Read-only.</span></span>
| <span data-ttu-id="0d9f8-138">move</span><span class="sxs-lookup"><span data-stu-id="0d9f8-138">move</span></span>             | <span data-ttu-id="0d9f8-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-139">[itemActionStat][]</span></span>      | <span data-ttu-id="0d9f8-140">Estatísticas sobre as ações de **movimentação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="0d9f8-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-141">Read-only.</span></span>
| <span data-ttu-id="0d9f8-142">Access</span><span class="sxs-lookup"><span data-stu-id="0d9f8-142">access</span></span>           | <span data-ttu-id="0d9f8-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-143">[itemActionStat][]</span></span>      | <span data-ttu-id="0d9f8-144">Estatísticas sobre as ações de **acesso** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="0d9f8-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d9f8-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="0d9f8-148">Relações</span><span class="sxs-lookup"><span data-stu-id="0d9f8-148">Relationships</span></span>

| <span data-ttu-id="0d9f8-149">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="0d9f8-149">Relationship name</span></span> | <span data-ttu-id="0d9f8-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d9f8-150">Type</span></span>                        | <span data-ttu-id="0d9f8-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d9f8-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="0d9f8-152">activities</span><span class="sxs-lookup"><span data-stu-id="0d9f8-152">activities</span></span>        | <span data-ttu-id="0d9f8-153">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="0d9f8-153">[itemActivity][] collection</span></span> | <span data-ttu-id="0d9f8-154">Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .</span><span class="sxs-lookup"><span data-stu-id="0d9f8-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0d9f8-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d9f8-156">JSON representation</span></span>

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
