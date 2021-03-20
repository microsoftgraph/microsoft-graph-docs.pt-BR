---
title: List lists
description: Obter uma lista dos objetos todoTaskList e suas propriedades.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4735dff24dbccb8fbb7106a819b0b36bb132d01
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953818"
---
# <a name="list-lists"></a><span data-ttu-id="20bdb-103">List lists</span><span class="sxs-lookup"><span data-stu-id="20bdb-103">List lists</span></span>
<span data-ttu-id="20bdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20bdb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20bdb-105">Obter uma lista dos [objetos todoTaskList](../resources/todotasklist.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="20bdb-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="20bdb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20bdb-106">Permissions</span></span>
<span data-ttu-id="20bdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20bdb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20bdb-109">Permission type</span></span>|<span data-ttu-id="20bdb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20bdb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20bdb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20bdb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20bdb-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20bdb-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="20bdb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20bdb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20bdb-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20bdb-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="20bdb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20bdb-115">Application</span></span>|<span data-ttu-id="20bdb-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="20bdb-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="20bdb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20bdb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20bdb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20bdb-118">Optional query parameters</span></span>
<span data-ttu-id="20bdb-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20bdb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="20bdb-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="20bdb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20bdb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20bdb-121">Request headers</span></span>
|<span data-ttu-id="20bdb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="20bdb-122">Name</span></span>|<span data-ttu-id="20bdb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="20bdb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20bdb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="20bdb-124">Authorization</span></span>|<span data-ttu-id="20bdb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20bdb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20bdb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20bdb-127">Request body</span></span>
<span data-ttu-id="20bdb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20bdb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20bdb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="20bdb-129">Response</span></span>

<span data-ttu-id="20bdb-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20bdb-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20bdb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20bdb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20bdb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20bdb-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20bdb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="20bdb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="20bdb-134">C#</span><span class="sxs-lookup"><span data-stu-id="20bdb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20bdb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20bdb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20bdb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20bdb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20bdb-137">Java</span><span class="sxs-lookup"><span data-stu-id="20bdb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="20bdb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="20bdb-138">Response</span></span>
<span data-ttu-id="20bdb-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="20bdb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAAABrJAAA=",
      "displayName": "Tasks",
      "isOwner": true,
      "isShared": false,
      "wellknownListName": "defaultList"
    },
        {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAEFTTrJAAA=",
      "displayName": "Monthly Tasks",
      "isOwner":true,
      "isShared": false,
      "wellknownListName": "none"
    }
  ]
}
```



