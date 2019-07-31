---
title: Obter outlookTask
description: Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f37cc1bae0b227348c6152161768ce40c4db9dc9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983732"
---
# <a name="get-outlooktask"></a><span data-ttu-id="95c14-103">Obter outlookTask</span><span class="sxs-lookup"><span data-stu-id="95c14-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c14-104">Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="95c14-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="95c14-105">Por padrão, essa operação (e as operações de POST, PATCH e tarefa [completa](../api/outlooktask-complete.md) ) retorna as propriedades relacionadas à data no UTC.</span><span class="sxs-lookup"><span data-stu-id="95c14-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="95c14-106">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="95c14-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="95c14-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="95c14-107">Permissions</span></span>

<span data-ttu-id="95c14-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95c14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95c14-110">Permission type</span></span>                        | <span data-ttu-id="95c14-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95c14-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="95c14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95c14-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="95c14-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="95c14-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="95c14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95c14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95c14-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="95c14-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="95c14-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95c14-116">Application</span></span>                            | <span data-ttu-id="95c14-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95c14-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="95c14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95c14-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95c14-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95c14-119">Optional query parameters</span></span>

<span data-ttu-id="95c14-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95c14-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95c14-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95c14-121">Request headers</span></span>

| <span data-ttu-id="95c14-122">Nome</span><span class="sxs-lookup"><span data-stu-id="95c14-122">Name</span></span>                     | <span data-ttu-id="95c14-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c14-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="95c14-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="95c14-124">Authorization</span></span>            | <span data-ttu-id="95c14-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95c14-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="95c14-127">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="95c14-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="95c14-128">Especifica o fuso horário para as propriedades de hora na resposta, que seria no UTC se esse cabeçalho não for especificado.</span><span class="sxs-lookup"><span data-stu-id="95c14-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="95c14-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="95c14-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95c14-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95c14-130">Request body</span></span>

<span data-ttu-id="95c14-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95c14-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95c14-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c14-132">Response</span></span>

<span data-ttu-id="95c14-133">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c14-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95c14-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95c14-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="95c14-135">Exemplo 1: obter uma tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="95c14-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="95c14-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c14-136">Request</span></span>

<span data-ttu-id="95c14-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95c14-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95c14-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="95c14-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95c14-139">C#</span><span class="sxs-lookup"><span data-stu-id="95c14-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95c14-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="95c14-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95c14-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="95c14-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="95c14-142">Java</span><span class="sxs-lookup"><span data-stu-id="95c14-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="95c14-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c14-143">Response</span></span>

<span data-ttu-id="95c14-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c14-144">Here is an example of the response.</span></span> <span data-ttu-id="95c14-145">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="95c14-145">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="95c14-146">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="95c14-146">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="95c14-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95c14-147">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="95c14-148">Exemplo 2: obter a tarefa do Outlook com as propriedades de data e hora no horário padrão do Pacífico</span><span class="sxs-lookup"><span data-stu-id="95c14-148">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="95c14-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95c14-149">Request</span></span>

<span data-ttu-id="95c14-150">Este exemplo usa o `Prefer: outlook.timezone` cabeçalho para especificar que a API deve retornar as propriedades de data e hora na resposta no horário padrão do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="95c14-150">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="95c14-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="95c14-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95c14-152">C#</span><span class="sxs-lookup"><span data-stu-id="95c14-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95c14-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="95c14-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95c14-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="95c14-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="95c14-155">Java</span><span class="sxs-lookup"><span data-stu-id="95c14-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95c14-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="95c14-156">Response</span></span>

<span data-ttu-id="95c14-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95c14-157">Here is an example of the response.</span></span> <span data-ttu-id="95c14-158">As propriedades de data e hora na resposta são retornadas no horário padrão do Pacífico especificado.</span><span class="sxs-lookup"><span data-stu-id="95c14-158">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="95c14-159">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="95c14-159">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="95c14-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95c14-160">All of the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
