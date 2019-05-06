---
title: Obter outlookTask
description: Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 741aa6d7363473f3e38fa797d0f389f20cfcd39b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596719"
---
# <a name="get-outlooktask"></a><span data-ttu-id="a0ffc-103">Obter outlookTask</span><span class="sxs-lookup"><span data-stu-id="a0ffc-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ffc-104">Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="a0ffc-105">Por padrão, essa operação (e as operações de POST, PATCH e tarefa [completa](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="a0ffc-106">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0ffc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0ffc-107">Permissions</span></span>

<span data-ttu-id="a0ffc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ffc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0ffc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0ffc-110">Permission type</span></span>                        | <span data-ttu-id="a0ffc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0ffc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="a0ffc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0ffc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0ffc-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a0ffc-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="a0ffc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0ffc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ffc-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a0ffc-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="a0ffc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ffc-116">Application</span></span>                            | <span data-ttu-id="a0ffc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="a0ffc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0ffc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0ffc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0ffc-119">Optional query parameters</span></span>

<span data-ttu-id="a0ffc-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0ffc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ffc-121">Request headers</span></span>

| <span data-ttu-id="a0ffc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a0ffc-122">Name</span></span>                     | <span data-ttu-id="a0ffc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ffc-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="a0ffc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0ffc-124">Authorization</span></span>            | <span data-ttu-id="a0ffc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="a0ffc-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a0ffc-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a0ffc-128">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="a0ffc-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0ffc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ffc-130">Request body</span></span>

<span data-ttu-id="a0ffc-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0ffc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ffc-132">Response</span></span>

<span data-ttu-id="a0ffc-133">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0ffc-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0ffc-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="a0ffc-135">Exemplo 1: obter uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="a0ffc-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="a0ffc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ffc-136">Request</span></span>

<span data-ttu-id="a0ffc-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a0ffc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ffc-138">Response</span></span>

<span data-ttu-id="a0ffc-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-139">Here is an example of the response.</span></span> <span data-ttu-id="a0ffc-140">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-140">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="a0ffc-141">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a0ffc-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-142">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
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
  "hasAttachments": false,
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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0ffc-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a0ffc-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0ffc-144">Basic</span><span class="sxs-lookup"><span data-stu-id="a0ffc-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0ffc-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0ffc-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_outlooktask-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="a0ffc-146">Exemplo 2: obter a tarefa do Outlook com as propriedades de data e hora no horário padrão do Pacífico</span><span class="sxs-lookup"><span data-stu-id="a0ffc-146">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="a0ffc-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ffc-147">Request</span></span>

<span data-ttu-id="a0ffc-148">Este exemplo usa o `Prefer: outlook.timezone` cabeçalho para especificar que a API deve retornar as propriedades de data e hora na resposta no horário padrão do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-148">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="a0ffc-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ffc-149">Response</span></span>

<span data-ttu-id="a0ffc-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-150">Here is an example of the response.</span></span> <span data-ttu-id="a0ffc-151">As propriedades de data e hora na resposta são retornadas no horário padrão do Pacífico especificado.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-151">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="a0ffc-152">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-152">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a0ffc-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0ffc-153">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments": false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0ffc-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a0ffc-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0ffc-155">Basic</span><span class="sxs-lookup"><span data-stu-id="a0ffc-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_outlooktask-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0ffc-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0ffc-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_outlooktask-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
