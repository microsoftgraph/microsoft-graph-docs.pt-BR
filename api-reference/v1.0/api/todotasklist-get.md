---
title: Obter todoTaskList
description: Leia as propriedades e os relacionamentos de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9b70fa36c3109b77796e212aa152358ac4cc6d20
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874266"
---
# <a name="get-todotasklist"></a><span data-ttu-id="8e100-103">Obter todoTaskList</span><span class="sxs-lookup"><span data-stu-id="8e100-103">Get todoTaskList</span></span>
<span data-ttu-id="8e100-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e100-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e100-105">Leia as propriedades e os relacionamentos de um [objeto todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="8e100-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e100-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e100-106">Permissions</span></span>
<span data-ttu-id="8e100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e100-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e100-109">Permission type</span></span>|<span data-ttu-id="8e100-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e100-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e100-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e100-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e100-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e100-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8e100-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e100-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e100-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e100-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8e100-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e100-115">Application</span></span>|<span data-ttu-id="8e100-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e100-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e100-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e100-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e100-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e100-118">Optional query parameters</span></span>
<span data-ttu-id="8e100-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e100-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e100-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e100-120">Request headers</span></span>
|<span data-ttu-id="8e100-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8e100-121">Name</span></span>|<span data-ttu-id="8e100-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e100-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8e100-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e100-123">Authorization</span></span>|<span data-ttu-id="8e100-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e100-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e100-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e100-126">Request body</span></span>
<span data-ttu-id="8e100-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e100-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e100-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e100-128">Response</span></span>

<span data-ttu-id="8e100-129">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e100-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e100-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e100-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e100-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e100-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8e100-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e100-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="8e100-133">C#</span><span class="sxs-lookup"><span data-stu-id="8e100-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e100-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e100-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e100-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e100-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e100-136">Java</span><span class="sxs-lookup"><span data-stu-id="8e100-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8e100-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e100-137">Response</span></span>
><span data-ttu-id="8e100-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8e100-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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



