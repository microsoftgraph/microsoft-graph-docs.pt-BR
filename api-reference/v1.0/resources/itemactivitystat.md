---
author: daspek
ms.author: dspektor
title: tipo de recurso Entidadeitemactivitystat
description: O objeto Entidadeitemactivitystat fornece informações sobre as atividades que ocorreram em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 80cc78486415f809082a2e9631dee86293e3389e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009321"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="73322-103">tipo de recurso Entidadeitemactivitystat</span><span class="sxs-lookup"><span data-stu-id="73322-103">itemActivityStat resource type</span></span>

<span data-ttu-id="73322-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73322-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73322-105">O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="73322-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="properties"></a><span data-ttu-id="73322-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73322-106">Properties</span></span>

| <span data-ttu-id="73322-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73322-107">Property</span></span>         | <span data-ttu-id="73322-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="73322-108">Type</span></span>                    | <span data-ttu-id="73322-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73322-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="73322-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="73322-110">incompleteData</span></span>   | <span data-ttu-id="73322-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="73322-111">[incompleteData][]</span></span>      | <span data-ttu-id="73322-112">Indica que as estatísticas neste intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="73322-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="73322-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-113">Read-only.</span></span>
| <span data-ttu-id="73322-114">istendência</span><span class="sxs-lookup"><span data-stu-id="73322-114">isTrending</span></span>       | <span data-ttu-id="73322-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="73322-115">Boolean</span></span>                 | <span data-ttu-id="73322-116">Indica se o item é "Trending".</span><span class="sxs-lookup"><span data-stu-id="73322-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="73322-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-117">Read-only.</span></span>
| <span data-ttu-id="73322-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73322-118">startDateTime</span></span>    | <span data-ttu-id="73322-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73322-119">DateTimeOffset</span></span>          | <span data-ttu-id="73322-120">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="73322-120">When the interval starts.</span></span> <span data-ttu-id="73322-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-121">Read-only.</span></span>
| <span data-ttu-id="73322-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="73322-122">endDateTime</span></span>      | <span data-ttu-id="73322-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73322-123">DateTimeOffset</span></span>          | <span data-ttu-id="73322-124">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="73322-124">When the interval ends.</span></span> <span data-ttu-id="73322-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-125">Read-only.</span></span>
| <span data-ttu-id="73322-126">create</span><span class="sxs-lookup"><span data-stu-id="73322-126">create</span></span>           | <span data-ttu-id="73322-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="73322-127">[itemActionStat][]</span></span>      | <span data-ttu-id="73322-128">Estatísticas sobre as ações de **criação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="73322-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="73322-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-129">Read-only.</span></span>
| <span data-ttu-id="73322-130">edit</span><span class="sxs-lookup"><span data-stu-id="73322-130">edit</span></span>             | <span data-ttu-id="73322-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="73322-131">[itemActionStat][]</span></span>      | <span data-ttu-id="73322-132">Estatísticas sobre as ações de **edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="73322-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="73322-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-133">Read-only.</span></span>
| <span data-ttu-id="73322-134">delete</span><span class="sxs-lookup"><span data-stu-id="73322-134">delete</span></span>           | <span data-ttu-id="73322-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="73322-135">[itemActionStat][]</span></span>      | <span data-ttu-id="73322-136">Estatísticas sobre as ações de **exclusão** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="73322-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="73322-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-137">Read-only.</span></span>
| <span data-ttu-id="73322-138">move</span><span class="sxs-lookup"><span data-stu-id="73322-138">move</span></span>             | <span data-ttu-id="73322-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="73322-139">[itemActionStat][]</span></span>      | <span data-ttu-id="73322-140">Estatísticas sobre as ações de **movimentação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="73322-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="73322-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-141">Read-only.</span></span>
| <span data-ttu-id="73322-142">Access</span><span class="sxs-lookup"><span data-stu-id="73322-142">access</span></span>           | <span data-ttu-id="73322-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="73322-143">[itemActionStat][]</span></span>      | <span data-ttu-id="73322-144">Estatísticas sobre as ações de **acesso** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="73322-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="73322-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73322-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="73322-148">Relações</span><span class="sxs-lookup"><span data-stu-id="73322-148">Relationships</span></span>

| <span data-ttu-id="73322-149">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="73322-149">Relationship name</span></span> | <span data-ttu-id="73322-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="73322-150">Type</span></span>                        | <span data-ttu-id="73322-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="73322-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="73322-152">activities</span><span class="sxs-lookup"><span data-stu-id="73322-152">activities</span></span>        | <span data-ttu-id="73322-153">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="73322-153">[itemActivity][] collection</span></span> | <span data-ttu-id="73322-154">Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .</span><span class="sxs-lookup"><span data-stu-id="73322-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="73322-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73322-156">JSON representation</span></span>

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

