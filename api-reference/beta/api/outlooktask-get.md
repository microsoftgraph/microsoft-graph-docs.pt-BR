---
title: Obter outlookTask
description: Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8db32df8b0e92451c98e4d6bde6a2c503bb17c67
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055488"
---
# <a name="get-outlooktask-deprecated"></a><span data-ttu-id="ca8ca-103">Obter outlookTask (preterido)</span><span class="sxs-lookup"><span data-stu-id="ca8ca-103">Get outlookTask (deprecated)</span></span>

<span data-ttu-id="ca8ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca8ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="ca8ca-105">Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-105">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="ca8ca-106">Por padrão, essa operação (e as [](../api/outlooktask-complete.md) operações POST, PATCH e tarefa completa) retorna propriedades relacionadas à data em UTC.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="ca8ca-107">Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca8ca-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca8ca-108">Permissions</span></span>

<span data-ttu-id="ca8ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca8ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca8ca-111">Permission type</span></span>                        | <span data-ttu-id="ca8ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca8ca-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="ca8ca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca8ca-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca8ca-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ca8ca-114">Tasks.Read</span></span>                          |
| <span data-ttu-id="ca8ca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca8ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca8ca-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="ca8ca-116">Tasks.Read</span></span>                          |
| <span data-ttu-id="ca8ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca8ca-117">Application</span></span>                            | <span data-ttu-id="ca8ca-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-118">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="ca8ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8ca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca8ca-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca8ca-120">Optional query parameters</span></span>

<span data-ttu-id="ca8ca-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca8ca-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ca-122">Request headers</span></span>

| <span data-ttu-id="ca8ca-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ca8ca-123">Name</span></span>                     | <span data-ttu-id="ca8ca-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca8ca-124">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="ca8ca-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca8ca-125">Authorization</span></span>            | <span data-ttu-id="ca8ca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="ca8ca-128">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ca8ca-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ca8ca-129">Especifica o fuso horário para propriedades de tempo na resposta, que estaria em UTC se esse header não for especificado.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="ca8ca-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca8ca-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ca-131">Request body</span></span>

<span data-ttu-id="ca8ca-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca8ca-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8ca-133">Response</span></span>

<span data-ttu-id="ca8ca-134">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto outlookTask](../resources/outlooktask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-134">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca8ca-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca8ca-135">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="ca8ca-136">Exemplo 1: Obter uma tarefa Outlook tarefa</span><span class="sxs-lookup"><span data-stu-id="ca8ca-136">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="ca8ca-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ca-137">Request</span></span>

<span data-ttu-id="ca8ca-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca8ca-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8ca-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```
# <a name="c"></a>[<span data-ttu-id="ca8ca-140">C#</span><span class="sxs-lookup"><span data-stu-id="ca8ca-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca8ca-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca8ca-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca8ca-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca8ca-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca8ca-143">Java</span><span class="sxs-lookup"><span data-stu-id="ca8ca-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="ca8ca-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8ca-144">Response</span></span>

<span data-ttu-id="ca8ca-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-145">Here is an example of the response.</span></span> <span data-ttu-id="ca8ca-146">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-146">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="ca8ca-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="ca8ca-148">Exemplo 2: Obter Outlook com propriedades de data e hora no Horário Padrão do Pacífico</span><span class="sxs-lookup"><span data-stu-id="ca8ca-148">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="ca8ca-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ca-149">Request</span></span>

<span data-ttu-id="ca8ca-150">Este exemplo usa o header para especificar que a API deve retornar propriedades de `Prefer: outlook.timezone` data/hora na resposta no Horário Padrão do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-150">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca8ca-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8ca-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="ca8ca-152">C#</span><span class="sxs-lookup"><span data-stu-id="ca8ca-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca8ca-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca8ca-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca8ca-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca8ca-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca8ca-155">Java</span><span class="sxs-lookup"><span data-stu-id="ca8ca-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktask-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca8ca-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8ca-156">Response</span></span>

<span data-ttu-id="ca8ca-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-157">Here is an example of the response.</span></span> <span data-ttu-id="ca8ca-158">As propriedades de data e hora na resposta são retornadas no Horário Padrão do Pacífico especificado.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-158">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="ca8ca-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ca-159">**Note:** The response object shown here might be shortened for readability.</span></span>

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
