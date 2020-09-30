---
title: tipo de recurso todoTaskList
description: Uma lista na Microsoft que contém um ou mais recursos do todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bddf0b72173b2f37b3fdd8544bc777c87bb33ee3
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314591"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="774ec-103">tipo de recurso todoTaskList</span><span class="sxs-lookup"><span data-stu-id="774ec-103">todoTaskList resource type</span></span>

<span data-ttu-id="774ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="774ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="774ec-105">Uma lista na Microsoft que contém um ou mais recursos do [todoTask](./todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="774ec-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="774ec-106">Em tarefas pendentes, há listas de tarefas internas, como **emails sinalizados** e **tarefas** que não podem ser renomeadas ou excluídas.</span><span class="sxs-lookup"><span data-stu-id="774ec-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="774ec-107">No entanto, você pode criar listas de tarefas adicionais.</span><span class="sxs-lookup"><span data-stu-id="774ec-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="774ec-108">Este recurso suporta</span><span class="sxs-lookup"><span data-stu-id="774ec-108">This resource supports</span></span>
* <span data-ttu-id="774ec-109">Adicionando seus dados às propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="774ec-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="774ec-110">Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.</span><span class="sxs-lookup"><span data-stu-id="774ec-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="774ec-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="774ec-111">Methods</span></span>
|<span data-ttu-id="774ec-112">Método</span><span class="sxs-lookup"><span data-stu-id="774ec-112">Method</span></span>|<span data-ttu-id="774ec-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="774ec-113">Return type</span></span>|<span data-ttu-id="774ec-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="774ec-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="774ec-115">List lists</span><span class="sxs-lookup"><span data-stu-id="774ec-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="774ec-116">Coleção [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="774ec-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="774ec-117">Obtenha todos os [todoTaskList](todotasklist.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="774ec-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="774ec-118">Criar todoTaskList</span><span class="sxs-lookup"><span data-stu-id="774ec-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="774ec-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="774ec-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="774ec-120">Criar um [todoTaskList](todotasklist.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="774ec-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="774ec-121">Obter lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="774ec-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="774ec-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="774ec-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="774ec-123">Leia as propriedades e as relações do [todoTaskList](todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="774ec-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="774ec-124">Atualizar lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="774ec-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="774ec-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="774ec-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="774ec-126">Atualize as propriedades graváveis do [todoTaskList](todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="774ec-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="774ec-127">Excluir lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="774ec-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="774ec-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="774ec-128">None</span></span>| <span data-ttu-id="774ec-129">Exclua o [todoTaskList](todotasklist.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="774ec-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="774ec-130">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="774ec-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="774ec-131">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="774ec-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="774ec-132">Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.</span><span class="sxs-lookup"><span data-stu-id="774ec-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="774ec-133">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="774ec-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="774ec-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="774ec-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="774ec-135">Criar um [todoTask](todotask.md) na lista de tarefas especificada.</span><span class="sxs-lookup"><span data-stu-id="774ec-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="774ec-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="774ec-136">Properties</span></span>
|<span data-ttu-id="774ec-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="774ec-137">Property</span></span>|<span data-ttu-id="774ec-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="774ec-138">Type</span></span>|<span data-ttu-id="774ec-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="774ec-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="774ec-140">displayName</span><span class="sxs-lookup"><span data-stu-id="774ec-140">displayName</span></span>|<span data-ttu-id="774ec-141">String</span><span class="sxs-lookup"><span data-stu-id="774ec-141">String</span></span>|<span data-ttu-id="774ec-142">O nome da lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="774ec-142">The name of the task list.</span></span>|
|<span data-ttu-id="774ec-143">id</span><span class="sxs-lookup"><span data-stu-id="774ec-143">id</span></span>|<span data-ttu-id="774ec-144">String</span><span class="sxs-lookup"><span data-stu-id="774ec-144">String</span></span>| <span data-ttu-id="774ec-145">O identificador da lista de tarefas, exclusivo na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="774ec-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="774ec-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="774ec-146">Read-only.</span></span> <span data-ttu-id="774ec-147">Herdado da [entidade](entity.md)</span><span class="sxs-lookup"><span data-stu-id="774ec-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="774ec-148">IsOwner</span><span class="sxs-lookup"><span data-stu-id="774ec-148">isOwner</span></span>|<span data-ttu-id="774ec-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="774ec-149">Boolean</span></span>| <span data-ttu-id="774ec-150">True se o usuário é proprietário da lista de tarefas determinada.</span><span class="sxs-lookup"><span data-stu-id="774ec-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="774ec-151">isShared</span><span class="sxs-lookup"><span data-stu-id="774ec-151">isShared</span></span>|<span data-ttu-id="774ec-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="774ec-152">Boolean</span></span>| <span data-ttu-id="774ec-153">True se a lista de tarefas é compartilhada com outros usuários</span><span class="sxs-lookup"><span data-stu-id="774ec-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="774ec-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="774ec-154">wellknownListName</span></span>|<span data-ttu-id="774ec-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="774ec-155">wellknownListName</span></span>| <span data-ttu-id="774ec-156">Propriedade que indica o nome da lista se a lista fornecida é uma lista conhecida.</span><span class="sxs-lookup"><span data-stu-id="774ec-156">Property indicating the list name if the given list is a well-known list.</span></span> <span data-ttu-id="774ec-157">Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="774ec-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

### <a name="wellknownlistname-values"></a><span data-ttu-id="774ec-158">valores de wellknownListName</span><span class="sxs-lookup"><span data-stu-id="774ec-158">wellknownListName values</span></span>
|<span data-ttu-id="774ec-159">Member</span><span class="sxs-lookup"><span data-stu-id="774ec-159">Member</span></span>|<span data-ttu-id="774ec-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="774ec-160">Description</span></span>|
|:---|:---|
|<span data-ttu-id="774ec-161">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="774ec-161">none</span></span>| <span data-ttu-id="774ec-162">Lista criada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="774ec-162">User created list.</span></span>|
|<span data-ttu-id="774ec-163">defaultlist</span><span class="sxs-lookup"><span data-stu-id="774ec-163">defaultList</span></span>| <span data-ttu-id="774ec-164">Lista de **tarefas** interna.</span><span class="sxs-lookup"><span data-stu-id="774ec-164">Built-in **Tasks** list.</span></span>|
|<span data-ttu-id="774ec-165">flaggedEmails</span><span class="sxs-lookup"><span data-stu-id="774ec-165">flaggedEmails</span></span>| <span data-ttu-id="774ec-166">Lista de **emails sinalizada** interna.</span><span class="sxs-lookup"><span data-stu-id="774ec-166">Built-in **Flagged email** list.</span></span> <span data-ttu-id="774ec-167">As tarefas de emails sinalizados estão presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="774ec-167">Tasks from flagged emails are present in this list.</span></span>|
|<span data-ttu-id="774ec-168">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="774ec-168">unknownFutureValue</span></span>| <span data-ttu-id="774ec-169">Valor de sentinela de enumeração evolvable.</span><span class="sxs-lookup"><span data-stu-id="774ec-169">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="774ec-170">Não usar.</span><span class="sxs-lookup"><span data-stu-id="774ec-170">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="774ec-171">Relações</span><span class="sxs-lookup"><span data-stu-id="774ec-171">Relationships</span></span>
|<span data-ttu-id="774ec-172">Relação</span><span class="sxs-lookup"><span data-stu-id="774ec-172">Relationship</span></span>|<span data-ttu-id="774ec-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="774ec-173">Type</span></span>|<span data-ttu-id="774ec-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="774ec-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="774ec-175">extensions</span><span class="sxs-lookup"><span data-stu-id="774ec-175">extensions</span></span>|<span data-ttu-id="774ec-176">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="774ec-176">[extension](extension.md) collection</span></span>| <span data-ttu-id="774ec-177">A coleção de extensões abertas definida para a lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="774ec-177">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="774ec-178">Anulável.</span><span class="sxs-lookup"><span data-stu-id="774ec-178">Nullable.</span></span>|
|<span data-ttu-id="774ec-179">tarefas</span><span class="sxs-lookup"><span data-stu-id="774ec-179">tasks</span></span>|<span data-ttu-id="774ec-180">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="774ec-180">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="774ec-181">As tarefas desta lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="774ec-181">The tasks in this task list.</span></span> <span data-ttu-id="774ec-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="774ec-182">Read-only.</span></span> <span data-ttu-id="774ec-183">Anulável.</span><span class="sxs-lookup"><span data-stu-id="774ec-183">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="774ec-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="774ec-184">JSON representation</span></span>
<span data-ttu-id="774ec-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="774ec-185">The following is a JSON representation of the resource.</span></span>
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



