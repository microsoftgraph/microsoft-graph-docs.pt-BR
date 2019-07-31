---
author: daspek
description: O recurso Entidadeitemactivitystat fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.
ms.date: 09/14/2017
title: Entidadeitemactivitystat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61c410d807869615ed35365743d1ae87b5b6e890
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967088"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="acb6d-103">tipo de recurso Entidadeitemactivitystat</span><span class="sxs-lookup"><span data-stu-id="acb6d-103">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acb6d-104">O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="acb6d-104">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acb6d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acb6d-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="acb6d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acb6d-106">Properties</span></span>

| <span data-ttu-id="acb6d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acb6d-107">Property</span></span>         | <span data-ttu-id="acb6d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="acb6d-108">Type</span></span>                    | <span data-ttu-id="acb6d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb6d-109">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="acb6d-110">incompleteData</span><span class="sxs-lookup"><span data-stu-id="acb6d-110">incompleteData</span></span>   | <span data-ttu-id="acb6d-111">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-111">[incompleteData][]</span></span>      | <span data-ttu-id="acb6d-112">Indica que as estatísticas neste intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="acb6d-112">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="acb6d-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-113">Read-only.</span></span>
| <span data-ttu-id="acb6d-114">istendência</span><span class="sxs-lookup"><span data-stu-id="acb6d-114">isTrending</span></span>       | <span data-ttu-id="acb6d-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="acb6d-115">Boolean</span></span>                 | <span data-ttu-id="acb6d-116">Indica se o item é "Trending".</span><span class="sxs-lookup"><span data-stu-id="acb6d-116">Indicates whether the item is "trending."</span></span> <span data-ttu-id="acb6d-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-117">Read-only.</span></span>
| <span data-ttu-id="acb6d-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="acb6d-118">startDateTime</span></span>    | <span data-ttu-id="acb6d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acb6d-119">DateTimeOffset</span></span>          | <span data-ttu-id="acb6d-120">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="acb6d-120">When the interval starts.</span></span> <span data-ttu-id="acb6d-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-121">Read-only.</span></span>
| <span data-ttu-id="acb6d-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="acb6d-122">endDateTime</span></span>      | <span data-ttu-id="acb6d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acb6d-123">DateTimeOffset</span></span>          | <span data-ttu-id="acb6d-124">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="acb6d-124">When the interval ends.</span></span> <span data-ttu-id="acb6d-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-125">Read-only.</span></span>
| <span data-ttu-id="acb6d-126">create</span><span class="sxs-lookup"><span data-stu-id="acb6d-126">create</span></span>           | <span data-ttu-id="acb6d-127">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-127">[itemActionStat][]</span></span>      | <span data-ttu-id="acb6d-128">Estatísticas sobre as ações de **criação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="acb6d-128">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="acb6d-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-129">Read-only.</span></span>
| <span data-ttu-id="acb6d-130">edit</span><span class="sxs-lookup"><span data-stu-id="acb6d-130">edit</span></span>             | <span data-ttu-id="acb6d-131">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-131">[itemActionStat][]</span></span>      | <span data-ttu-id="acb6d-132">Estatísticas sobre as ações de **edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="acb6d-132">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="acb6d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-133">Read-only.</span></span>
| <span data-ttu-id="acb6d-134">delete</span><span class="sxs-lookup"><span data-stu-id="acb6d-134">delete</span></span>           | <span data-ttu-id="acb6d-135">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-135">[itemActionStat][]</span></span>      | <span data-ttu-id="acb6d-136">Estatísticas sobre as ações de **exclusão** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="acb6d-136">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="acb6d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-137">Read-only.</span></span>
| <span data-ttu-id="acb6d-138">move</span><span class="sxs-lookup"><span data-stu-id="acb6d-138">move</span></span>             | <span data-ttu-id="acb6d-139">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-139">[itemActionStat][]</span></span>      | <span data-ttu-id="acb6d-140">Estatísticas sobre as ações de **movimentação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="acb6d-140">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="acb6d-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-141">Read-only.</span></span>
| <span data-ttu-id="acb6d-142">Access</span><span class="sxs-lookup"><span data-stu-id="acb6d-142">access</span></span>           | <span data-ttu-id="acb6d-143">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-143">[itemActionStat][]</span></span>      | <span data-ttu-id="acb6d-144">Estatísticas sobre as ações de **acesso** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="acb6d-144">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="acb6d-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acb6d-145">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="acb6d-148">Relações</span><span class="sxs-lookup"><span data-stu-id="acb6d-148">Relationships</span></span>

| <span data-ttu-id="acb6d-149">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="acb6d-149">Relationship name</span></span> | <span data-ttu-id="acb6d-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="acb6d-150">Type</span></span>                        | <span data-ttu-id="acb6d-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="acb6d-151">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="acb6d-152">activities</span><span class="sxs-lookup"><span data-stu-id="acb6d-152">activities</span></span>        | <span data-ttu-id="acb6d-153">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="acb6d-153">[itemActivity][] collection</span></span> | <span data-ttu-id="acb6d-154">Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .</span><span class="sxs-lookup"><span data-stu-id="acb6d-154">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="acb6d-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="acb6d-156">Remarks</span></span>

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
