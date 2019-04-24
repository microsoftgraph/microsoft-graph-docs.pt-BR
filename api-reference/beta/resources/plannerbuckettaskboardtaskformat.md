---
title: tipo de recurso plannerBucketTaskBoardTaskFormat
description: O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas). Cada tarefa terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eca8865e54d68fb7b403364b065e642ad61e9276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457057"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="92d37-104">tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="92d37-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d37-105">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição buckets do quadro de tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais são atribuídas).</span><span class="sxs-lookup"><span data-stu-id="92d37-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="92d37-106">Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="92d37-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="92d37-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="92d37-107">Methods</span></span>

| <span data-ttu-id="92d37-108">Método</span><span class="sxs-lookup"><span data-stu-id="92d37-108">Method</span></span>           | <span data-ttu-id="92d37-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="92d37-109">Return Type</span></span>    |<span data-ttu-id="92d37-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d37-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92d37-111">Obter plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="92d37-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="92d37-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="92d37-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="92d37-113">Leia as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="92d37-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="92d37-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="92d37-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="92d37-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="92d37-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="92d37-116">Atualize o objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="92d37-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="92d37-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92d37-117">Properties</span></span>
| <span data-ttu-id="92d37-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92d37-118">Property</span></span>     | <span data-ttu-id="92d37-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="92d37-119">Type</span></span>   |<span data-ttu-id="92d37-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d37-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92d37-121">id</span><span class="sxs-lookup"><span data-stu-id="92d37-121">id</span></span>|<span data-ttu-id="92d37-122">String</span><span class="sxs-lookup"><span data-stu-id="92d37-122">String</span></span>| <span data-ttu-id="92d37-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92d37-123">Read-only.</span></span> <span data-ttu-id="92d37-124">ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="92d37-124">ID of the resource.</span></span> <span data-ttu-id="92d37-125">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="92d37-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="92d37-126">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="92d37-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="92d37-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="92d37-127">orderHint</span></span>|<span data-ttu-id="92d37-128">String</span><span class="sxs-lookup"><span data-stu-id="92d37-128">String</span></span>|<span data-ttu-id="92d37-129">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="92d37-129">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="92d37-130">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="92d37-130">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="92d37-131">Relações</span><span class="sxs-lookup"><span data-stu-id="92d37-131">Relationships</span></span>
<span data-ttu-id="92d37-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="92d37-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="92d37-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92d37-133">JSON representation</span></span>
<span data-ttu-id="92d37-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92d37-134">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbuckettaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
