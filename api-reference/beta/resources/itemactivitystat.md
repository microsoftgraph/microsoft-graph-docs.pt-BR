---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: d0917d0100d33abee1095e2a7d06a4732d382937
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854247"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="9eb68-102">tipo de recurso de itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="9eb68-102">itemActivityStat resource type</span></span>

> <span data-ttu-id="9eb68-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9eb68-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9eb68-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9eb68-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9eb68-105">O recurso de **itemActivityStat** fornece informações sobre atividades realizadas dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="9eb68-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9eb68-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9eb68-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9eb68-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9eb68-107">Properties</span></span>

| <span data-ttu-id="9eb68-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9eb68-108">Property</span></span>         | <span data-ttu-id="9eb68-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eb68-109">Type</span></span>                    | <span data-ttu-id="9eb68-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eb68-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="9eb68-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="9eb68-111">incompleteData</span></span>   | <span data-ttu-id="9eb68-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-112">[incompleteData][]</span></span>      | <span data-ttu-id="9eb68-113">Indica que as estatísticas nesse intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="9eb68-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="9eb68-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-114">Read-only.</span></span>
| <span data-ttu-id="9eb68-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="9eb68-115">isTrending</span></span>       | <span data-ttu-id="9eb68-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="9eb68-116">Boolean</span></span>                 | <span data-ttu-id="9eb68-117">Indica se o item é "tendências".</span><span class="sxs-lookup"><span data-stu-id="9eb68-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="9eb68-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-118">Read-only.</span></span>
| <span data-ttu-id="9eb68-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9eb68-119">startDateTime</span></span>    | <span data-ttu-id="9eb68-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eb68-120">DateTimeOffset</span></span>          | <span data-ttu-id="9eb68-121">Quando o intervalo for iniciado.</span><span class="sxs-lookup"><span data-stu-id="9eb68-121">When the interval starts.</span></span> <span data-ttu-id="9eb68-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-122">Read-only.</span></span>
| <span data-ttu-id="9eb68-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9eb68-123">endDateTime</span></span>      | <span data-ttu-id="9eb68-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eb68-124">DateTimeOffset</span></span>          | <span data-ttu-id="9eb68-125">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="9eb68-125">When the interval ends.</span></span> <span data-ttu-id="9eb68-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-126">Read-only.</span></span>
| <span data-ttu-id="9eb68-127">create</span><span class="sxs-lookup"><span data-stu-id="9eb68-127">create</span></span>           | <span data-ttu-id="9eb68-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-128">[itemActionStat][]</span></span>      | <span data-ttu-id="9eb68-129">Estatísticas sobre as ações **criar** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9eb68-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="9eb68-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-130">Read-only.</span></span>
| <span data-ttu-id="9eb68-131">edit</span><span class="sxs-lookup"><span data-stu-id="9eb68-131">edit</span></span>             | <span data-ttu-id="9eb68-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-132">[itemActionStat][]</span></span>      | <span data-ttu-id="9eb68-133">Estatísticas sobre as ações de **Editar** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9eb68-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="9eb68-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-134">Read-only.</span></span>
| <span data-ttu-id="9eb68-135">delete</span><span class="sxs-lookup"><span data-stu-id="9eb68-135">delete</span></span>           | <span data-ttu-id="9eb68-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-136">[itemActionStat][]</span></span>      | <span data-ttu-id="9eb68-137">Estatísticas sobre as ações **Excluir** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9eb68-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="9eb68-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-138">Read-only.</span></span>
| <span data-ttu-id="9eb68-139">move</span><span class="sxs-lookup"><span data-stu-id="9eb68-139">move</span></span>             | <span data-ttu-id="9eb68-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-140">[itemActionStat][]</span></span>      | <span data-ttu-id="9eb68-141">Estatísticas sobre as ações de **Mover** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9eb68-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="9eb68-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-142">Read-only.</span></span>
| <span data-ttu-id="9eb68-143">acesso</span><span class="sxs-lookup"><span data-stu-id="9eb68-143">access</span></span>           | <span data-ttu-id="9eb68-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-144">[itemActionStat][]</span></span>      | <span data-ttu-id="9eb68-145">Estatísticas sobre as ações de **acesso** nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9eb68-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="9eb68-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9eb68-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="9eb68-149">Relações</span><span class="sxs-lookup"><span data-stu-id="9eb68-149">Relationships</span></span>

| <span data-ttu-id="9eb68-150">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="9eb68-150">Relationship name</span></span> | <span data-ttu-id="9eb68-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="9eb68-151">Type</span></span>                        | <span data-ttu-id="9eb68-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="9eb68-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="9eb68-153">activities</span><span class="sxs-lookup"><span data-stu-id="9eb68-153">activities</span></span>        | <span data-ttu-id="9eb68-154">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="9eb68-154">[itemActivity][] collection</span></span> | <span data-ttu-id="9eb68-155">Expõe **itemActivities** representados neste recurso **itemActivityStat** .</span><span class="sxs-lookup"><span data-stu-id="9eb68-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="9eb68-157">Comentários</span><span class="sxs-lookup"><span data-stu-id="9eb68-157">Remarks</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
