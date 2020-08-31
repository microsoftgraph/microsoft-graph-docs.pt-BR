---
title: Listar tarefas
description: Obtenha todas as tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: da90726d3776e48df847533a6af5a80b47300a73
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312156"
---
# <a name="list-tasks-deprecated"></a><span data-ttu-id="46afb-103">Listar tarefas (preterido)</span><span class="sxs-lookup"><span data-stu-id="46afb-103">List tasks (deprecated)</span></span>

<span data-ttu-id="46afb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46afb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="46afb-105">Obtenha todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="46afb-105">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="46afb-106">Por padrão, essa operação (e as operações de POST, PATCH e tarefa [completa](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="46afb-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="46afb-107">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="46afb-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="46afb-108">Veja um [exemplo](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) para obter uma única tarefa.</span><span class="sxs-lookup"><span data-stu-id="46afb-108">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="46afb-109">Você pode aplicar o cabeçalho de forma semelhante para obter várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="46afb-109">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="46afb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="46afb-110">Permissions</span></span>
<span data-ttu-id="46afb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46afb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46afb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46afb-113">Permission type</span></span>      | <span data-ttu-id="46afb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46afb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46afb-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46afb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="46afb-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="46afb-116">Tasks.Read</span></span>    |
|<span data-ttu-id="46afb-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46afb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46afb-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="46afb-118">Tasks.Read</span></span>    |
|<span data-ttu-id="46afb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46afb-119">Application</span></span> | <span data-ttu-id="46afb-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46afb-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46afb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46afb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46afb-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46afb-122">Optional query parameters</span></span>
<span data-ttu-id="46afb-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46afb-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46afb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46afb-124">Request headers</span></span>
| <span data-ttu-id="46afb-125">Nome</span><span class="sxs-lookup"><span data-stu-id="46afb-125">Name</span></span>      |<span data-ttu-id="46afb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="46afb-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46afb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="46afb-127">Authorization</span></span>  | <span data-ttu-id="46afb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46afb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46afb-130">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="46afb-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="46afb-131">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="46afb-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="46afb-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="46afb-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46afb-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46afb-133">Request body</span></span>
<span data-ttu-id="46afb-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46afb-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46afb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="46afb-135">Response</span></span>

<span data-ttu-id="46afb-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46afb-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46afb-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46afb-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46afb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46afb-138">Request</span></span>
<span data-ttu-id="46afb-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46afb-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46afb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="46afb-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlookuser_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
# <a name="c"></a>[<span data-ttu-id="46afb-141">C#</span><span class="sxs-lookup"><span data-stu-id="46afb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlookuser-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46afb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46afb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlookuser-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46afb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46afb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlookuser-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="46afb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="46afb-144">Response</span></span>
<span data-ttu-id="46afb-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46afb-145">Here is an example of the response.</span></span> <span data-ttu-id="46afb-146">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="46afb-146">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="46afb-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46afb-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
