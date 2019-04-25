---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: Entidadeitemactivitystat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561891"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="59ee1-102">tipo de recurso Entidadeitemactivitystat</span><span class="sxs-lookup"><span data-stu-id="59ee1-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59ee1-103">O recurso **entidadeitemactivitystat** fornece informações sobre as atividades que aconteceram dentro de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="59ee1-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59ee1-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59ee1-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="59ee1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59ee1-105">Properties</span></span>

| <span data-ttu-id="59ee1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59ee1-106">Property</span></span>         | <span data-ttu-id="59ee1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="59ee1-107">Type</span></span>                    | <span data-ttu-id="59ee1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="59ee1-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="59ee1-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="59ee1-109">incompleteData</span></span>   | <span data-ttu-id="59ee1-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-110">[incompleteData][]</span></span>      | <span data-ttu-id="59ee1-111">Indica que as estatísticas neste intervalo são baseadas em dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="59ee1-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="59ee1-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-112">Read-only.</span></span>
| <span data-ttu-id="59ee1-113">isTendência</span><span class="sxs-lookup"><span data-stu-id="59ee1-113">isTrending</span></span>       | <span data-ttu-id="59ee1-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="59ee1-114">Boolean</span></span>                 | <span data-ttu-id="59ee1-115">Indica se o item é "Trending".</span><span class="sxs-lookup"><span data-stu-id="59ee1-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="59ee1-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-116">Read-only.</span></span>
| <span data-ttu-id="59ee1-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59ee1-117">startDateTime</span></span>    | <span data-ttu-id="59ee1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59ee1-118">DateTimeOffset</span></span>          | <span data-ttu-id="59ee1-119">Quando o intervalo é iniciado.</span><span class="sxs-lookup"><span data-stu-id="59ee1-119">When the interval starts.</span></span> <span data-ttu-id="59ee1-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-120">Read-only.</span></span>
| <span data-ttu-id="59ee1-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="59ee1-121">endDateTime</span></span>      | <span data-ttu-id="59ee1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59ee1-122">DateTimeOffset</span></span>          | <span data-ttu-id="59ee1-123">Quando o intervalo termina.</span><span class="sxs-lookup"><span data-stu-id="59ee1-123">When the interval ends.</span></span> <span data-ttu-id="59ee1-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-124">Read-only.</span></span>
| <span data-ttu-id="59ee1-125">create</span><span class="sxs-lookup"><span data-stu-id="59ee1-125">create</span></span>           | <span data-ttu-id="59ee1-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-126">[itemActionStat][]</span></span>      | <span data-ttu-id="59ee1-127">Estatísticas sobre as ações de **criação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="59ee1-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="59ee1-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-128">Read-only.</span></span>
| <span data-ttu-id="59ee1-129">edit</span><span class="sxs-lookup"><span data-stu-id="59ee1-129">edit</span></span>             | <span data-ttu-id="59ee1-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-130">[itemActionStat][]</span></span>      | <span data-ttu-id="59ee1-131">Estatísticas sobre as ações de **edição** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="59ee1-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="59ee1-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-132">Read-only.</span></span>
| <span data-ttu-id="59ee1-133">delete</span><span class="sxs-lookup"><span data-stu-id="59ee1-133">delete</span></span>           | <span data-ttu-id="59ee1-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-134">[itemActionStat][]</span></span>      | <span data-ttu-id="59ee1-135">Estatísticas sobre as ações de **exclusão** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="59ee1-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="59ee1-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-136">Read-only.</span></span>
| <span data-ttu-id="59ee1-137">move</span><span class="sxs-lookup"><span data-stu-id="59ee1-137">move</span></span>             | <span data-ttu-id="59ee1-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-138">[itemActionStat][]</span></span>      | <span data-ttu-id="59ee1-139">Estatísticas sobre as ações de **movimentação** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="59ee1-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="59ee1-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-140">Read-only.</span></span>
| <span data-ttu-id="59ee1-141">Access</span><span class="sxs-lookup"><span data-stu-id="59ee1-141">access</span></span>           | <span data-ttu-id="59ee1-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-142">[itemActionStat][]</span></span>      | <span data-ttu-id="59ee1-143">Estatísticas sobre as ações de **acesso** neste intervalo.</span><span class="sxs-lookup"><span data-stu-id="59ee1-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="59ee1-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59ee1-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="59ee1-147">Relações</span><span class="sxs-lookup"><span data-stu-id="59ee1-147">Relationships</span></span>

| <span data-ttu-id="59ee1-148">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="59ee1-148">Relationship name</span></span> | <span data-ttu-id="59ee1-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="59ee1-149">Type</span></span>                        | <span data-ttu-id="59ee1-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="59ee1-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="59ee1-151">activities</span><span class="sxs-lookup"><span data-stu-id="59ee1-151">activities</span></span>        | <span data-ttu-id="59ee1-152">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="59ee1-152">[itemActivity][] collection</span></span> | <span data-ttu-id="59ee1-153">Expõe as **actividades** representadas neste recurso **entidadeitemactivitystat** .</span><span class="sxs-lookup"><span data-stu-id="59ee1-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="59ee1-155">Comentários</span><span class="sxs-lookup"><span data-stu-id="59ee1-155">Remarks</span></span>

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
