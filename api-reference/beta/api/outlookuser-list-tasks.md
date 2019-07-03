---
title: Listar tarefas
description: Obter todas as tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5d08e9e8ade8a3537d27ec33a61006456668ddae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447135"
---
# <a name="list-tasks"></a><span data-ttu-id="496ad-103">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="496ad-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="496ad-104">Obter todas as tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="496ad-104">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="496ad-105">Por padrão, essa operação (e as operações de POST, PATCH e tarefa [completa](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="496ad-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="496ad-106">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="496ad-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="496ad-107">Veja um [exemplo](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) para obter uma única tarefa.</span><span class="sxs-lookup"><span data-stu-id="496ad-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="496ad-108">Você pode aplicar o cabeçalho de forma semelhante para obter várias tarefas.</span><span class="sxs-lookup"><span data-stu-id="496ad-108">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="496ad-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="496ad-109">Permissions</span></span>
<span data-ttu-id="496ad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="496ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="496ad-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="496ad-112">Permission type</span></span>      | <span data-ttu-id="496ad-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="496ad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="496ad-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="496ad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="496ad-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="496ad-115">Tasks.Read</span></span>    |
|<span data-ttu-id="496ad-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="496ad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="496ad-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="496ad-117">Tasks.Read</span></span>    |
|<span data-ttu-id="496ad-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="496ad-118">Application</span></span> | <span data-ttu-id="496ad-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="496ad-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="496ad-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="496ad-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="496ad-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="496ad-121">Optional query parameters</span></span>
<span data-ttu-id="496ad-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="496ad-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="496ad-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="496ad-123">Request headers</span></span>
| <span data-ttu-id="496ad-124">Nome</span><span class="sxs-lookup"><span data-stu-id="496ad-124">Name</span></span>      |<span data-ttu-id="496ad-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="496ad-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="496ad-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="496ad-126">Authorization</span></span>  | <span data-ttu-id="496ad-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="496ad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="496ad-129">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="496ad-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="496ad-130">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="496ad-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="496ad-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="496ad-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="496ad-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="496ad-132">Request body</span></span>
<span data-ttu-id="496ad-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="496ad-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="496ad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="496ad-134">Response</span></span>

<span data-ttu-id="496ad-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="496ad-135">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="496ad-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="496ad-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="496ad-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="496ad-137">Request</span></span>
<span data-ttu-id="496ad-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="496ad-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="496ad-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="496ad-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="496ad-140">C#</span><span class="sxs-lookup"><span data-stu-id="496ad-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="496ad-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="496ad-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="496ad-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="496ad-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="496ad-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="496ad-143">Response</span></span>
<span data-ttu-id="496ad-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="496ad-144">Here is an example of the response.</span></span> <span data-ttu-id="496ad-145">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="496ad-145">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="496ad-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="496ad-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
