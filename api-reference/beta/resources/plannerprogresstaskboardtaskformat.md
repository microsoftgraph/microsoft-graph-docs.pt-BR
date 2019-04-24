---
title: tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com colunas para não iniciado , Em andamento e concluído). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522122"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="52ec3-104">tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52ec3-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52ec3-105">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição de progresso do quadro de tarefas (um modo organizado pelo estado do campo PercentComplete no objeto Task, com colunas para não iniciado , Em andamento e concluído).</span><span class="sxs-lookup"><span data-stu-id="52ec3-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="52ec3-106">Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="52ec3-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="52ec3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="52ec3-107">Methods</span></span>

| <span data-ttu-id="52ec3-108">Método</span><span class="sxs-lookup"><span data-stu-id="52ec3-108">Method</span></span>           | <span data-ttu-id="52ec3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52ec3-109">Return Type</span></span>    |<span data-ttu-id="52ec3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ec3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52ec3-111">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52ec3-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="52ec3-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52ec3-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="52ec3-113">Leia as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="52ec3-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="52ec3-114">Update</span><span class="sxs-lookup"><span data-stu-id="52ec3-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="52ec3-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="52ec3-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="52ec3-116">Atualize o objeto **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="52ec3-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52ec3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52ec3-117">Properties</span></span>
| <span data-ttu-id="52ec3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52ec3-118">Property</span></span>     | <span data-ttu-id="52ec3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="52ec3-119">Type</span></span>   |<span data-ttu-id="52ec3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52ec3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52ec3-121">id</span><span class="sxs-lookup"><span data-stu-id="52ec3-121">id</span></span>|<span data-ttu-id="52ec3-122">String</span><span class="sxs-lookup"><span data-stu-id="52ec3-122">String</span></span>| <span data-ttu-id="52ec3-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52ec3-123">Read-only.</span></span> <span data-ttu-id="52ec3-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="52ec3-124">ID of the resource.</span></span> <span data-ttu-id="52ec3-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="52ec3-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="52ec3-126">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="52ec3-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="52ec3-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="52ec3-127">orderHint</span></span>|<span data-ttu-id="52ec3-128">String</span><span class="sxs-lookup"><span data-stu-id="52ec3-128">String</span></span>|<span data-ttu-id="52ec3-129">O valor de dica usado para ordenar a tarefa no modo de exibição de progresso do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="52ec3-129">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="52ec3-130">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="52ec3-130">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="52ec3-131">Relações</span><span class="sxs-lookup"><span data-stu-id="52ec3-131">Relationships</span></span>
<span data-ttu-id="52ec3-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="52ec3-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="52ec3-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52ec3-133">JSON representation</span></span>
<span data-ttu-id="52ec3-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52ec3-134">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerprogresstaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
