---
title: Criar todoTask
description: Criar um novo objeto Task em um todoTaskList especificado.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c8902d70c08ed6fdf16677f2388a26c4c76ea18e
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364373"
---
# <a name="create-todotask"></a><span data-ttu-id="55bde-103">Criar todoTask</span><span class="sxs-lookup"><span data-stu-id="55bde-103">Create todoTask</span></span>
<span data-ttu-id="55bde-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="55bde-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="55bde-105">Criar um novo objeto Task em um [todoTaskList](../resources/todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="55bde-105">Create a new task object in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55bde-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55bde-106">Permissions</span></span>
<span data-ttu-id="55bde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55bde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55bde-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55bde-109">Permission type</span></span>|<span data-ttu-id="55bde-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55bde-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55bde-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55bde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55bde-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55bde-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="55bde-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55bde-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55bde-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55bde-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="55bde-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55bde-115">Application</span></span>|<span data-ttu-id="55bde-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55bde-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55bde-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55bde-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="55bde-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55bde-118">Request headers</span></span>
|<span data-ttu-id="55bde-119">Nome</span><span class="sxs-lookup"><span data-stu-id="55bde-119">Name</span></span>|<span data-ttu-id="55bde-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55bde-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55bde-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55bde-121">Authorization</span></span>|<span data-ttu-id="55bde-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55bde-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="55bde-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55bde-124">Content-Type</span></span>|<span data-ttu-id="55bde-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55bde-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55bde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55bde-127">Request body</span></span>
<span data-ttu-id="55bde-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="55bde-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="55bde-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTask](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="55bde-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="55bde-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55bde-130">Property</span></span>|<span data-ttu-id="55bde-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55bde-131">Type</span></span>|<span data-ttu-id="55bde-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55bde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55bde-133">id</span><span class="sxs-lookup"><span data-stu-id="55bde-133">id</span></span>|<span data-ttu-id="55bde-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55bde-134">String</span></span>|<span data-ttu-id="55bde-135">Identificador exclusivo para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-135">Unique identifier for the task.</span></span> <span data-ttu-id="55bde-136">Por padrão, esse valor é alterado quando o item é movido de uma lista para outra.</span><span class="sxs-lookup"><span data-stu-id="55bde-136">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="55bde-137">body</span><span class="sxs-lookup"><span data-stu-id="55bde-137">body</span></span>|[<span data-ttu-id="55bde-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="55bde-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="55bde-139">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-139">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="55bde-140">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="55bde-140">completedDateTime</span></span>|[<span data-ttu-id="55bde-141">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="55bde-141">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="55bde-142">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="55bde-142">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="55bde-143">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="55bde-143">dueDateTime</span></span>|[<span data-ttu-id="55bde-144">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="55bde-144">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="55bde-145">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="55bde-145">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="55bde-146">importância</span><span class="sxs-lookup"><span data-stu-id="55bde-146">importance</span></span>|<span data-ttu-id="55bde-147">importância</span><span class="sxs-lookup"><span data-stu-id="55bde-147">importance</span></span>|<span data-ttu-id="55bde-148">A importância da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-148">The importance of the task.</span></span> <span data-ttu-id="55bde-149">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="55bde-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="55bde-150">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="55bde-150">isReminderOn</span></span>|<span data-ttu-id="55bde-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="55bde-151">Boolean</span></span>|<span data-ttu-id="55bde-152">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-152">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="55bde-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="55bde-153">recurrence</span></span>|[<span data-ttu-id="55bde-154">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="55bde-154">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="55bde-155">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-155">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="55bde-156">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="55bde-156">reminderDateTime</span></span>|[<span data-ttu-id="55bde-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="55bde-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="55bde-158">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-158">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="55bde-159">status</span><span class="sxs-lookup"><span data-stu-id="55bde-159">status</span></span>|<span data-ttu-id="55bde-160">taskStatus</span><span class="sxs-lookup"><span data-stu-id="55bde-160">taskStatus</span></span>|<span data-ttu-id="55bde-161">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-161">Indicates the state or progress of the task.</span></span> <span data-ttu-id="55bde-162">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="55bde-162">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="55bde-163">title</span><span class="sxs-lookup"><span data-stu-id="55bde-163">title</span></span>|<span data-ttu-id="55bde-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55bde-164">String</span></span>|<span data-ttu-id="55bde-165">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-165">A brief description of the task.</span></span>|
|<span data-ttu-id="55bde-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55bde-166">createdDateTime</span></span>|<span data-ttu-id="55bde-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55bde-167">DateTimeOffset</span></span>|<span data-ttu-id="55bde-168">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-168">The date and time when the task was created.</span></span> <span data-ttu-id="55bde-169">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="55bde-169">By default, it is in UTC.</span></span> <span data-ttu-id="55bde-170">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55bde-170">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="55bde-171">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="55bde-171">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="55bde-172">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="55bde-172">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="55bde-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55bde-173">lastModifiedDateTime</span></span>|<span data-ttu-id="55bde-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55bde-174">DateTimeOffset</span></span>|<span data-ttu-id="55bde-175">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="55bde-176">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="55bde-176">By default, it is in UTC.</span></span> <span data-ttu-id="55bde-177">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55bde-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="55bde-178">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="55bde-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55bde-179">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="55bde-179">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="55bde-180">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55bde-180">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="55bde-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55bde-181">DateTimeOffset</span></span>|<span data-ttu-id="55bde-182">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="55bde-182">The date and time when the task was last modified.</span></span> <span data-ttu-id="55bde-183">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="55bde-183">By default, it is in UTC.</span></span> <span data-ttu-id="55bde-184">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55bde-184">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="55bde-185">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="55bde-185">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55bde-186">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="55bde-186">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|



## <a name="response"></a><span data-ttu-id="55bde-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="55bde-187">Response</span></span>

<span data-ttu-id="55bde-188">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55bde-188">If successful, this method returns a `201 Created` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55bde-189">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55bde-189">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55bde-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55bde-190">Request</span></span>
<span data-ttu-id="55bde-191">O exemplo a seguir cria um **todoTask** na lista de tarefas especificada e inclui um [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="55bde-191">The following example creates a **todoTask** in the specified task list, and includes a [linkedResource](../resources/linkedresource.md).</span></span>

# <a name="http"></a>[<span data-ttu-id="55bde-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="55bde-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"],
  "name": "create_todotask_from_tasks"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks
Content-Type: application/json
Content-length: 608

{
   "title":"A new task",
   "linkedResources":[
      {
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="55bde-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55bde-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotask-from-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="55bde-194">C#</span><span class="sxs-lookup"><span data-stu-id="55bde-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotask-from-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55bde-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55bde-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotask-from-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="55bde-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="55bde-196">Response</span></span>
<span data-ttu-id="55bde-197">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55bde-197">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAnBoTIw==\"",
   "importance":"low",
   "isReminderOn":false,
   "status":"notStarted",
   "title":"A new task",
   "createdDateTime":"2020-08-18T09:03:05.8339192Z",
   "lastModifiedDateTime":"2020-08-18T09:03:06.0827766Z",
   "id":"AlMKXwbQAAAJws6wcAAAA=",
   "body":{
      "content":"",
      "contentType":"text"
   },
   "linkedResources":[
      {
         "id":"f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```



