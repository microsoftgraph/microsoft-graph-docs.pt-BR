---
title: Listar tarefas
description: Obter todas as tarefas do Outlook na pasta especificada.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3e04d42e851fcd6dc37f8251a9c40698de471fab
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457984"
---
# <a name="list-tasks-deprecated"></a><span data-ttu-id="bde1a-103">Listar tarefas (preterido)</span><span class="sxs-lookup"><span data-stu-id="bde1a-103">List tasks (deprecated)</span></span>

<span data-ttu-id="bde1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bde1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="bde1a-105">Obter todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="bde1a-105">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="bde1a-106">Por padrão, essa operação (e as operações de POST, PATCH e tarefa [completa](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="bde1a-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="bde1a-107">Você pode usar um `Prefer: outlook.timezone` cabeçalho de solicitação para ter todas as propriedades relacionadas à data na resposta representada em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="bde1a-107">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="bde1a-108">Veja um [exemplo](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) para obter uma única tarefa.</span><span class="sxs-lookup"><span data-stu-id="bde1a-108">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="bde1a-109">Você pode aplicar o cabeçalho de forma semelhante para obter várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="bde1a-109">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="bde1a-110">Se houver mais de um grupo de tarefas e você quiser obter todas as tarefas em um grupo de tarefas específico, primeiro [obtenha todas as pastas de tarefas desse grupo de tarefas](outlooktaskgroup-list-taskfolders.md)e, em seguida, obtenha as tarefas em cada uma dessas pastas de tarefas.</span><span class="sxs-lookup"><span data-stu-id="bde1a-110">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="bde1a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="bde1a-111">Permissions</span></span>
<span data-ttu-id="bde1a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bde1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bde1a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bde1a-114">Permission type</span></span>      | <span data-ttu-id="bde1a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bde1a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bde1a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bde1a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bde1a-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bde1a-117">Tasks.Read</span></span>    |
|<span data-ttu-id="bde1a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bde1a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bde1a-119">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="bde1a-119">Tasks.Read</span></span>    |
|<span data-ttu-id="bde1a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bde1a-120">Application</span></span> | <span data-ttu-id="bde1a-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bde1a-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bde1a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bde1a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bde1a-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bde1a-123">Optional query parameters</span></span>
<span data-ttu-id="bde1a-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bde1a-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bde1a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bde1a-125">Request headers</span></span>
| <span data-ttu-id="bde1a-126">Nome</span><span class="sxs-lookup"><span data-stu-id="bde1a-126">Name</span></span>      |<span data-ttu-id="bde1a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="bde1a-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bde1a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="bde1a-128">Authorization</span></span>  | <span data-ttu-id="bde1a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bde1a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bde1a-131">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bde1a-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="bde1a-132">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="bde1a-132">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="bde1a-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bde1a-133">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bde1a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bde1a-134">Request body</span></span>
<span data-ttu-id="bde1a-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bde1a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bde1a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bde1a-136">Response</span></span>

<span data-ttu-id="bde1a-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bde1a-137">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bde1a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bde1a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bde1a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bde1a-139">Request</span></span>
<span data-ttu-id="bde1a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bde1a-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bde1a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bde1a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlooktaskfolder_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
# <a name="c"></a>[<span data-ttu-id="bde1a-142">C#</span><span class="sxs-lookup"><span data-stu-id="bde1a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlooktaskfolder-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bde1a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bde1a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlooktaskfolder-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bde1a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bde1a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlooktaskfolder-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bde1a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bde1a-145">Response</span></span>
<span data-ttu-id="bde1a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bde1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
   {
      "id": "AAMkADA1MTrfAAA=",
      "createdDateTime": "2016-04-22T05:44:01.2012012Z",
      "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-25T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-23T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    },
    {
      "id": "AAMkADA1MTrgAAA=",
      "createdDateTime": "2016-04-22T06:03:35.9279794Z",
      "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-27T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-26T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
