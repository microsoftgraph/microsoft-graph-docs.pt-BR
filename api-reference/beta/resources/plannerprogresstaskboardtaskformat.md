---
title: tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7be6483f127910224b05e05fdf885780d8767176
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521668"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="0f010-104">tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0f010-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="0f010-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0f010-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f010-106">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com as colunas não iniciadas, em andamento e concluída).</span><span class="sxs-lookup"><span data-stu-id="0f010-106">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="0f010-107">Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="0f010-107">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="0f010-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f010-108">Methods</span></span>

| <span data-ttu-id="0f010-109">Método</span><span class="sxs-lookup"><span data-stu-id="0f010-109">Method</span></span>           | <span data-ttu-id="0f010-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f010-110">Return Type</span></span>    |<span data-ttu-id="0f010-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f010-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f010-112">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0f010-112">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="0f010-113">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0f010-113">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="0f010-114">Leia as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="0f010-114">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="0f010-115">Update</span><span class="sxs-lookup"><span data-stu-id="0f010-115">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="0f010-116">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0f010-116">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="0f010-117">Atualize o objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="0f010-117">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f010-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f010-118">Properties</span></span>
| <span data-ttu-id="0f010-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f010-119">Property</span></span>     | <span data-ttu-id="0f010-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f010-120">Type</span></span>   |<span data-ttu-id="0f010-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f010-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f010-122">id</span><span class="sxs-lookup"><span data-stu-id="0f010-122">id</span></span>|<span data-ttu-id="0f010-123">String</span><span class="sxs-lookup"><span data-stu-id="0f010-123">String</span></span>| <span data-ttu-id="0f010-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f010-124">Read-only.</span></span> <span data-ttu-id="0f010-125">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f010-125">ID of the resource.</span></span> <span data-ttu-id="0f010-126">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0f010-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0f010-127">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="0f010-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0f010-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="0f010-128">orderHint</span></span>|<span data-ttu-id="0f010-129">String</span><span class="sxs-lookup"><span data-stu-id="0f010-129">String</span></span>|<span data-ttu-id="0f010-130">O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="0f010-130">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="0f010-131">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="0f010-131">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f010-132">Relações</span><span class="sxs-lookup"><span data-stu-id="0f010-132">Relationships</span></span>
<span data-ttu-id="0f010-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f010-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0f010-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f010-134">JSON representation</span></span>
<span data-ttu-id="0f010-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f010-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
