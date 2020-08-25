---
title: Obter todoTask
description: Leia as propriedades e os relacionamentos de um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6f009dd3f23f7bb65d490fe1782fbb3dbfc4dd62
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873262"
---
# <a name="get-todotask"></a><span data-ttu-id="3deb3-103">Obter todoTask</span><span class="sxs-lookup"><span data-stu-id="3deb3-103">Get todoTask</span></span>
<span data-ttu-id="3deb3-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="3deb3-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="3deb3-105">Leia as propriedades e os relacionamentos de um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="3deb3-105">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3deb3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3deb3-106">Permissions</span></span>
<span data-ttu-id="3deb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3deb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3deb3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3deb3-109">Permission type</span></span>|<span data-ttu-id="3deb3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3deb3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3deb3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3deb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3deb3-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3deb3-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="3deb3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3deb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3deb3-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3deb3-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="3deb3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3deb3-115">Application</span></span>|<span data-ttu-id="3deb3-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3deb3-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="3deb3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3deb3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3deb3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3deb3-118">Optional query parameters</span></span>
<span data-ttu-id="3deb3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3deb3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3deb3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3deb3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3deb3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3deb3-121">Request headers</span></span>
|<span data-ttu-id="3deb3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3deb3-122">Name</span></span>|<span data-ttu-id="3deb3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3deb3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3deb3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3deb3-124">Authorization</span></span>|<span data-ttu-id="3deb3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3deb3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3deb3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3deb3-127">Request body</span></span>
<span data-ttu-id="3deb3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3deb3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3deb3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3deb3-129">Response</span></span>

<span data-ttu-id="3deb3-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTask](../resources/todotask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3deb3-130">If successful, this method returns a `200 OK` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3deb3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3deb3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3deb3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3deb3-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3deb3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3deb3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="3deb3-134">C#</span><span class="sxs-lookup"><span data-stu-id="3deb3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3deb3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3deb3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3deb3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3deb3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3deb3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3deb3-137">Response</span></span>
<span data-ttu-id="3deb3-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3deb3-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

