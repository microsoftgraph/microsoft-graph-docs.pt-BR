---
title: Obter todoTaskList
description: Leia as propriedades e os relacionamentos de um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 89760dc319ac621a4aa34ff13da178acb60dd0e1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905124"
---
# <a name="get-todotasklist"></a><span data-ttu-id="f7e5e-103">Obter todoTaskList</span><span class="sxs-lookup"><span data-stu-id="f7e5e-103">Get todoTaskList</span></span>
<span data-ttu-id="f7e5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7e5e-105">Leia as propriedades e os relacionamentos de um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="f7e5e-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7e5e-106">Permissions</span></span>
<span data-ttu-id="f7e5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7e5e-109">Permission type</span></span>|<span data-ttu-id="f7e5e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7e5e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7e5e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7e5e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7e5e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7e5e-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f7e5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7e5e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7e5e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7e5e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f7e5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7e5e-115">Application</span></span>|<span data-ttu-id="f7e5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7e5e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7e5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7e5e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7e5e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7e5e-118">Optional query parameters</span></span>
<span data-ttu-id="f7e5e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7e5e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7e5e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7e5e-120">Request headers</span></span>
|<span data-ttu-id="f7e5e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f7e5e-121">Name</span></span>|<span data-ttu-id="f7e5e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7e5e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7e5e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7e5e-123">Authorization</span></span>|<span data-ttu-id="f7e5e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7e5e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e5e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7e5e-126">Request body</span></span>
<span data-ttu-id="f7e5e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7e5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e5e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7e5e-128">Response</span></span>

<span data-ttu-id="f7e5e-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7e5e-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7e5e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7e5e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7e5e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7e5e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f7e5e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7e5e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="f7e5e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f7e5e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7e5e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7e5e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7e5e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7e5e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7e5e-136">Java</span><span class="sxs-lookup"><span data-stu-id="f7e5e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f7e5e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7e5e-137">Response</span></span>
><span data-ttu-id="f7e5e-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7e5e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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



