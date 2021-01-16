---
title: Tipo de recurso plannerPlanContainer
description: Representa um contêiner para um plannerPlan. O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8b3abb10892077159e6f02c33a31d501a75dba2a
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883225"
---
# <a name="plannerplancontainer-resource-type"></a><span data-ttu-id="81e1d-104">Tipo de recurso plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="81e1d-104">plannerPlanContainer resource type</span></span>

<span data-ttu-id="81e1d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81e1d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81e1d-106">Representa um contêiner para um [plannerPlan](plannerPlan.md).</span><span class="sxs-lookup"><span data-stu-id="81e1d-106">Represents a container for a [plannerPlan](plannerPlan.md).</span></span> <span data-ttu-id="81e1d-107">O contêiner é um recurso que especifica as regras de autorização e o tempo de vida do plano.</span><span class="sxs-lookup"><span data-stu-id="81e1d-107">The container is a resource that specifies authorization rules and the lifetime of the plan.</span></span> <span data-ttu-id="81e1d-108">Isso significa que somente as pessoas autorizadas a trabalhar com o recurso que contém o plano poderão trabalhar com o plano e as tarefas dentro dele.</span><span class="sxs-lookup"><span data-stu-id="81e1d-108">This means that only the people who are authorized to work with the resource containing the plan will be able to work with the plan and the tasks within it.</span></span> <span data-ttu-id="81e1d-109">Quando o recurso que contém é excluído, os planos contidos também são excluídos.</span><span class="sxs-lookup"><span data-stu-id="81e1d-109">When the containing resource is deleted, the contained plans are also deleted.</span></span> <span data-ttu-id="81e1d-110">As propriedades **de plannerPlanContainer** não podem ser alteradas depois que o plano é criado.</span><span class="sxs-lookup"><span data-stu-id="81e1d-110">Properties of **plannerPlanContainer** cannot be changed after the plan is created.</span></span>

<span data-ttu-id="81e1d-111">Atualmente, o Planner oferece suporte aos tipos de contêiner listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="81e1d-111">Planner currently supports the container types listed in the following table.</span></span> <span data-ttu-id="81e1d-112">Ao criar um plano, a **propriedade containerUrl** deve ser especificada com o caminho do recurso identificado na tabela.</span><span class="sxs-lookup"><span data-stu-id="81e1d-112">When creating a plan, the **containerUrl** property must be specified with the path of the resource identified in the table.</span></span>

|<span data-ttu-id="81e1d-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="81e1d-113">Type</span></span>|<span data-ttu-id="81e1d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="81e1d-114">Description</span></span>|<span data-ttu-id="81e1d-115">Caminho para o recurso</span><span class="sxs-lookup"><span data-stu-id="81e1d-115">Path to the resource</span></span>|
|----|-----------|--------------------|
|<span data-ttu-id="81e1d-116">group</span><span class="sxs-lookup"><span data-stu-id="81e1d-116">group</span></span>| <span data-ttu-id="81e1d-117">O plano está contido em um grupo.</span><span class="sxs-lookup"><span data-stu-id="81e1d-117">Plan is contained by a group.</span></span>| <span data-ttu-id="81e1d-118"> https://graph.microsoft.com/v1.0/groups/&lt;id&gt;</span><span class="sxs-lookup"><span data-stu-id="81e1d-118">https://graph.microsoft.com/v1.0/groups/&lt;id&gt;</span></span>|

## <a name="properties"></a><span data-ttu-id="81e1d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81e1d-119">Properties</span></span>
|<span data-ttu-id="81e1d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81e1d-120">Property</span></span>|<span data-ttu-id="81e1d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="81e1d-121">Type</span></span>|<span data-ttu-id="81e1d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81e1d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e1d-123">containerId</span><span class="sxs-lookup"><span data-stu-id="81e1d-123">containerId</span></span>|<span data-ttu-id="81e1d-124">String</span><span class="sxs-lookup"><span data-stu-id="81e1d-124">String</span></span>|<span data-ttu-id="81e1d-125">O identificador do recurso que contém o plano.</span><span class="sxs-lookup"><span data-stu-id="81e1d-125">The identifier of the resource that contains the plan.</span></span>|
|<span data-ttu-id="81e1d-126">type</span><span class="sxs-lookup"><span data-stu-id="81e1d-126">type</span></span>|<span data-ttu-id="81e1d-127">plannerContainerType</span><span class="sxs-lookup"><span data-stu-id="81e1d-127">plannerContainerType</span></span>| <span data-ttu-id="81e1d-128">O tipo do recurso que contém o plano.</span><span class="sxs-lookup"><span data-stu-id="81e1d-128">The type of the resource that contains the plan.</span></span> <span data-ttu-id="81e1d-129">Consulte a tabela anterior para ver os tipos com suporte.</span><span class="sxs-lookup"><span data-stu-id="81e1d-129">See the previous table for supported types.</span></span> <span data-ttu-id="81e1d-130">Os valores possíveis são: `group` e `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="81e1d-130">Possible values are: `group`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="81e1d-131">url</span><span class="sxs-lookup"><span data-stu-id="81e1d-131">url</span></span>|<span data-ttu-id="81e1d-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81e1d-132">String</span></span>|<span data-ttu-id="81e1d-133">A URL canônica completa do contêiner.</span><span class="sxs-lookup"><span data-stu-id="81e1d-133">The full canonical URL of the container.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81e1d-134">Relações</span><span class="sxs-lookup"><span data-stu-id="81e1d-134">Relationships</span></span>
<span data-ttu-id="81e1d-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81e1d-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81e1d-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81e1d-136">JSON representation</span></span>
<span data-ttu-id="81e1d-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81e1d-137">The following is a JSON representation of the resource.</span></span>
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

