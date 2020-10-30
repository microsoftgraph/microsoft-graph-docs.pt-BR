---
title: tipo de recurso todo
description: Representa os serviços To Do disponíveis para um usuário.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa468c6d6556ad70d3650e40fb3fd01c46ccdb35
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797222"
---
# <a name="todo-resource-type"></a><span data-ttu-id="5d86b-103">tipo de recurso todo</span><span class="sxs-lookup"><span data-stu-id="5d86b-103">todo resource type</span></span>

<span data-ttu-id="5d86b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d86b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d86b-105">Representa os serviços To Do disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="5d86b-105">Represents the To Do services available to a user.</span></span>

<span data-ttu-id="5d86b-106">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="5d86b-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5d86b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5d86b-107">Methods</span></span>
|<span data-ttu-id="5d86b-108">Método</span><span class="sxs-lookup"><span data-stu-id="5d86b-108">Method</span></span>|<span data-ttu-id="5d86b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d86b-109">Return type</span></span>|<span data-ttu-id="5d86b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d86b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5d86b-111">List lists</span><span class="sxs-lookup"><span data-stu-id="5d86b-111">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="5d86b-112">Coleção [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="5d86b-112">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="5d86b-113">Obtenha todas as listas de tarefas na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d86b-113">Get all the task lists in the user's mailbox.</span></span> |
|[<span data-ttu-id="5d86b-114">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5d86b-114">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="5d86b-115">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5d86b-115">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="5d86b-116">Criar uma lista de tarefas To Dona caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d86b-116">Create a To Do task list in the user's mailbox.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d86b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d86b-117">Properties</span></span>
<span data-ttu-id="5d86b-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5d86b-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5d86b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5d86b-119">Relationships</span></span>
|<span data-ttu-id="5d86b-120">Relação</span><span class="sxs-lookup"><span data-stu-id="5d86b-120">Relationship</span></span>|<span data-ttu-id="5d86b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d86b-121">Type</span></span>|<span data-ttu-id="5d86b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d86b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d86b-123">listas</span><span class="sxs-lookup"><span data-stu-id="5d86b-123">lists</span></span>|<span data-ttu-id="5d86b-124">Coleção [todoTaskList](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="5d86b-124">[todoTaskList](../resources/todotasklist.md) collection</span></span>| <span data-ttu-id="5d86b-125">As listas de tarefas na caixa de correio dos usuários.</span><span class="sxs-lookup"><span data-stu-id="5d86b-125">The task lists in the users mailbox.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d86b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d86b-126">JSON representation</span></span>
<span data-ttu-id="5d86b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d86b-127">The following is a JSON representation of the resource.</span></span>
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



