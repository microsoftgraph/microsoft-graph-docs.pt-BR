---
title: Atualizar todoTask
description: Atualizar as propriedades de um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ffc7d5c90d2ec88638e35456ff74a2c48e3f1dc4
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873931"
---
# <a name="update-todotask"></a><span data-ttu-id="26e00-103">Atualizar todoTask</span><span class="sxs-lookup"><span data-stu-id="26e00-103">Update todoTask</span></span>
<span data-ttu-id="26e00-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="26e00-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="26e00-105">Atualizar as propriedades de um [objeto todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="26e00-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26e00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26e00-106">Permissions</span></span>
<span data-ttu-id="26e00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26e00-109">Permission type</span></span>|<span data-ttu-id="26e00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26e00-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26e00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26e00-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e00-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="26e00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26e00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e00-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e00-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="26e00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26e00-115">Application</span></span>|<span data-ttu-id="26e00-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="26e00-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26e00-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="26e00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26e00-118">Request headers</span></span>
|<span data-ttu-id="26e00-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26e00-119">Name</span></span>|<span data-ttu-id="26e00-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e00-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26e00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26e00-121">Authorization</span></span>|<span data-ttu-id="26e00-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26e00-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="26e00-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26e00-124">Content-Type</span></span>|<span data-ttu-id="26e00-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26e00-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26e00-127">Request body</span></span>
<span data-ttu-id="26e00-128">No corpo da solicitação, fornece uma representação JSON do [objeto todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="26e00-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="26e00-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTask](../resources/todotask.md).</span><span class="sxs-lookup"><span data-stu-id="26e00-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="26e00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26e00-130">Property</span></span>|<span data-ttu-id="26e00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26e00-131">Type</span></span>|<span data-ttu-id="26e00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e00-133">id</span><span class="sxs-lookup"><span data-stu-id="26e00-133">id</span></span>|<span data-ttu-id="26e00-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26e00-134">String</span></span>|<span data-ttu-id="26e00-135">O identificador exclusivo da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-135">The unique identifier of the task.</span></span> <span data-ttu-id="26e00-136">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="26e00-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="26e00-137">body</span><span class="sxs-lookup"><span data-stu-id="26e00-137">body</span></span>|[<span data-ttu-id="26e00-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="26e00-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="26e00-139">Corpo da tarefa que normalmente contém informações sobre a tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="26e00-140">Observe para qual tipo de HTML há suporte.</span><span class="sxs-lookup"><span data-stu-id="26e00-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="26e00-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="26e00-141">completedDateTime</span></span>|[<span data-ttu-id="26e00-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="26e00-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="26e00-143">A data no fuso horário especificado que a tarefa foi concluída.</span><span class="sxs-lookup"><span data-stu-id="26e00-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="26e00-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="26e00-144">dueDateTime</span></span>|[<span data-ttu-id="26e00-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="26e00-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="26e00-146">A data no fuso horário especificado que a tarefa será concluída.</span><span class="sxs-lookup"><span data-stu-id="26e00-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="26e00-147">importância</span><span class="sxs-lookup"><span data-stu-id="26e00-147">importance</span></span>|<span data-ttu-id="26e00-148">importância</span><span class="sxs-lookup"><span data-stu-id="26e00-148">importance</span></span>|<span data-ttu-id="26e00-149">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="26e00-149">The importance of the event.</span></span> <span data-ttu-id="26e00-150">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="26e00-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="26e00-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="26e00-151">isReminderOn</span></span>|<span data-ttu-id="26e00-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="26e00-152">Boolean</span></span>|<span data-ttu-id="26e00-153">Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="26e00-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="26e00-154">recurrence</span></span>|[<span data-ttu-id="26e00-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="26e00-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="26e00-156">O padrão de recorrência da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="26e00-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="26e00-157">reminderDateTime</span></span>|[<span data-ttu-id="26e00-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="26e00-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="26e00-159">A data e hora do alerta de lembrete da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="26e00-160">status</span><span class="sxs-lookup"><span data-stu-id="26e00-160">status</span></span>|<span data-ttu-id="26e00-161">taskStatus</span><span class="sxs-lookup"><span data-stu-id="26e00-161">taskStatus</span></span>|<span data-ttu-id="26e00-162">Indica o estado ou o progresso da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="26e00-163">Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span><span class="sxs-lookup"><span data-stu-id="26e00-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="26e00-164">title</span><span class="sxs-lookup"><span data-stu-id="26e00-164">title</span></span>|<span data-ttu-id="26e00-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26e00-165">String</span></span>|<span data-ttu-id="26e00-166">Uma breve descrição da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-166">A brief description of the task.</span></span>|
|<span data-ttu-id="26e00-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26e00-167">createdDateTime</span></span>|<span data-ttu-id="26e00-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e00-168">DateTimeOffset</span></span>|<span data-ttu-id="26e00-169">A data e a hora da criação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-169">The date and time when the task was created.</span></span> <span data-ttu-id="26e00-170">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="26e00-170">By default, it is in UTC.</span></span> <span data-ttu-id="26e00-171">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26e00-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="26e00-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26e00-172">lastModifiedDateTime</span></span>|<span data-ttu-id="26e00-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e00-173">DateTimeOffset</span></span>|<span data-ttu-id="26e00-174">A data e hora da última modificação da tarefa.</span><span class="sxs-lookup"><span data-stu-id="26e00-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="26e00-175">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="26e00-175">By default, it is in UTC.</span></span> <span data-ttu-id="26e00-176">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26e00-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="26e00-177">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26e00-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="26e00-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e00-178">DateTimeOffset</span></span>|<span data-ttu-id="26e00-179">A data e a hora em que o corpo da tarefa foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="26e00-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="26e00-180">Por padrão, está definida em UTC.</span><span class="sxs-lookup"><span data-stu-id="26e00-180">By default, it is in UTC.</span></span> <span data-ttu-id="26e00-181">Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26e00-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="26e00-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="26e00-182">Response</span></span>

<span data-ttu-id="26e00-183">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [todoTask](../resources/todotask.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26e00-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26e00-184">Exemplos</span><span class="sxs-lookup"><span data-stu-id="26e00-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26e00-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26e00-185">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="26e00-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="26e00-186">HTTP</span></span>](#tab/http)
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
   "dueDateTime":{
      "dateTime":"2020-07-25T16:00:00",
      "timeZone":"Eastern Standard Time"
   }
}
```
# <a name="javascript"></a>[<span data-ttu-id="26e00-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26e00-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="26e00-188">C#</span><span class="sxs-lookup"><span data-stu-id="26e00-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26e00-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26e00-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26e00-190">Java</span><span class="sxs-lookup"><span data-stu-id="26e00-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="26e00-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="26e00-191">Response</span></span>
<span data-ttu-id="26e00-192">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26e00-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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



