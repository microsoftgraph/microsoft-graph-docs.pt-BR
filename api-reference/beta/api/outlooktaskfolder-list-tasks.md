---
title: Listar tarefas
description: Obter todas as tarefas do Outlook na pasta especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2e417489f41619843c5fc107fd13acd3eb38a469
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447240"
---
# <a name="list-tasks"></a><span data-ttu-id="c1a5b-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="c1a5b-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a5b-104">Obter todas as tarefas do Outlook na pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="c1a5b-105">Por padrão, essa operação (e as operações de POST, PATCH e tarefa [completa](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="c1a5b-106">Você pode usar um `Prefer: outlook.timezone` cabeçalho de solicitação para ter todas as propriedades relacionadas à data na resposta representada em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="c1a5b-107">Veja um [exemplo](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) para obter uma única tarefa.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="c1a5b-108">Você pode aplicar o cabeçalho de forma semelhante para obter várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="c1a5b-109">Se houver mais de um grupo de tarefas e você quiser obter todas as tarefas em um grupo de tarefas específico, primeiro [obtenha todas as pastas de tarefas desse grupo de tarefas](outlooktaskgroup-list-taskfolders.md)e, em seguida, obtenha as tarefas em cada uma dessas pastas de tarefas.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a5b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1a5b-110">Permissions</span></span>
<span data-ttu-id="c1a5b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a5b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1a5b-113">Permission type</span></span>      | <span data-ttu-id="c1a5b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1a5b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1a5b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1a5b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c1a5b-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c1a5b-116">Tasks.Read</span></span>    |
|<span data-ttu-id="c1a5b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1a5b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a5b-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c1a5b-118">Tasks.Read</span></span>    |
|<span data-ttu-id="c1a5b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1a5b-119">Application</span></span> | <span data-ttu-id="c1a5b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1a5b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a5b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1a5b-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1a5b-122">Optional query parameters</span></span>
<span data-ttu-id="c1a5b-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1a5b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a5b-124">Request headers</span></span>
| <span data-ttu-id="c1a5b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="c1a5b-125">Name</span></span>      |<span data-ttu-id="c1a5b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a5b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1a5b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1a5b-127">Authorization</span></span>  | <span data-ttu-id="c1a5b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1a5b-130">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c1a5b-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c1a5b-131">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c1a5b-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a5b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a5b-133">Request body</span></span>
<span data-ttu-id="c1a5b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1a5b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a5b-135">Response</span></span>

<span data-ttu-id="c1a5b-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1a5b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1a5b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1a5b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a5b-138">Request</span></span>
<span data-ttu-id="c1a5b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1a5b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a5b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1a5b-141">C#</span><span class="sxs-lookup"><span data-stu-id="c1a5b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1a5b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1a5b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1a5b-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c1a5b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1a5b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a5b-144">Response</span></span>
<span data-ttu-id="c1a5b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1a5b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
