---
title: Atualizar todoTask
description: Atualiza as propriedades de um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 846e364161e2ca48d6a7733939c146ea543b3a2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058540"
---
# <a name="update-todotask"></a><span data-ttu-id="307ff-103">Atualizar todoTask</span><span class="sxs-lookup"><span data-stu-id="307ff-103">Update todoTask</span></span>
<span data-ttu-id="307ff-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="307ff-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="307ff-105">Atualiza as propriedades de um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="307ff-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="307ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="307ff-106">Permissions</span></span>
<span data-ttu-id="307ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="307ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="307ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="307ff-109">Permission type</span></span>|<span data-ttu-id="307ff-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="307ff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="307ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="307ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="307ff-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="307ff-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="307ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="307ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="307ff-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="307ff-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="307ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="307ff-115">Application</span></span>|<span data-ttu-id="307ff-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="307ff-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="307ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="307ff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="307ff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="307ff-118">Request headers</span></span>
|<span data-ttu-id="307ff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="307ff-119">Name</span></span>|<span data-ttu-id="307ff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="307ff-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="307ff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="307ff-121">Authorization</span></span>|<span data-ttu-id="307ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="307ff-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="307ff-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="307ff-124">Content-Type</span></span>|<span data-ttu-id="307ff-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="307ff-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="307ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="307ff-127">Request body</span></span>
<span data-ttu-id="307ff-128">No corpo da solicitação, forneça uma representação JSON do objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="307ff-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="307ff-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTask](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="307ff-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="307ff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="307ff-130">Property</span></span>|<span data-ttu-id="307ff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="307ff-131">Type</span></span>|<span data-ttu-id="307ff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="307ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="307ff-133">id</span><span class="sxs-lookup"><span data-stu-id="307ff-133">id</span></span>|<span data-ttu-id="307ff-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="307ff-134">String</span></span>|<span data-ttu-id="307ff-135">O identificador exclusivo da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-135">The unique identifier of the task.</span></span> <span data-ttu-id="307ff-136">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="307ff-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="307ff-137">body</span><span class="sxs-lookup"><span data-stu-id="307ff-137">body</span></span>|[<span data-ttu-id="307ff-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="307ff-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="307ff-139">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="307ff-140">Observe para qual tipo de HTML há suporte.</span><span class="sxs-lookup"><span data-stu-id="307ff-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="307ff-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="307ff-141">completedDateTime</span></span>|[<span data-ttu-id="307ff-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="307ff-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="307ff-143">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="307ff-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="307ff-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="307ff-144">dueDateTime</span></span>|[<span data-ttu-id="307ff-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="307ff-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="307ff-146">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="307ff-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="307ff-147">importance</span><span class="sxs-lookup"><span data-stu-id="307ff-147">importance</span></span>|<span data-ttu-id="307ff-148">importância</span><span class="sxs-lookup"><span data-stu-id="307ff-148">importance</span></span>|<span data-ttu-id="307ff-149">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="307ff-149">The importance of the event.</span></span> <span data-ttu-id="307ff-150">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="307ff-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="307ff-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="307ff-151">isReminderOn</span></span>|<span data-ttu-id="307ff-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="307ff-152">Boolean</span></span>|<span data-ttu-id="307ff-153">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="307ff-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="307ff-154">recurrence</span></span>|[<span data-ttu-id="307ff-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="307ff-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="307ff-156">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="307ff-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="307ff-157">reminderDateTime</span></span>|[<span data-ttu-id="307ff-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="307ff-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="307ff-159">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="307ff-160">status</span><span class="sxs-lookup"><span data-stu-id="307ff-160">status</span></span>|<span data-ttu-id="307ff-161">taskStatus</span><span class="sxs-lookup"><span data-stu-id="307ff-161">taskStatus</span></span>|<span data-ttu-id="307ff-162">Indica o estado ou o andamento da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="307ff-163">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="307ff-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="307ff-164">title</span><span class="sxs-lookup"><span data-stu-id="307ff-164">title</span></span>|<span data-ttu-id="307ff-165">String</span><span class="sxs-lookup"><span data-stu-id="307ff-165">String</span></span>|<span data-ttu-id="307ff-166">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-166">A brief description of the task.</span></span>|
|<span data-ttu-id="307ff-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="307ff-167">createdDateTime</span></span>|<span data-ttu-id="307ff-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="307ff-168">DateTimeOffset</span></span>|<span data-ttu-id="307ff-169">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-169">The date and time when the task was created.</span></span> <span data-ttu-id="307ff-170">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="307ff-170">By default, it is in UTC.</span></span> <span data-ttu-id="307ff-171">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="307ff-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="307ff-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="307ff-172">lastModifiedDateTime</span></span>|<span data-ttu-id="307ff-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="307ff-173">DateTimeOffset</span></span>|<span data-ttu-id="307ff-174">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="307ff-175">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="307ff-175">By default, it is in UTC.</span></span> <span data-ttu-id="307ff-176">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="307ff-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="307ff-177">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="307ff-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="307ff-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="307ff-178">DateTimeOffset</span></span>|<span data-ttu-id="307ff-179">A data e hora da última modificação do corpo da tarefa.</span><span class="sxs-lookup"><span data-stu-id="307ff-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="307ff-180">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="307ff-180">By default, it is in UTC.</span></span> <span data-ttu-id="307ff-181">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="307ff-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="307ff-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="307ff-182">Response</span></span>

<span data-ttu-id="307ff-183">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTask](../resources/todotask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="307ff-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="307ff-184">Exemplos</span><span class="sxs-lookup"><span data-stu-id="307ff-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="307ff-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="307ff-185">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="307ff-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="307ff-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_todotask",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
Content-Type: application/json
Content-length: 608

{
    "dueDateTime":
    {
        "dateTime":"2020-07-25T16:00:00",
        "timeZone":"Eastern Standard Time"
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="307ff-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="307ff-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="307ff-188">C#</span><span class="sxs-lookup"><span data-stu-id="307ff-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="307ff-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="307ff-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="307ff-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="307ff-190">Response</span></span>
<span data-ttu-id="307ff-191">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="307ff-191">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
   "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
   
```



