---
title: Criar todoTask
description: Crie um novo objeto task em um todoTaskList especificado.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2fcca012cfb1b7e569296cbb892e1f523f7f257a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873525"
---
# <a name="create-todotask"></a><span data-ttu-id="72269-103">Criar todoTask</span><span class="sxs-lookup"><span data-stu-id="72269-103">Create todoTask</span></span>
<span data-ttu-id="72269-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72269-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72269-105">Criar um novo objeto task em um [todoTaskList especificado.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="72269-105">Create a new task object in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72269-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72269-106">Permissions</span></span>
<span data-ttu-id="72269-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72269-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72269-109">Permission type</span></span>|<span data-ttu-id="72269-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72269-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72269-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72269-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72269-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72269-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="72269-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72269-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72269-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72269-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="72269-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72269-115">Application</span></span>|<span data-ttu-id="72269-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72269-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72269-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72269-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="72269-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72269-118">Request headers</span></span>
|<span data-ttu-id="72269-119">Nome</span><span class="sxs-lookup"><span data-stu-id="72269-119">Name</span></span>|<span data-ttu-id="72269-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="72269-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72269-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="72269-121">Authorization</span></span>|<span data-ttu-id="72269-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72269-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="72269-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72269-124">Content-Type</span></span>|<span data-ttu-id="72269-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72269-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72269-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72269-127">Request body</span></span>
<span data-ttu-id="72269-128">No corpo da solicitação, fornece uma representação JSON do [objeto todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="72269-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="72269-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTask](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="72269-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="72269-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72269-130">Property</span></span>|<span data-ttu-id="72269-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="72269-131">Type</span></span>|<span data-ttu-id="72269-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="72269-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72269-133">id</span><span class="sxs-lookup"><span data-stu-id="72269-133">id</span></span>|<span data-ttu-id="72269-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72269-134">String</span></span>|<span data-ttu-id="72269-135">Identificador exclusivo para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-135">Unique identifier for the task.</span></span> <span data-ttu-id="72269-136">Por padrão, esse valor muda quando o item é movido de uma lista para outra.</span><span class="sxs-lookup"><span data-stu-id="72269-136">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="72269-137">body</span><span class="sxs-lookup"><span data-stu-id="72269-137">body</span></span>|[<span data-ttu-id="72269-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="72269-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="72269-139">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-139">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="72269-140">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="72269-140">completedDateTime</span></span>|[<span data-ttu-id="72269-141">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="72269-141">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="72269-142">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="72269-142">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="72269-143">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="72269-143">dueDateTime</span></span>|[<span data-ttu-id="72269-144">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="72269-144">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="72269-145">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="72269-145">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="72269-146">importância</span><span class="sxs-lookup"><span data-stu-id="72269-146">importance</span></span>|<span data-ttu-id="72269-147">importância</span><span class="sxs-lookup"><span data-stu-id="72269-147">importance</span></span>|<span data-ttu-id="72269-148">A importância da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-148">The importance of the task.</span></span> <span data-ttu-id="72269-149">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="72269-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="72269-150">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="72269-150">isReminderOn</span></span>|<span data-ttu-id="72269-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="72269-151">Boolean</span></span>|<span data-ttu-id="72269-152">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-152">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="72269-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="72269-153">recurrence</span></span>|[<span data-ttu-id="72269-154">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="72269-154">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="72269-155">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-155">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="72269-156">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="72269-156">reminderDateTime</span></span>|[<span data-ttu-id="72269-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="72269-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="72269-158">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-158">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="72269-159">status</span><span class="sxs-lookup"><span data-stu-id="72269-159">status</span></span>|<span data-ttu-id="72269-160">taskStatus</span><span class="sxs-lookup"><span data-stu-id="72269-160">taskStatus</span></span>|<span data-ttu-id="72269-161">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-161">Indicates the state or progress of the task.</span></span> <span data-ttu-id="72269-162">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="72269-162">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="72269-163">title</span><span class="sxs-lookup"><span data-stu-id="72269-163">title</span></span>|<span data-ttu-id="72269-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72269-164">String</span></span>|<span data-ttu-id="72269-165">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-165">A brief description of the task.</span></span>|
|<span data-ttu-id="72269-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72269-166">createdDateTime</span></span>|<span data-ttu-id="72269-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72269-167">DateTimeOffset</span></span>|<span data-ttu-id="72269-168">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-168">The date and time when the task was created.</span></span> <span data-ttu-id="72269-169">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="72269-169">By default, it is in UTC.</span></span> <span data-ttu-id="72269-170">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72269-170">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="72269-171">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="72269-171">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="72269-172">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="72269-172">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="72269-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72269-173">lastModifiedDateTime</span></span>|<span data-ttu-id="72269-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72269-174">DateTimeOffset</span></span>|<span data-ttu-id="72269-175">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="72269-176">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="72269-176">By default, it is in UTC.</span></span> <span data-ttu-id="72269-177">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72269-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="72269-178">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="72269-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72269-179">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="72269-179">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="72269-180">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72269-180">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="72269-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72269-181">DateTimeOffset</span></span>|<span data-ttu-id="72269-182">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="72269-182">The date and time when the task was last modified.</span></span> <span data-ttu-id="72269-183">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="72269-183">By default, it is in UTC.</span></span> <span data-ttu-id="72269-184">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72269-184">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="72269-185">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="72269-185">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72269-186">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="72269-186">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|



## <a name="response"></a><span data-ttu-id="72269-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="72269-187">Response</span></span>

<span data-ttu-id="72269-188">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72269-188">If successful, this method returns a `201 Created` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72269-189">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72269-189">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72269-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72269-190">Request</span></span>
<span data-ttu-id="72269-191">O exemplo a seguir cria **um todoTask** na lista de tarefas especificada e inclui um [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="72269-191">The following example creates a **todoTask** in the specified task list, and includes a [linkedResource](../resources/linkedresource.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="72269-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="72269-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"],
  "name": "create_todotask_from_tasks"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks
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
# <a name="c"></a>[<span data-ttu-id="72269-193">C#</span><span class="sxs-lookup"><span data-stu-id="72269-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotask-from-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72269-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72269-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotask-from-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72269-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72269-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotask-from-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72269-196">Java</span><span class="sxs-lookup"><span data-stu-id="72269-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotask-from-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="72269-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="72269-197">Response</span></span>
<span data-ttu-id="72269-198">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72269-198">**Note:** The response object shown here might be shortened for readability.</span></span>
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



