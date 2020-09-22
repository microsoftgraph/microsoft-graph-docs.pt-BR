---
author: daspek
description: O recurso Entidadeitemactivitystat fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.
ms.date: 09/14/2017
title: Entidadeitemactivitystat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c21183911e111b2070d463f4552f913d93780493
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075655"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="7f038-103">tipo de recurso Entidadeitemactivitystat</span><span class="sxs-lookup"><span data-stu-id="7f038-103">itemActivityStat resource type</span></span>

<span data-ttu-id="7f038-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f038-105">O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="7f038-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f038-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f038-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7f038-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f038-107">Properties</span></span>

| <span data-ttu-id="7f038-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f038-108">Property</span></span>         | <span data-ttu-id="7f038-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f038-109">Type</span></span>                    | <span data-ttu-id="7f038-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f038-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="7f038-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="7f038-111">incompleteData</span></span>   | <span data-ttu-id="7f038-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="7f038-112">[incompleteData][]</span></span>      | <span data-ttu-id="7f038-113">Indica que as estatísticas neste intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="7f038-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="7f038-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-114">Read-only.</span></span>
| <span data-ttu-id="7f038-115">istendência</span><span class="sxs-lookup"><span data-stu-id="7f038-115">isTrending</span></span>       | <span data-ttu-id="7f038-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f038-116">Boolean</span></span>                 | <span data-ttu-id="7f038-117">Indica se o item é "Trending".</span><span class="sxs-lookup"><span data-stu-id="7f038-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="7f038-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-118">Read-only.</span></span>
| <span data-ttu-id="7f038-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f038-119">startDateTime</span></span>    | <span data-ttu-id="7f038-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f038-120">DateTimeOffset</span></span>          | <span data-ttu-id="7f038-121">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="7f038-121">When the interval starts.</span></span> <span data-ttu-id="7f038-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-122">Read-only.</span></span>
| <span data-ttu-id="7f038-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7f038-123">endDateTime</span></span>      | <span data-ttu-id="7f038-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f038-124">DateTimeOffset</span></span>          | <span data-ttu-id="7f038-125">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="7f038-125">When the interval ends.</span></span> <span data-ttu-id="7f038-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-126">Read-only.</span></span>
| <span data-ttu-id="7f038-127">create</span><span class="sxs-lookup"><span data-stu-id="7f038-127">create</span></span>           | <span data-ttu-id="7f038-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7f038-128">[itemActionStat][]</span></span>      | <span data-ttu-id="7f038-129">Estatísticas sobre as ações de **criação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="7f038-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="7f038-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-130">Read-only.</span></span>
| <span data-ttu-id="7f038-131">edit</span><span class="sxs-lookup"><span data-stu-id="7f038-131">edit</span></span>             | <span data-ttu-id="7f038-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7f038-132">[itemActionStat][]</span></span>      | <span data-ttu-id="7f038-133">Estatísticas sobre as ações de **edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="7f038-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="7f038-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-134">Read-only.</span></span>
| <span data-ttu-id="7f038-135">delete</span><span class="sxs-lookup"><span data-stu-id="7f038-135">delete</span></span>           | <span data-ttu-id="7f038-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7f038-136">[itemActionStat][]</span></span>      | <span data-ttu-id="7f038-137">Estatísticas sobre as ações de **exclusão** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="7f038-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="7f038-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-138">Read-only.</span></span>
| <span data-ttu-id="7f038-139">move</span><span class="sxs-lookup"><span data-stu-id="7f038-139">move</span></span>             | <span data-ttu-id="7f038-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7f038-140">[itemActionStat][]</span></span>      | <span data-ttu-id="7f038-141">Estatísticas sobre as ações de **movimentação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="7f038-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="7f038-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-142">Read-only.</span></span>
| <span data-ttu-id="7f038-143">Access</span><span class="sxs-lookup"><span data-stu-id="7f038-143">access</span></span>           | <span data-ttu-id="7f038-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="7f038-144">[itemActionStat][]</span></span>      | <span data-ttu-id="7f038-145">Estatísticas sobre as ações de **acesso** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="7f038-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="7f038-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7f038-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="7f038-149">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="7f038-149">Relationships</span></span>

| <span data-ttu-id="7f038-150">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="7f038-150">Relationship name</span></span> | <span data-ttu-id="7f038-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f038-151">Type</span></span>                        | <span data-ttu-id="7f038-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f038-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="7f038-153">activities</span><span class="sxs-lookup"><span data-stu-id="7f038-153">activities</span></span>        | <span data-ttu-id="7f038-154">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="7f038-154">[itemActivity][] collection</span></span> | <span data-ttu-id="7f038-155">Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .</span><span class="sxs-lookup"><span data-stu-id="7f038-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="7f038-157">Comentários</span><span class="sxs-lookup"><span data-stu-id="7f038-157">Remarks</span></span>

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


