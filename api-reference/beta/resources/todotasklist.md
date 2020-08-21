---
title: tipo de recurso todoTaskList
description: Uma lista na Microsoft que contém um ou mais recursos do todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34f90329fc6ca4d5e12ff2f2b191819b88f895b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849825"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="6f9b3-103">tipo de recurso todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6f9b3-103">todoTaskList resource type</span></span>

<span data-ttu-id="6f9b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f9b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f9b3-105">Uma lista na Microsoft que contém um ou mais recursos do [todoTask](./todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="6f9b3-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="6f9b3-106">Em tarefas pendentes, há listas de tarefas internas, como **emails sinalizados** e **tarefas** que não podem ser renomeadas ou excluídas.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="6f9b3-107">No entanto, você pode criar listas de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="6f9b3-108">Este recurso suporta</span><span class="sxs-lookup"><span data-stu-id="6f9b3-108">This resource supports</span></span>
* <span data-ttu-id="6f9b3-109">Adicionando seus dados às propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="6f9b3-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="6f9b3-110">Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="6f9b3-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f9b3-111">Methods</span></span>
|<span data-ttu-id="6f9b3-112">Método</span><span class="sxs-lookup"><span data-stu-id="6f9b3-112">Method</span></span>|<span data-ttu-id="6f9b3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f9b3-113">Return type</span></span>|<span data-ttu-id="6f9b3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f9b3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6f9b3-115">Listar listas</span><span class="sxs-lookup"><span data-stu-id="6f9b3-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="6f9b3-116">coleção [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="6f9b3-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="6f9b3-117">Obtenha todos os [todoTaskList](todotasklist.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="6f9b3-118">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6f9b3-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="6f9b3-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6f9b3-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="6f9b3-120">Criar um [todoTaskList](todotasklist.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="6f9b3-121">Obter lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="6f9b3-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="6f9b3-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6f9b3-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="6f9b3-123">Leia as propriedades e as relações do [todoTaskList](todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="6f9b3-124">Atualizar lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="6f9b3-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="6f9b3-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6f9b3-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="6f9b3-126">Atualize as propriedades graváveis do [todoTaskList](todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="6f9b3-127">Excluir lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="6f9b3-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="6f9b3-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6f9b3-128">None</span></span>| <span data-ttu-id="6f9b3-129">Exclua o [todoTaskList](todotasklist.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="6f9b3-130">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="6f9b3-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="6f9b3-131">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="6f9b3-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="6f9b3-132">Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="6f9b3-133">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="6f9b3-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="6f9b3-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="6f9b3-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="6f9b3-135">Criar um [todoTask](todotask.md) na lista de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f9b3-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f9b3-136">Properties</span></span>
|<span data-ttu-id="6f9b3-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f9b3-137">Property</span></span>|<span data-ttu-id="6f9b3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f9b3-138">Type</span></span>|<span data-ttu-id="6f9b3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f9b3-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f9b3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="6f9b3-140">displayName</span></span>|<span data-ttu-id="6f9b3-141">String</span><span class="sxs-lookup"><span data-stu-id="6f9b3-141">String</span></span>|<span data-ttu-id="6f9b3-142">O nome da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-142">The name of the task list.</span></span>|
|<span data-ttu-id="6f9b3-143">id</span><span class="sxs-lookup"><span data-stu-id="6f9b3-143">id</span></span>|<span data-ttu-id="6f9b3-144">String</span><span class="sxs-lookup"><span data-stu-id="6f9b3-144">String</span></span>| <span data-ttu-id="6f9b3-145">O identificador da lista de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="6f9b3-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-146">Read-only.</span></span> <span data-ttu-id="6f9b3-147">Herdado da [entidade](entity.md)</span><span class="sxs-lookup"><span data-stu-id="6f9b3-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="6f9b3-148">IsOwner</span><span class="sxs-lookup"><span data-stu-id="6f9b3-148">isOwner</span></span>|<span data-ttu-id="6f9b3-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f9b3-149">Boolean</span></span>| <span data-ttu-id="6f9b3-150">True se o usuário é proprietário da lista de tarefas determinada.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="6f9b3-151">isShared</span><span class="sxs-lookup"><span data-stu-id="6f9b3-151">isShared</span></span>|<span data-ttu-id="6f9b3-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f9b3-152">Boolean</span></span>| <span data-ttu-id="6f9b3-153">True se a lista de tarefas é compartilhada com outros usuários</span><span class="sxs-lookup"><span data-stu-id="6f9b3-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="6f9b3-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="6f9b3-154">wellknownListName</span></span>|<span data-ttu-id="6f9b3-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="6f9b3-155">wellknownListName</span></span>| <span data-ttu-id="6f9b3-156">Propriedade que indica o nome da lista conhecido se a lista fornecida é uma lista conhecida.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-156">Property indicating the well-known list name if the given list is a well-known list.</span></span> <span data-ttu-id="6f9b3-157">Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f9b3-158">Relações</span><span class="sxs-lookup"><span data-stu-id="6f9b3-158">Relationships</span></span>
|<span data-ttu-id="6f9b3-159">Relação</span><span class="sxs-lookup"><span data-stu-id="6f9b3-159">Relationship</span></span>|<span data-ttu-id="6f9b3-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f9b3-160">Type</span></span>|<span data-ttu-id="6f9b3-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f9b3-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f9b3-162">extensions</span><span class="sxs-lookup"><span data-stu-id="6f9b3-162">extensions</span></span>|<span data-ttu-id="6f9b3-163">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="6f9b3-163">[extension](extension.md) collection</span></span>| <span data-ttu-id="6f9b3-164">A coleção de extensões abertas definida para a lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-164">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="6f9b3-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-165">Nullable.</span></span>|
|<span data-ttu-id="6f9b3-166">tarefas</span><span class="sxs-lookup"><span data-stu-id="6f9b3-166">tasks</span></span>|<span data-ttu-id="6f9b3-167">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="6f9b3-167">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="6f9b3-168">As tarefas desta lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-168">The tasks in this task list.</span></span> <span data-ttu-id="6f9b3-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-169">Read-only.</span></span> <span data-ttu-id="6f9b3-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-170">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f9b3-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f9b3-171">JSON representation</span></span>
<span data-ttu-id="6f9b3-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f9b3-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```

