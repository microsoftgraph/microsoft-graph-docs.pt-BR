---
title: tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9e690c13086cb0c40905255678f8b7134521e2f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533978"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="03216-104">tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="03216-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="03216-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03216-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03216-106">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída).</span><span class="sxs-lookup"><span data-stu-id="03216-106">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="03216-107">Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="03216-107">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="03216-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="03216-108">Methods</span></span>

| <span data-ttu-id="03216-109">Método</span><span class="sxs-lookup"><span data-stu-id="03216-109">Method</span></span>           | <span data-ttu-id="03216-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03216-110">Return Type</span></span>    |<span data-ttu-id="03216-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="03216-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03216-112">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="03216-112">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="03216-113">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="03216-113">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="03216-114">Leia as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="03216-114">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="03216-115">Atualizar</span><span class="sxs-lookup"><span data-stu-id="03216-115">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="03216-116">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="03216-116">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="03216-117">Atualize o objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="03216-117">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="03216-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03216-118">Properties</span></span>
| <span data-ttu-id="03216-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03216-119">Property</span></span>     | <span data-ttu-id="03216-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="03216-120">Type</span></span>   |<span data-ttu-id="03216-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="03216-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03216-122">id</span><span class="sxs-lookup"><span data-stu-id="03216-122">id</span></span>|<span data-ttu-id="03216-123">String</span><span class="sxs-lookup"><span data-stu-id="03216-123">String</span></span>| <span data-ttu-id="03216-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03216-124">Read-only.</span></span> <span data-ttu-id="03216-125">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="03216-125">ID of the resource.</span></span> <span data-ttu-id="03216-126">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="03216-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="03216-127">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="03216-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="03216-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="03216-128">orderHint</span></span>|<span data-ttu-id="03216-129">String</span><span class="sxs-lookup"><span data-stu-id="03216-129">String</span></span>|<span data-ttu-id="03216-130">O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="03216-130">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="03216-131">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="03216-131">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="03216-132">Relações</span><span class="sxs-lookup"><span data-stu-id="03216-132">Relationships</span></span>
<span data-ttu-id="03216-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03216-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="03216-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03216-134">JSON representation</span></span>
<span data-ttu-id="03216-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03216-135">Here is a JSON representation of the resource.</span></span>

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
