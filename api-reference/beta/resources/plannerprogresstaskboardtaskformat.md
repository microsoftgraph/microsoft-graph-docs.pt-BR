---
title: Tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada **tarefa** terá um objeto plannerProgressTaskBoardTaskFormat associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522067"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="a612a-104">Tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a612a-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a612a-p102">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="a612a-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="a612a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a612a-107">Methods</span></span>

| <span data-ttu-id="a612a-108">Método</span><span class="sxs-lookup"><span data-stu-id="a612a-108">Method</span></span>           | <span data-ttu-id="a612a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a612a-109">Return Type</span></span>    |<span data-ttu-id="a612a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a612a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a612a-111">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a612a-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="a612a-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a612a-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="a612a-113">Leia as propriedades e as relações do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="a612a-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="a612a-114">Update</span><span class="sxs-lookup"><span data-stu-id="a612a-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="a612a-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a612a-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="a612a-116">Atualize o objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="a612a-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a612a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a612a-117">Properties</span></span>
| <span data-ttu-id="a612a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a612a-118">Property</span></span>     | <span data-ttu-id="a612a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a612a-119">Type</span></span>   |<span data-ttu-id="a612a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a612a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a612a-121">id</span><span class="sxs-lookup"><span data-stu-id="a612a-121">id</span></span>|<span data-ttu-id="a612a-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a612a-122">String</span></span>| <span data-ttu-id="a612a-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a612a-123">Read-only.</span></span> <span data-ttu-id="a612a-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="a612a-124">ID of the resource.</span></span> <span data-ttu-id="a612a-125">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a612a-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a612a-126">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="a612a-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a612a-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="a612a-127">orderHint</span></span>|<span data-ttu-id="a612a-128">String</span><span class="sxs-lookup"><span data-stu-id="a612a-128">String</span></span>|<span data-ttu-id="a612a-p104">Valor da dica usado para ordenar a tarefa no modo de exibição Progress do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="a612a-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a612a-131">Relações</span><span class="sxs-lookup"><span data-stu-id="a612a-131">Relationships</span></span>
<span data-ttu-id="a612a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a612a-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a612a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a612a-133">JSON representation</span></span>
<span data-ttu-id="a612a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a612a-134">Here is a JSON representation of the resource.</span></span>

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
