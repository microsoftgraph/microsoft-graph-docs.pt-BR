---
title: Obter todoTaskList
description: Leia as propriedades e as relações de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8150220c7e70197d425b9868c3062b094dcd5a91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953842"
---
# <a name="get-todotasklist"></a><span data-ttu-id="6dddb-103">Obter todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6dddb-103">Get todoTaskList</span></span>
<span data-ttu-id="6dddb-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="6dddb-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="6dddb-105">Leia as propriedades e as relações de um [objeto todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="6dddb-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dddb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dddb-106">Permissions</span></span>
<span data-ttu-id="6dddb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dddb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dddb-109">Permission type</span></span>|<span data-ttu-id="6dddb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dddb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dddb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dddb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dddb-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dddb-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="6dddb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dddb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dddb-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dddb-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="6dddb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dddb-115">Application</span></span>|<span data-ttu-id="6dddb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dddb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dddb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dddb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dddb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6dddb-118">Optional query parameters</span></span>
<span data-ttu-id="6dddb-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6dddb-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dddb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dddb-120">Request headers</span></span>
|<span data-ttu-id="6dddb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6dddb-121">Name</span></span>|<span data-ttu-id="6dddb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dddb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6dddb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dddb-123">Authorization</span></span>|<span data-ttu-id="6dddb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dddb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dddb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dddb-126">Request body</span></span>
<span data-ttu-id="6dddb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6dddb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dddb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dddb-128">Response</span></span>

<span data-ttu-id="6dddb-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dddb-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dddb-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6dddb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dddb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dddb-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6dddb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dddb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="6dddb-133">C#</span><span class="sxs-lookup"><span data-stu-id="6dddb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dddb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dddb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dddb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dddb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6dddb-136">Java</span><span class="sxs-lookup"><span data-stu-id="6dddb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6dddb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dddb-137">Response</span></span>
><span data-ttu-id="6dddb-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6dddb-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.todoTaskList",
    "id": "5daae1ed-e1ed-5daa-ede1-aa5dede1aa5d",
    "displayName": "Monthly tasks",
    "isOwner": "true",
    "isShared": "false",
    "wellknownListName": "defaultList"
  }
}
```



