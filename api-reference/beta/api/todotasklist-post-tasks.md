---
title: Criar todoTask
description: Criar um novo objeto Task em um todoTaskList especificado.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 457a855f7746ce2ce4924f03e6a7862be4bce41f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849834"
---
# <a name="create-todotask"></a><span data-ttu-id="61405-103">Criar todoTask</span><span class="sxs-lookup"><span data-stu-id="61405-103">Create todoTask</span></span>
<span data-ttu-id="61405-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="61405-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="61405-105">Criar um novo objeto Task em um [todoTaskList](../resources/todotasklist.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="61405-105">Create a new task object in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="61405-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61405-106">Permissions</span></span>
<span data-ttu-id="61405-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61405-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61405-109">Permission type</span></span>|<span data-ttu-id="61405-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61405-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61405-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61405-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61405-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61405-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="61405-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61405-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61405-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61405-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="61405-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61405-115">Application</span></span>|<span data-ttu-id="61405-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61405-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61405-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61405-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="61405-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61405-118">Request headers</span></span>
|<span data-ttu-id="61405-119">Nome</span><span class="sxs-lookup"><span data-stu-id="61405-119">Name</span></span>|<span data-ttu-id="61405-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="61405-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61405-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="61405-121">Authorization</span></span>|<span data-ttu-id="61405-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61405-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="61405-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61405-124">Content-Type</span></span>|<span data-ttu-id="61405-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61405-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61405-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61405-127">Request body</span></span>
<span data-ttu-id="61405-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="61405-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="61405-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTask](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="61405-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="61405-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61405-130">Property</span></span>|<span data-ttu-id="61405-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61405-131">Type</span></span>|<span data-ttu-id="61405-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61405-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61405-133">id</span><span class="sxs-lookup"><span data-stu-id="61405-133">id</span></span>|<span data-ttu-id="61405-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61405-134">String</span></span>|<span data-ttu-id="61405-135">Identificador exclusivo para a tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-135">Unique identifier for the task.</span></span> <span data-ttu-id="61405-136">Por padrão, esse valor é alterado quando o item é movido de uma lista para outra.</span><span class="sxs-lookup"><span data-stu-id="61405-136">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="61405-137">corpo</span><span class="sxs-lookup"><span data-stu-id="61405-137">body</span></span>|[<span data-ttu-id="61405-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="61405-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="61405-139">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-139">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="61405-140">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="61405-140">completedDateTime</span></span>|[<span data-ttu-id="61405-141">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61405-141">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="61405-142">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="61405-142">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="61405-143">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="61405-143">dueDateTime</span></span>|[<span data-ttu-id="61405-144">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61405-144">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="61405-145">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="61405-145">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="61405-146">importância</span><span class="sxs-lookup"><span data-stu-id="61405-146">importance</span></span>|<span data-ttu-id="61405-147">importância</span><span class="sxs-lookup"><span data-stu-id="61405-147">importance</span></span>|<span data-ttu-id="61405-148">A importância da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-148">The importance of the task.</span></span> <span data-ttu-id="61405-149">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="61405-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="61405-150">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="61405-150">isReminderOn</span></span>|<span data-ttu-id="61405-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="61405-151">Boolean</span></span>|<span data-ttu-id="61405-152">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-152">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="61405-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="61405-153">recurrence</span></span>|[<span data-ttu-id="61405-154">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="61405-154">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="61405-155">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-155">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="61405-156">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="61405-156">reminderDateTime</span></span>|[<span data-ttu-id="61405-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61405-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="61405-158">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-158">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="61405-159">status</span><span class="sxs-lookup"><span data-stu-id="61405-159">status</span></span>|<span data-ttu-id="61405-160">taskStatus</span><span class="sxs-lookup"><span data-stu-id="61405-160">taskStatus</span></span>|<span data-ttu-id="61405-161">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-161">Indicates the state or progress of the task.</span></span> <span data-ttu-id="61405-162">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="61405-162">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="61405-163">title</span><span class="sxs-lookup"><span data-stu-id="61405-163">title</span></span>|<span data-ttu-id="61405-164">String</span><span class="sxs-lookup"><span data-stu-id="61405-164">String</span></span>|<span data-ttu-id="61405-165">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-165">A brief description of the task.</span></span>|
|<span data-ttu-id="61405-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61405-166">createdDateTime</span></span>|<span data-ttu-id="61405-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61405-167">DateTimeOffset</span></span>|<span data-ttu-id="61405-168">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-168">The date and time when the task was created.</span></span> <span data-ttu-id="61405-169">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="61405-169">By default, it is in UTC.</span></span> <span data-ttu-id="61405-170">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61405-170">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="61405-171">O valor da propriedade usa o formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="61405-171">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="61405-172">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="61405-172">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="61405-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61405-173">lastModifiedDateTime</span></span>|<span data-ttu-id="61405-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61405-174">DateTimeOffset</span></span>|<span data-ttu-id="61405-175">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="61405-176">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="61405-176">By default, it is in UTC.</span></span> <span data-ttu-id="61405-177">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61405-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="61405-178">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="61405-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61405-179">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="61405-179">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="61405-180">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61405-180">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="61405-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61405-181">DateTimeOffset</span></span>|<span data-ttu-id="61405-182">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="61405-182">The date and time when the task was last modified.</span></span> <span data-ttu-id="61405-183">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="61405-183">By default, it is in UTC.</span></span> <span data-ttu-id="61405-184">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61405-184">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="61405-185">O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="61405-185">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61405-186">Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="61405-186">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|



## <a name="response"></a><span data-ttu-id="61405-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="61405-187">Response</span></span>

<span data-ttu-id="61405-188">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61405-188">If successful, this method returns a `201 Created` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61405-189">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61405-189">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61405-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61405-190">Request</span></span>
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
  "linkedResources": [{
            "webUrl": "http://microsoft.com",
            "applicationName": "Microsoft",
            "displayName": "Microsoft"
        }]
}
```


### <a name="response"></a><span data-ttu-id="61405-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="61405-191">Response</span></span>
<span data-ttu-id="61405-192">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="61405-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.etag": "W/\"xzyPKP0BiUGgld+lMKXwbQAAnBoTIw==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "A new task",
    "createdDateTime": "2020-08-18T09:03:05.8339192Z",
    "lastModifiedDateTime": "2020-08-18T09:03:06.0827766Z",
    "id": "AlMKXwbQAAAJws6wcAAAA=",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "linkedResources": [{
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
            "webUrl": "http://microsoft.com",
            "applicationName": "Microsoft",
            "displayName": "Microsoft"
        }]
}
```

