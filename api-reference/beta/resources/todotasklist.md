---
title: tipo de recurso todoTaskList
description: Uma lista na Microsoft que contém um ou mais recursos do todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0523404e836223f8a59e191d1e7040a279433795
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073380"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="d5a68-103">tipo de recurso todoTaskList</span><span class="sxs-lookup"><span data-stu-id="d5a68-103">todoTaskList resource type</span></span>

<span data-ttu-id="d5a68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5a68-105">Uma lista na Microsoft que contém um ou mais recursos do [todoTask](./todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="d5a68-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="d5a68-106">Em tarefas pendentes, há listas de tarefas internas, como **emails sinalizados** e **tarefas** que não podem ser renomeadas ou excluídas.</span><span class="sxs-lookup"><span data-stu-id="d5a68-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="d5a68-107">No entanto, você pode criar listas de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="d5a68-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="d5a68-108">Este recurso suporta</span><span class="sxs-lookup"><span data-stu-id="d5a68-108">This resource supports</span></span>
* <span data-ttu-id="d5a68-109">Adicionando seus dados às propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="d5a68-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="d5a68-110">Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.</span><span class="sxs-lookup"><span data-stu-id="d5a68-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="d5a68-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5a68-111">Methods</span></span>
|<span data-ttu-id="d5a68-112">Método</span><span class="sxs-lookup"><span data-stu-id="d5a68-112">Method</span></span>|<span data-ttu-id="d5a68-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5a68-113">Return type</span></span>|<span data-ttu-id="d5a68-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5a68-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5a68-115">List lists</span><span class="sxs-lookup"><span data-stu-id="d5a68-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="d5a68-116">Coleção [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="d5a68-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="d5a68-117">Obtenha todos os [todoTaskList](todotasklist.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5a68-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="d5a68-118">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="d5a68-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="d5a68-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="d5a68-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="d5a68-120">Criar um [todoTaskList](todotasklist.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5a68-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="d5a68-121">Obter lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="d5a68-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="d5a68-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="d5a68-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="d5a68-123">Leia as propriedades e as relações do [todoTaskList](todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d5a68-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="d5a68-124">Atualizar lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="d5a68-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="d5a68-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="d5a68-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="d5a68-126">Atualize as propriedades graváveis do [todoTaskList](todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d5a68-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="d5a68-127">Excluir lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="d5a68-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="d5a68-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5a68-128">None</span></span>| <span data-ttu-id="d5a68-129">Exclua o [todoTaskList](todotasklist.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="d5a68-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="d5a68-130">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d5a68-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="d5a68-131">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="d5a68-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="d5a68-132">Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.</span><span class="sxs-lookup"><span data-stu-id="d5a68-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="d5a68-133">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="d5a68-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="d5a68-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="d5a68-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="d5a68-135">Criar um [todoTask](todotask.md) na lista de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="d5a68-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5a68-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5a68-136">Properties</span></span>
|<span data-ttu-id="d5a68-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5a68-137">Property</span></span>|<span data-ttu-id="d5a68-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5a68-138">Type</span></span>|<span data-ttu-id="d5a68-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5a68-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5a68-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d5a68-140">displayName</span></span>|<span data-ttu-id="d5a68-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5a68-141">String</span></span>|<span data-ttu-id="d5a68-142">O nome da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d5a68-142">The name of the task list.</span></span>|
|<span data-ttu-id="d5a68-143">id</span><span class="sxs-lookup"><span data-stu-id="d5a68-143">id</span></span>|<span data-ttu-id="d5a68-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5a68-144">String</span></span>| <span data-ttu-id="d5a68-145">O identificador da lista de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5a68-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="d5a68-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5a68-146">Read-only.</span></span> <span data-ttu-id="d5a68-147">Herdado da [entidade](entity.md)</span><span class="sxs-lookup"><span data-stu-id="d5a68-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="d5a68-148">IsOwner</span><span class="sxs-lookup"><span data-stu-id="d5a68-148">isOwner</span></span>|<span data-ttu-id="d5a68-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5a68-149">Boolean</span></span>| <span data-ttu-id="d5a68-150">True se o usuário é proprietário da lista de tarefas determinada.</span><span class="sxs-lookup"><span data-stu-id="d5a68-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="d5a68-151">isShared</span><span class="sxs-lookup"><span data-stu-id="d5a68-151">isShared</span></span>|<span data-ttu-id="d5a68-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5a68-152">Boolean</span></span>| <span data-ttu-id="d5a68-153">True se a lista de tarefas é compartilhada com outros usuários</span><span class="sxs-lookup"><span data-stu-id="d5a68-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="d5a68-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="d5a68-154">wellknownListName</span></span>|<span data-ttu-id="d5a68-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="d5a68-155">wellknownListName</span></span>| <span data-ttu-id="d5a68-156">Propriedade que indica o nome da lista conhecido se a lista fornecida é uma lista conhecida.</span><span class="sxs-lookup"><span data-stu-id="d5a68-156">Property indicating the well-known list name if the given list is a well-known list.</span></span> <span data-ttu-id="d5a68-157">Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d5a68-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5a68-158">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d5a68-158">Relationships</span></span>
|<span data-ttu-id="d5a68-159">Relação</span><span class="sxs-lookup"><span data-stu-id="d5a68-159">Relationship</span></span>|<span data-ttu-id="d5a68-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5a68-160">Type</span></span>|<span data-ttu-id="d5a68-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5a68-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5a68-162">extensions</span><span class="sxs-lookup"><span data-stu-id="d5a68-162">extensions</span></span>|<span data-ttu-id="d5a68-163">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="d5a68-163">[extension](extension.md) collection</span></span>| <span data-ttu-id="d5a68-164">A coleção de extensões abertas definida para a lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d5a68-164">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="d5a68-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d5a68-165">Nullable.</span></span>|
|<span data-ttu-id="d5a68-166">tarefas</span><span class="sxs-lookup"><span data-stu-id="d5a68-166">tasks</span></span>|<span data-ttu-id="d5a68-167">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="d5a68-167">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="d5a68-168">As tarefas desta lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d5a68-168">The tasks in this task list.</span></span> <span data-ttu-id="d5a68-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5a68-169">Read-only.</span></span> <span data-ttu-id="d5a68-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d5a68-170">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5a68-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5a68-171">JSON representation</span></span>
<span data-ttu-id="d5a68-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5a68-172">The following is a JSON representation of the resource.</span></span>
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



