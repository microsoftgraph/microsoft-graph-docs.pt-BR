---
title: tipo de recurso todo
description: Representa os serviços de tarefas pendentes disponíveis para um usuário.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99b2936cf84c5cfdc25a39ff6f0e35518658d0ff
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849828"
---
# <a name="todo-resource-type"></a><span data-ttu-id="73bc4-103">tipo de recurso todo</span><span class="sxs-lookup"><span data-stu-id="73bc4-103">todo resource type</span></span>

<span data-ttu-id="73bc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73bc4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73bc4-105">Representa os serviços de tarefas pendentes disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="73bc4-105">Represents the To Do services available to a user.</span></span>

<span data-ttu-id="73bc4-106">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="73bc4-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="73bc4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="73bc4-107">Methods</span></span>
|<span data-ttu-id="73bc4-108">Método</span><span class="sxs-lookup"><span data-stu-id="73bc4-108">Method</span></span>|<span data-ttu-id="73bc4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73bc4-109">Return type</span></span>|<span data-ttu-id="73bc4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bc4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73bc4-111">Listar listas</span><span class="sxs-lookup"><span data-stu-id="73bc4-111">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="73bc4-112">coleção [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="73bc4-112">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="73bc4-113">Obtenha todas as listas de tarefas na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="73bc4-113">Get all the task lists in the user's mailbox.</span></span> |
|[<span data-ttu-id="73bc4-114">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="73bc4-114">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="73bc4-115">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="73bc4-115">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="73bc4-116">Criar uma lista de tarefas pendentes na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="73bc4-116">Create a To Do task list in the user's mailbox.</span></span> |

## <a name="properties"></a><span data-ttu-id="73bc4-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73bc4-117">Properties</span></span>
<span data-ttu-id="73bc4-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="73bc4-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="73bc4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="73bc4-119">Relationships</span></span>
|<span data-ttu-id="73bc4-120">Relação</span><span class="sxs-lookup"><span data-stu-id="73bc4-120">Relationship</span></span>|<span data-ttu-id="73bc4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="73bc4-121">Type</span></span>|<span data-ttu-id="73bc4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bc4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73bc4-123">listas</span><span class="sxs-lookup"><span data-stu-id="73bc4-123">lists</span></span>|<span data-ttu-id="73bc4-124">coleção [todoTaskList](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="73bc4-124">[todoTaskList](../resources/todotasklist.md) collection</span></span>| <span data-ttu-id="73bc4-125">As listas de tarefas na caixa de correio dos usuários.</span><span class="sxs-lookup"><span data-stu-id="73bc4-125">The task lists in the users mailbox.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73bc4-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73bc4-126">JSON representation</span></span>
<span data-ttu-id="73bc4-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73bc4-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todo",
  "id": "String"
}
```

