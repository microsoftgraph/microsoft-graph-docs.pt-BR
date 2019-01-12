---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955132"
---
# <a name="planner-resource-type"></a><span data-ttu-id="88d29-105">Tipo de recurso planner</span><span class="sxs-lookup"><span data-stu-id="88d29-105">planner resource type</span></span>

<span data-ttu-id="88d29-p102">O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="88d29-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="88d29-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="88d29-109">Methods</span></span>

| <span data-ttu-id="88d29-110">Método</span><span class="sxs-lookup"><span data-stu-id="88d29-110">Method</span></span>           | <span data-ttu-id="88d29-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="88d29-111">Return Type</span></span>    |<span data-ttu-id="88d29-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d29-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88d29-113">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="88d29-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="88d29-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="88d29-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="88d29-115">Crie um novo **plannerBucket** ao postar na coleção de buckets.</span><span class="sxs-lookup"><span data-stu-id="88d29-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="88d29-116">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="88d29-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="88d29-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="88d29-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="88d29-118">Crie um novo **plannerPlan** ao postar na coleção de planos.</span><span class="sxs-lookup"><span data-stu-id="88d29-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="88d29-119">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="88d29-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="88d29-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="88d29-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="88d29-121">Crie um novo **plannerTask** ao postar na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="88d29-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88d29-122">Relações</span><span class="sxs-lookup"><span data-stu-id="88d29-122">Relationships</span></span>
| <span data-ttu-id="88d29-123">Relação</span><span class="sxs-lookup"><span data-stu-id="88d29-123">Relationship</span></span> | <span data-ttu-id="88d29-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="88d29-124">Type</span></span>   |<span data-ttu-id="88d29-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d29-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88d29-126">buckets</span><span class="sxs-lookup"><span data-stu-id="88d29-126">buckets</span></span>|<span data-ttu-id="88d29-127">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="88d29-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="88d29-p103">Somente leitura. Anulável. Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="88d29-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="88d29-131">plans</span><span class="sxs-lookup"><span data-stu-id="88d29-131">plans</span></span>|<span data-ttu-id="88d29-132">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="88d29-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="88d29-p104">Somente leitura. Anulável. Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="88d29-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="88d29-136">tarefas</span><span class="sxs-lookup"><span data-stu-id="88d29-136">tasks</span></span>|<span data-ttu-id="88d29-137">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="88d29-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="88d29-p105">Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="88d29-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88d29-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88d29-141">JSON representation</span></span>
<span data-ttu-id="88d29-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88d29-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="88d29-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88d29-143">Example</span></span>

<span data-ttu-id="88d29-144">O recurso de **Planejador** estará disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="88d29-144">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
