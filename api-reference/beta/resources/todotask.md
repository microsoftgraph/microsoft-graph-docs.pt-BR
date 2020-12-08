---
title: tipo de recurso todoTask
description: Um recurso todoTask controla um item de trabalho.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ffcd3da43b7ae165045b545c656035e47d291419
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597197"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="4c368-103">tipo de recurso todoTask</span><span class="sxs-lookup"><span data-stu-id="4c368-103">todoTask resource type</span></span>

<span data-ttu-id="4c368-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4c368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c368-105">Um **todoTask** representa uma tarefa, como uma parte do trabalho ou item pessoal, que pode ser controlada e concluída.</span><span class="sxs-lookup"><span data-stu-id="4c368-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="4c368-106">Um **todoTask** está sempre contido em um [todoTaskList](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="4c368-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="4c368-107">Ele inclui uma relação com uma coleção de objetos [linkedResource](./linkedResource.md) , controlando uma ou mais fontes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="4c368-108">Esse recurso suporta o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4c368-108">This resource supports the following:</span></span>
* <span data-ttu-id="4c368-109">Adicionar seus dados como propriedades personalizadas em [extensões abertas](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="4c368-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="4c368-110">Assinar as [notificações de alteração](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="4c368-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
* <span data-ttu-id="4c368-111">Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.</span><span class="sxs-lookup"><span data-stu-id="4c368-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>


## <a name="methods"></a><span data-ttu-id="4c368-112">Methods</span><span class="sxs-lookup"><span data-stu-id="4c368-112">Methods</span></span>
|<span data-ttu-id="4c368-113">Método</span><span class="sxs-lookup"><span data-stu-id="4c368-113">Method</span></span>|<span data-ttu-id="4c368-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4c368-114">Return type</span></span>|<span data-ttu-id="4c368-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c368-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c368-116">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="4c368-116">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="4c368-117">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="4c368-117">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="4c368-118">Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.</span><span class="sxs-lookup"><span data-stu-id="4c368-118">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="4c368-119">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="4c368-119">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="4c368-120">todoTask</span><span class="sxs-lookup"><span data-stu-id="4c368-120">todoTask</span></span>](todotask.md)| <span data-ttu-id="4c368-121">Criar um [todoTask](todotask.md) na lista de tarefas especificada</span><span class="sxs-lookup"><span data-stu-id="4c368-121">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="4c368-122">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="4c368-122">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="4c368-123">todoTask</span><span class="sxs-lookup"><span data-stu-id="4c368-123">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="4c368-124">Leia as propriedades e os relacionamentos de um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="4c368-124">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="4c368-125">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="4c368-125">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="4c368-126">todoTask</span><span class="sxs-lookup"><span data-stu-id="4c368-126">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="4c368-127">Atualiza as propriedades de um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="4c368-127">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="4c368-128">Excluir tarefa</span><span class="sxs-lookup"><span data-stu-id="4c368-128">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="4c368-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c368-129">None</span></span>|<span data-ttu-id="4c368-130">Exclui um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="4c368-130">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="4c368-131">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="4c368-131">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="4c368-132">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="4c368-132">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="4c368-133">Obtenha o linkedResources da propriedade de navegação linkedResources.</span><span class="sxs-lookup"><span data-stu-id="4c368-133">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="4c368-134">Criar linkedResources</span><span class="sxs-lookup"><span data-stu-id="4c368-134">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="4c368-135">linkedResource</span><span class="sxs-lookup"><span data-stu-id="4c368-135">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="4c368-136">Criar um novo objeto linkedResources.</span><span class="sxs-lookup"><span data-stu-id="4c368-136">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c368-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c368-137">Properties</span></span>
|<span data-ttu-id="4c368-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c368-138">Property</span></span>|<span data-ttu-id="4c368-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c368-139">Type</span></span>|<span data-ttu-id="4c368-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c368-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c368-141">corpo</span><span class="sxs-lookup"><span data-stu-id="4c368-141">body</span></span>|[<span data-ttu-id="4c368-142">itemBody</span><span class="sxs-lookup"><span data-stu-id="4c368-142">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="4c368-143">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-143">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="4c368-144">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c368-144">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="4c368-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c368-145">DateTimeOffset</span></span>|<span data-ttu-id="4c368-146">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-146">The date and time when the task was last modified.</span></span> <span data-ttu-id="4c368-147">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="4c368-147">By default, it is in UTC.</span></span> <span data-ttu-id="4c368-148">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c368-148">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="4c368-149">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4c368-149">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c368-150">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="4c368-150">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="4c368-151">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c368-151">completedDateTime</span></span>|[<span data-ttu-id="4c368-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c368-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c368-153">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="4c368-153">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="4c368-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c368-154">createdDateTime</span></span>|<span data-ttu-id="4c368-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c368-155">DateTimeOffset</span></span>|<span data-ttu-id="4c368-156">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-156">The date and time when the task was created.</span></span> <span data-ttu-id="4c368-157">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="4c368-157">By default, it is in UTC.</span></span> <span data-ttu-id="4c368-158">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c368-158">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="4c368-159">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="4c368-159">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="4c368-160">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="4c368-160">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="4c368-161">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4c368-161">dueDateTime</span></span>|[<span data-ttu-id="4c368-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c368-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c368-163">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="4c368-163">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="4c368-164">id</span><span class="sxs-lookup"><span data-stu-id="4c368-164">id</span></span>|<span data-ttu-id="4c368-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c368-165">String</span></span>|<span data-ttu-id="4c368-166">Identificador exclusivo para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-166">Unique identifier for the task.</span></span> <span data-ttu-id="4c368-167">Por padrão, esse valor é alterado quando o item é movido de uma lista para outra.</span><span class="sxs-lookup"><span data-stu-id="4c368-167">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="4c368-168">importância</span><span class="sxs-lookup"><span data-stu-id="4c368-168">importance</span></span>|<span data-ttu-id="4c368-169">importância</span><span class="sxs-lookup"><span data-stu-id="4c368-169">importance</span></span>|<span data-ttu-id="4c368-170">A importância da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-170">The importance of the task.</span></span> <span data-ttu-id="4c368-171">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4c368-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="4c368-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="4c368-172">isReminderOn</span></span>|<span data-ttu-id="4c368-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="4c368-173">Boolean</span></span>|<span data-ttu-id="4c368-174">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="4c368-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c368-175">lastModifiedDateTime</span></span>|<span data-ttu-id="4c368-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c368-176">DateTimeOffset</span></span>|<span data-ttu-id="4c368-177">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="4c368-178">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="4c368-178">By default, it is in UTC.</span></span> <span data-ttu-id="4c368-179">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c368-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="4c368-180">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4c368-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c368-181">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="4c368-181">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="4c368-182">recurrence</span><span class="sxs-lookup"><span data-stu-id="4c368-182">recurrence</span></span>|[<span data-ttu-id="4c368-183">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4c368-183">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="4c368-184">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-184">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="4c368-185">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="4c368-185">reminderDateTime</span></span>|[<span data-ttu-id="4c368-186">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4c368-186">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="4c368-187">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-187">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="4c368-188">status</span><span class="sxs-lookup"><span data-stu-id="4c368-188">status</span></span>|<span data-ttu-id="4c368-189">taskStatus</span><span class="sxs-lookup"><span data-stu-id="4c368-189">taskStatus</span></span>|<span data-ttu-id="4c368-190">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-190">Indicates the state or progress of the task.</span></span> <span data-ttu-id="4c368-191">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="4c368-191">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="4c368-192">title</span><span class="sxs-lookup"><span data-stu-id="4c368-192">title</span></span>|<span data-ttu-id="4c368-193">String</span><span class="sxs-lookup"><span data-stu-id="4c368-193">String</span></span>|<span data-ttu-id="4c368-194">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-194">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c368-195">Relações</span><span class="sxs-lookup"><span data-stu-id="4c368-195">Relationships</span></span>
|<span data-ttu-id="4c368-196">Relação</span><span class="sxs-lookup"><span data-stu-id="4c368-196">Relationship</span></span>|<span data-ttu-id="4c368-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c368-197">Type</span></span>|<span data-ttu-id="4c368-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c368-198">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c368-199">extensions</span><span class="sxs-lookup"><span data-stu-id="4c368-199">extensions</span></span>|<span data-ttu-id="4c368-200">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="4c368-200">[extension](extension.md) collection</span></span>| <span data-ttu-id="4c368-201">A coleção de extensões abertas definidas para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-201">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="4c368-202">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4c368-202">Nullable.</span></span>|
|<span data-ttu-id="4c368-203">linkedResources</span><span class="sxs-lookup"><span data-stu-id="4c368-203">linkedResources</span></span>|<span data-ttu-id="4c368-204">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="4c368-204">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="4c368-205">Uma coleção de recursos vinculados à tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c368-205">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4c368-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c368-206">JSON representation</span></span>
<span data-ttu-id="4c368-207">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c368-207">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTask",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "isReminderOn": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "title": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)"
}
```



