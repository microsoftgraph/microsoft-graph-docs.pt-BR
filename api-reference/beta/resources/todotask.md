---
title: tipo de recurso todoTask
description: Um recurso todoTask controla um item de trabalho.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 58859f2781ecec713e547340606411302232ec06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003490"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="2adf3-103">tipo de recurso todoTask</span><span class="sxs-lookup"><span data-stu-id="2adf3-103">todoTask resource type</span></span>

<span data-ttu-id="2adf3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2adf3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2adf3-105">Um **todoTask** representa uma tarefa, como uma parte do trabalho ou item pessoal, que pode ser controlada e concluída.</span><span class="sxs-lookup"><span data-stu-id="2adf3-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="2adf3-106">Um **todoTask** está sempre contido em um [todoTaskList](todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="2adf3-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="2adf3-107">Ele inclui uma relação com uma coleção de objetos [linkedResource](./linkedResource.md) , controlando uma ou mais fontes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="2adf3-108">Esse recurso suporta o seguinte:</span><span class="sxs-lookup"><span data-stu-id="2adf3-108">This resource supports the following:</span></span>
* <span data-ttu-id="2adf3-109">Adicionar seus dados como propriedades personalizadas em [extensões abertas](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="2adf3-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="2adf3-110">Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.</span><span class="sxs-lookup"><span data-stu-id="2adf3-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="2adf3-111">Methods</span><span class="sxs-lookup"><span data-stu-id="2adf3-111">Methods</span></span>
|<span data-ttu-id="2adf3-112">Método</span><span class="sxs-lookup"><span data-stu-id="2adf3-112">Method</span></span>|<span data-ttu-id="2adf3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2adf3-113">Return type</span></span>|<span data-ttu-id="2adf3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adf3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2adf3-115">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="2adf3-115">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="2adf3-116">coleção [todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="2adf3-116">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="2adf3-117">Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.</span><span class="sxs-lookup"><span data-stu-id="2adf3-117">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="2adf3-118">Criar tarefa</span><span class="sxs-lookup"><span data-stu-id="2adf3-118">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="2adf3-119">todoTask</span><span class="sxs-lookup"><span data-stu-id="2adf3-119">todoTask</span></span>](todotask.md)| <span data-ttu-id="2adf3-120">Criar um [todoTask](todotask.md) na lista de tarefas especificada</span><span class="sxs-lookup"><span data-stu-id="2adf3-120">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="2adf3-121">Obter tarefa</span><span class="sxs-lookup"><span data-stu-id="2adf3-121">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="2adf3-122">todoTask</span><span class="sxs-lookup"><span data-stu-id="2adf3-122">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="2adf3-123">Leia as propriedades e os relacionamentos de um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="2adf3-123">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="2adf3-124">Atualizar tarefa</span><span class="sxs-lookup"><span data-stu-id="2adf3-124">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="2adf3-125">todoTask</span><span class="sxs-lookup"><span data-stu-id="2adf3-125">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="2adf3-126">Atualiza as propriedades de um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="2adf3-126">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="2adf3-127">Excluir tarefa</span><span class="sxs-lookup"><span data-stu-id="2adf3-127">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="2adf3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2adf3-128">None</span></span>|<span data-ttu-id="2adf3-129">Exclui um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="2adf3-129">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="2adf3-130">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="2adf3-130">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="2adf3-131">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="2adf3-131">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="2adf3-132">Obtenha o linkedResources da propriedade de navegação linkedResources.</span><span class="sxs-lookup"><span data-stu-id="2adf3-132">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="2adf3-133">Criar linkedResources</span><span class="sxs-lookup"><span data-stu-id="2adf3-133">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="2adf3-134">linkedResource</span><span class="sxs-lookup"><span data-stu-id="2adf3-134">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="2adf3-135">Criar um novo objeto linkedResources.</span><span class="sxs-lookup"><span data-stu-id="2adf3-135">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2adf3-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2adf3-136">Properties</span></span>
|<span data-ttu-id="2adf3-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2adf3-137">Property</span></span>|<span data-ttu-id="2adf3-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="2adf3-138">Type</span></span>|<span data-ttu-id="2adf3-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adf3-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2adf3-140">corpo</span><span class="sxs-lookup"><span data-stu-id="2adf3-140">body</span></span>|[<span data-ttu-id="2adf3-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="2adf3-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="2adf3-142">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-142">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="2adf3-143">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2adf3-143">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="2adf3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2adf3-144">DateTimeOffset</span></span>|<span data-ttu-id="2adf3-145">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-145">The date and time when the task was last modified.</span></span> <span data-ttu-id="2adf3-146">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="2adf3-146">By default, it is in UTC.</span></span> <span data-ttu-id="2adf3-147">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2adf3-147">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="2adf3-148">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2adf3-148">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2adf3-149">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="2adf3-149">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="2adf3-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2adf3-150">completedDateTime</span></span>|[<span data-ttu-id="2adf3-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2adf3-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2adf3-152">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="2adf3-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="2adf3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2adf3-153">createdDateTime</span></span>|<span data-ttu-id="2adf3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2adf3-154">DateTimeOffset</span></span>|<span data-ttu-id="2adf3-155">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-155">The date and time when the task was created.</span></span> <span data-ttu-id="2adf3-156">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="2adf3-156">By default, it is in UTC.</span></span> <span data-ttu-id="2adf3-157">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2adf3-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="2adf3-158">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="2adf3-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="2adf3-159">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="2adf3-159">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="2adf3-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2adf3-160">dueDateTime</span></span>|[<span data-ttu-id="2adf3-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2adf3-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2adf3-162">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="2adf3-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="2adf3-163">id</span><span class="sxs-lookup"><span data-stu-id="2adf3-163">id</span></span>|<span data-ttu-id="2adf3-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2adf3-164">String</span></span>|<span data-ttu-id="2adf3-165">Identificador exclusivo para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-165">Unique identifier for the task.</span></span> <span data-ttu-id="2adf3-166">Por padrão, esse valor é alterado quando o item é movido de uma lista para outra.</span><span class="sxs-lookup"><span data-stu-id="2adf3-166">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="2adf3-167">importância</span><span class="sxs-lookup"><span data-stu-id="2adf3-167">importance</span></span>|<span data-ttu-id="2adf3-168">importância</span><span class="sxs-lookup"><span data-stu-id="2adf3-168">importance</span></span>|<span data-ttu-id="2adf3-169">A importância da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-169">The importance of the task.</span></span> <span data-ttu-id="2adf3-170">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2adf3-170">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="2adf3-171">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="2adf3-171">isReminderOn</span></span>|<span data-ttu-id="2adf3-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="2adf3-172">Boolean</span></span>|<span data-ttu-id="2adf3-173">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-173">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="2adf3-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2adf3-174">lastModifiedDateTime</span></span>|<span data-ttu-id="2adf3-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2adf3-175">DateTimeOffset</span></span>|<span data-ttu-id="2adf3-176">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-176">The date and time when the task was last modified.</span></span> <span data-ttu-id="2adf3-177">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="2adf3-177">By default, it is in UTC.</span></span> <span data-ttu-id="2adf3-178">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2adf3-178">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="2adf3-179">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2adf3-179">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2adf3-180">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="2adf3-180">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="2adf3-181">recorrência</span><span class="sxs-lookup"><span data-stu-id="2adf3-181">recurrence</span></span>|[<span data-ttu-id="2adf3-182">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="2adf3-182">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="2adf3-183">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-183">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="2adf3-184">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="2adf3-184">reminderDateTime</span></span>|[<span data-ttu-id="2adf3-185">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2adf3-185">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2adf3-186">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-186">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="2adf3-187">status</span><span class="sxs-lookup"><span data-stu-id="2adf3-187">status</span></span>|<span data-ttu-id="2adf3-188">taskStatus</span><span class="sxs-lookup"><span data-stu-id="2adf3-188">taskStatus</span></span>|<span data-ttu-id="2adf3-189">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-189">Indicates the state or progress of the task.</span></span> <span data-ttu-id="2adf3-190">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="2adf3-190">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="2adf3-191">title</span><span class="sxs-lookup"><span data-stu-id="2adf3-191">title</span></span>|<span data-ttu-id="2adf3-192">String</span><span class="sxs-lookup"><span data-stu-id="2adf3-192">String</span></span>|<span data-ttu-id="2adf3-193">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-193">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2adf3-194">Relações</span><span class="sxs-lookup"><span data-stu-id="2adf3-194">Relationships</span></span>
|<span data-ttu-id="2adf3-195">Relação</span><span class="sxs-lookup"><span data-stu-id="2adf3-195">Relationship</span></span>|<span data-ttu-id="2adf3-196">Tipo</span><span class="sxs-lookup"><span data-stu-id="2adf3-196">Type</span></span>|<span data-ttu-id="2adf3-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adf3-197">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2adf3-198">extensions</span><span class="sxs-lookup"><span data-stu-id="2adf3-198">extensions</span></span>|<span data-ttu-id="2adf3-199">[extension](extension.md) collection</span><span class="sxs-lookup"><span data-stu-id="2adf3-199">[extension](extension.md) collection</span></span>| <span data-ttu-id="2adf3-200">A coleção de extensões abertas definidas para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-200">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="2adf3-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2adf3-201">Nullable.</span></span>|
|<span data-ttu-id="2adf3-202">linkedResources</span><span class="sxs-lookup"><span data-stu-id="2adf3-202">linkedResources</span></span>|<span data-ttu-id="2adf3-203">coleção [linkedResource](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="2adf3-203">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="2adf3-204">Uma coleção de recursos vinculados à tarefa.</span><span class="sxs-lookup"><span data-stu-id="2adf3-204">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2adf3-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2adf3-205">JSON representation</span></span>
<span data-ttu-id="2adf3-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2adf3-206">The following is a JSON representation of the resource.</span></span>
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



