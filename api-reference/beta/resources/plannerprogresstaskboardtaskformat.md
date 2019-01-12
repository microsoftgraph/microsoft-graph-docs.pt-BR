---
title: Tipo de recurso plannerProgressTaskBoardTaskFormat
description: O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada tarefa terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 58e1b80c61dcb0c58996f65c1fa03c48c4edafbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955923"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="f697a-104">Tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f697a-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="f697a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f697a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f697a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f697a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f697a-p103">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="f697a-p103">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="f697a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f697a-109">Methods</span></span>

| <span data-ttu-id="f697a-110">Método</span><span class="sxs-lookup"><span data-stu-id="f697a-110">Method</span></span>           | <span data-ttu-id="f697a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f697a-111">Return Type</span></span>    |<span data-ttu-id="f697a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f697a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f697a-113">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f697a-113">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="f697a-114">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f697a-114">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="f697a-115">Leia as propriedades e as relações do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f697a-115">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="f697a-116">Update</span><span class="sxs-lookup"><span data-stu-id="f697a-116">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="f697a-117">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f697a-117">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="f697a-118">Atualize o objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f697a-118">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f697a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f697a-119">Properties</span></span>
| <span data-ttu-id="f697a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f697a-120">Property</span></span>     | <span data-ttu-id="f697a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f697a-121">Type</span></span>   |<span data-ttu-id="f697a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f697a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f697a-123">id</span><span class="sxs-lookup"><span data-stu-id="f697a-123">id</span></span>|<span data-ttu-id="f697a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f697a-124">String</span></span>| <span data-ttu-id="f697a-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f697a-125">Read-only.</span></span> <span data-ttu-id="f697a-126">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="f697a-126">ID of the resource.</span></span> <span data-ttu-id="f697a-127">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="f697a-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f697a-128">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="f697a-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="f697a-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="f697a-129">orderHint</span></span>|<span data-ttu-id="f697a-130">String</span><span class="sxs-lookup"><span data-stu-id="f697a-130">String</span></span>|<span data-ttu-id="f697a-p105">Valor da dica usado para ordenar a tarefa no modo de exibição Progress do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f697a-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f697a-133">Relações</span><span class="sxs-lookup"><span data-stu-id="f697a-133">Relationships</span></span>
<span data-ttu-id="f697a-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f697a-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f697a-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f697a-135">JSON representation</span></span>
<span data-ttu-id="f697a-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f697a-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
