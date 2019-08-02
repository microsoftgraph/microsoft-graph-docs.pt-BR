---
title: tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com colunas para não iniciado , Em andamento e concluído). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6b92cbd231e0cd194b49c11c25d24b93933abbe7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035172"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="ed2c9-104">tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ed2c9-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="ed2c9-105">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com colunas para não iniciado , Em andamento e concluído).</span><span class="sxs-lookup"><span data-stu-id="ed2c9-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="ed2c9-106">Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="ed2c9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed2c9-107">Methods</span></span>

| <span data-ttu-id="ed2c9-108">Método</span><span class="sxs-lookup"><span data-stu-id="ed2c9-108">Method</span></span>           | <span data-ttu-id="ed2c9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed2c9-109">Return Type</span></span>    |<span data-ttu-id="ed2c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed2c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed2c9-111">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ed2c9-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="ed2c9-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ed2c9-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="ed2c9-113">Leia as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="ed2c9-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="ed2c9-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="ed2c9-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="ed2c9-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ed2c9-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="ed2c9-116">Atualize o objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="ed2c9-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed2c9-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed2c9-117">Properties</span></span>
| <span data-ttu-id="ed2c9-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed2c9-118">Property</span></span>     | <span data-ttu-id="ed2c9-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed2c9-119">Type</span></span>   |<span data-ttu-id="ed2c9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed2c9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed2c9-121">id</span><span class="sxs-lookup"><span data-stu-id="ed2c9-121">id</span></span>|<span data-ttu-id="ed2c9-122">String</span><span class="sxs-lookup"><span data-stu-id="ed2c9-122">String</span></span>| <span data-ttu-id="ed2c9-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-123">Read-only.</span></span> <span data-ttu-id="ed2c9-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-124">ID of the resource.</span></span> <span data-ttu-id="ed2c9-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ed2c9-126">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ed2c9-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="ed2c9-127">orderHint</span></span>|<span data-ttu-id="ed2c9-128">String</span><span class="sxs-lookup"><span data-stu-id="ed2c9-128">String</span></span>|<span data-ttu-id="ed2c9-129">O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-129">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="ed2c9-130">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="ed2c9-130">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed2c9-131">Relações</span><span class="sxs-lookup"><span data-stu-id="ed2c9-131">Relationships</span></span>
<span data-ttu-id="ed2c9-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed2c9-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed2c9-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed2c9-133">JSON representation</span></span>
<span data-ttu-id="ed2c9-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed2c9-134">Here is a JSON representation of the resource.</span></span>

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
