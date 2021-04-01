---
title: Tipo de recurso plannerPlanContainer
description: Representa um contêiner para um plannerPlan. O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: acb7a85683bc94795953e524ee9630d6cfc01f24
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473882"
---
# <a name="plannerplancontainer-resource-type"></a><span data-ttu-id="67570-104">Tipo de recurso plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="67570-104">plannerPlanContainer resource type</span></span>

<span data-ttu-id="67570-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67570-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67570-106">Representa um contêiner para um [plannerPlan](plannerPlan.md).</span><span class="sxs-lookup"><span data-stu-id="67570-106">Represents a container for a [plannerPlan](plannerPlan.md).</span></span> <span data-ttu-id="67570-107">O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano.</span><span class="sxs-lookup"><span data-stu-id="67570-107">The container is a resource that specifies authorization rules and the lifetime of the plan.</span></span> <span data-ttu-id="67570-108">Isso significa que somente as pessoas que estão autorizadas a trabalhar com o recurso que contém o plano poderão trabalhar com o plano e as tarefas dentro dele.</span><span class="sxs-lookup"><span data-stu-id="67570-108">This means that only the people who are authorized to work with the resource containing the plan will be able to work with the plan and the tasks within it.</span></span> <span data-ttu-id="67570-109">Quando o recurso que contém é excluído, os planos contidos também são excluídos.</span><span class="sxs-lookup"><span data-stu-id="67570-109">When the containing resource is deleted, the contained plans are also deleted.</span></span> <span data-ttu-id="67570-110">As propriedades **do plannerPlanContainer** não podem ser alteradas após a criação do plano.</span><span class="sxs-lookup"><span data-stu-id="67570-110">Properties of **plannerPlanContainer** cannot be changed after the plan is created.</span></span>

<span data-ttu-id="67570-111">No momento, o Planner dá suporte aos tipos de contêiner listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="67570-111">Planner currently supports the container types listed in the following table.</span></span> <span data-ttu-id="67570-112">Ao criar um plano, a **propriedade containerUrl** deve ser especificada com o caminho do recurso identificado na tabela.</span><span class="sxs-lookup"><span data-stu-id="67570-112">When creating a plan, the **containerUrl** property must be specified with the path of the resource identified in the table.</span></span>

|<span data-ttu-id="67570-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="67570-113">Type</span></span>|<span data-ttu-id="67570-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="67570-114">Description</span></span>|<span data-ttu-id="67570-115">Caminho para o recurso</span><span class="sxs-lookup"><span data-stu-id="67570-115">Path to the resource</span></span>|
|----|-----------|--------------------|
|<span data-ttu-id="67570-116">group</span><span class="sxs-lookup"><span data-stu-id="67570-116">group</span></span>| <span data-ttu-id="67570-117">O plano está contido em um [grupo](group.md).</span><span class="sxs-lookup"><span data-stu-id="67570-117">Plan is contained by a [group](group.md).</span></span>| <span data-ttu-id="67570-118"> https://graph.microsoft.com/beta/groups/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="67570-118">https://graph.microsoft.com/beta/groups/&lt;id&gt;</span></span>|
|<span data-ttu-id="67570-119">roster</span><span class="sxs-lookup"><span data-stu-id="67570-119">roster</span></span>| <span data-ttu-id="67570-120">O plano está contido por [um plannerRoster](plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="67570-120">Plan is contained by a [plannerRoster](plannerroster.md)</span></span> | <span data-ttu-id="67570-121"> https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="67570-121">https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;</span></span>|

## <a name="properties"></a><span data-ttu-id="67570-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67570-122">Properties</span></span>
|<span data-ttu-id="67570-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67570-123">Property</span></span>|<span data-ttu-id="67570-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="67570-124">Type</span></span>|<span data-ttu-id="67570-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="67570-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67570-126">containerId</span><span class="sxs-lookup"><span data-stu-id="67570-126">containerId</span></span>|<span data-ttu-id="67570-127">String</span><span class="sxs-lookup"><span data-stu-id="67570-127">String</span></span>|<span data-ttu-id="67570-128">O identificador do recurso que contém o plano.</span><span class="sxs-lookup"><span data-stu-id="67570-128">The identifier of the resource that contains the plan.</span></span>|
|<span data-ttu-id="67570-129">tipo</span><span class="sxs-lookup"><span data-stu-id="67570-129">type</span></span>|<span data-ttu-id="67570-130">plannerContainerType</span><span class="sxs-lookup"><span data-stu-id="67570-130">plannerContainerType</span></span>| <span data-ttu-id="67570-131">O tipo do recurso que contém o plano.</span><span class="sxs-lookup"><span data-stu-id="67570-131">The type of the resource that contains the plan.</span></span> <span data-ttu-id="67570-132">Consulte a tabela anterior para tipos com suporte.</span><span class="sxs-lookup"><span data-stu-id="67570-132">See the previous table for supported types.</span></span> <span data-ttu-id="67570-133">Os valores possíveis são: `group`, `roster`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="67570-133">Possible values are: `group`, `roster`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="67570-134">url</span><span class="sxs-lookup"><span data-stu-id="67570-134">url</span></span>|<span data-ttu-id="67570-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67570-135">String</span></span>|<span data-ttu-id="67570-136">A URL canônica completa do contêiner.</span><span class="sxs-lookup"><span data-stu-id="67570-136">The full canonical URL of the container.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67570-137">Relações</span><span class="sxs-lookup"><span data-stu-id="67570-137">Relationships</span></span>
<span data-ttu-id="67570-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67570-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67570-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67570-139">JSON representation</span></span>
<span data-ttu-id="67570-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67570-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "url": "String",
  "containerId": "String",
  "type": "String"
}
```

