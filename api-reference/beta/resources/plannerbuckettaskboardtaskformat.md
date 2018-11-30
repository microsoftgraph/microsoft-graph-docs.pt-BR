---
title: Tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
ms.openlocfilehash: 2fa91a4900a12f4c7433049c8ee4be94cdaa7b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039253"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="17bac-104">Tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="17bac-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="17bac-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17bac-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17bac-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17bac-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17bac-p103">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="17bac-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="17bac-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="17bac-109">Methods</span></span>

| <span data-ttu-id="17bac-110">Método</span><span class="sxs-lookup"><span data-stu-id="17bac-110">Method</span></span>           | <span data-ttu-id="17bac-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17bac-111">Return Type</span></span>    |<span data-ttu-id="17bac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="17bac-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17bac-113">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="17bac-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="17bac-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="17bac-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="17bac-115">Leia as propriedades e as relações do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="17bac-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="17bac-116">Update</span><span class="sxs-lookup"><span data-stu-id="17bac-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="17bac-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="17bac-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="17bac-118">Atualize o objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="17bac-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="17bac-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17bac-119">Properties</span></span>
| <span data-ttu-id="17bac-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17bac-120">Property</span></span>     | <span data-ttu-id="17bac-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="17bac-121">Type</span></span>   |<span data-ttu-id="17bac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="17bac-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17bac-123">id</span><span class="sxs-lookup"><span data-stu-id="17bac-123">id</span></span>|<span data-ttu-id="17bac-124">String</span><span class="sxs-lookup"><span data-stu-id="17bac-124">String</span></span>| <span data-ttu-id="17bac-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17bac-125">Read-only.</span></span> <span data-ttu-id="17bac-126">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="17bac-126">ID of the resource.</span></span> <span data-ttu-id="17bac-127">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="17bac-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="17bac-128">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="17bac-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="17bac-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="17bac-129">orderHint</span></span>|<span data-ttu-id="17bac-130">String</span><span class="sxs-lookup"><span data-stu-id="17bac-130">String</span></span>|<span data-ttu-id="17bac-p105">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="17bac-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="17bac-133">Relações</span><span class="sxs-lookup"><span data-stu-id="17bac-133">Relationships</span></span>
<span data-ttu-id="17bac-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17bac-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="17bac-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17bac-135">JSON representation</span></span>
<span data-ttu-id="17bac-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17bac-136">Here is a JSON representation of the resource.</span></span>

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