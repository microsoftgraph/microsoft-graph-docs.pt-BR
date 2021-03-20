---
title: Obter todoTask
description: Leia as propriedades e as relações de um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d188675fc35ac647ef11c2016104a52bfca87cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942113"
---
# <a name="get-todotask"></a><span data-ttu-id="b6cb4-103">Obter todoTask</span><span class="sxs-lookup"><span data-stu-id="b6cb4-103">Get todoTask</span></span>
<span data-ttu-id="b6cb4-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="b6cb4-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="b6cb4-105">Leia as propriedades e as relações de um [objeto todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="b6cb4-105">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6cb4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6cb4-106">Permissions</span></span>
<span data-ttu-id="b6cb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6cb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6cb4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6cb4-109">Permission type</span></span>|<span data-ttu-id="b6cb4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6cb4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6cb4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6cb4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6cb4-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6cb4-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b6cb4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6cb4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6cb4-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6cb4-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b6cb4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6cb4-115">Application</span></span>|<span data-ttu-id="b6cb4-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b6cb4-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6cb4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cb4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6cb4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6cb4-118">Optional query parameters</span></span>
<span data-ttu-id="b6cb4-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6cb4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b6cb4-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6cb4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6cb4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cb4-121">Request headers</span></span>
|<span data-ttu-id="b6cb4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b6cb4-122">Name</span></span>|<span data-ttu-id="b6cb4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6cb4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6cb4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6cb4-124">Authorization</span></span>|<span data-ttu-id="b6cb4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6cb4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6cb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cb4-127">Request body</span></span>
<span data-ttu-id="b6cb4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6cb4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6cb4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cb4-129">Response</span></span>

<span data-ttu-id="b6cb4-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6cb4-130">If successful, this method returns a `200 OK` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6cb4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6cb4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6cb4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cb4-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b6cb4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cb4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "get_todotask_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="b6cb4-134">C#</span><span class="sxs-lookup"><span data-stu-id="b6cb4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6cb4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6cb4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6cb4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6cb4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6cb4-137">Java</span><span class="sxs-lookup"><span data-stu-id="b6cb4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b6cb4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cb4-138">Response</span></span>
<span data-ttu-id="b6cb4-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6cb4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



