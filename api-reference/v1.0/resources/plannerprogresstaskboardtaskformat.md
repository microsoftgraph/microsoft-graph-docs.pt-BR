---
title: tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0c08fed11b53610c06b27b9fa9d5e898b2f0620d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037357"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="ce131-104">tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ce131-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="ce131-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce131-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce131-106">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída).</span><span class="sxs-lookup"><span data-stu-id="ce131-106">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="ce131-107">Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="ce131-107">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="ce131-108">Methods</span><span class="sxs-lookup"><span data-stu-id="ce131-108">Methods</span></span>

| <span data-ttu-id="ce131-109">Método</span><span class="sxs-lookup"><span data-stu-id="ce131-109">Method</span></span>           | <span data-ttu-id="ce131-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce131-110">Return Type</span></span>    |<span data-ttu-id="ce131-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce131-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce131-112">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ce131-112">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="ce131-113">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ce131-113">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="ce131-114">Leia as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="ce131-114">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="ce131-115">Atualização</span><span class="sxs-lookup"><span data-stu-id="ce131-115">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="ce131-116">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ce131-116">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="ce131-117">Atualize o objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="ce131-117">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce131-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce131-118">Properties</span></span>
| <span data-ttu-id="ce131-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce131-119">Property</span></span>     | <span data-ttu-id="ce131-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce131-120">Type</span></span>   |<span data-ttu-id="ce131-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce131-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce131-122">id</span><span class="sxs-lookup"><span data-stu-id="ce131-122">id</span></span>|<span data-ttu-id="ce131-123">String</span><span class="sxs-lookup"><span data-stu-id="ce131-123">String</span></span>| <span data-ttu-id="ce131-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce131-124">Read-only.</span></span> <span data-ttu-id="ce131-125">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce131-125">ID of the resource.</span></span> <span data-ttu-id="ce131-126">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ce131-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ce131-127">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="ce131-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ce131-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="ce131-128">orderHint</span></span>|<span data-ttu-id="ce131-129">String</span><span class="sxs-lookup"><span data-stu-id="ce131-129">String</span></span>|<span data-ttu-id="ce131-130">O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="ce131-130">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="ce131-131">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ce131-131">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce131-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ce131-132">Relationships</span></span>
<span data-ttu-id="ce131-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce131-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ce131-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce131-134">JSON representation</span></span>
<span data-ttu-id="ce131-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce131-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

