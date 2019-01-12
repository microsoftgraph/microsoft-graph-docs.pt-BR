---
title: Tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea557bad20aa0fd10a73e71902b959913e8fff12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986191"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="e3ce9-104">Tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e3ce9-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="e3ce9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3ce9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3ce9-p103">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="e3ce9-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e3ce9-109">Methods</span></span>

| <span data-ttu-id="e3ce9-110">Método</span><span class="sxs-lookup"><span data-stu-id="e3ce9-110">Method</span></span>           | <span data-ttu-id="e3ce9-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3ce9-111">Return Type</span></span>    |<span data-ttu-id="e3ce9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3ce9-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3ce9-113">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e3ce9-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="e3ce9-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e3ce9-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="e3ce9-115">Leia as propriedades e as relações do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="e3ce9-116">Update</span><span class="sxs-lookup"><span data-stu-id="e3ce9-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="e3ce9-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e3ce9-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="e3ce9-118">Atualize o objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3ce9-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3ce9-119">Properties</span></span>
| <span data-ttu-id="e3ce9-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3ce9-120">Property</span></span>     | <span data-ttu-id="e3ce9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3ce9-121">Type</span></span>   |<span data-ttu-id="e3ce9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3ce9-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3ce9-123">id</span><span class="sxs-lookup"><span data-stu-id="e3ce9-123">id</span></span>|<span data-ttu-id="e3ce9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3ce9-124">String</span></span>| <span data-ttu-id="e3ce9-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-125">Read-only.</span></span> <span data-ttu-id="e3ce9-126">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-126">ID of the resource.</span></span> <span data-ttu-id="e3ce9-127">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e3ce9-128">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e3ce9-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="e3ce9-129">orderHint</span></span>|<span data-ttu-id="e3ce9-130">String</span><span class="sxs-lookup"><span data-stu-id="e3ce9-130">String</span></span>|<span data-ttu-id="e3ce9-p105">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e3ce9-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3ce9-133">Relações</span><span class="sxs-lookup"><span data-stu-id="e3ce9-133">Relationships</span></span>
<span data-ttu-id="e3ce9-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3ce9-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e3ce9-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3ce9-135">JSON representation</span></span>
<span data-ttu-id="e3ce9-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3ce9-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
