---
title: List lists
description: Obter uma lista dos objetos todoTaskList e suas propriedades.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 67e6bc042770381112f8c44f8e4e51111de8035f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873798"
---
# <a name="list-lists"></a><span data-ttu-id="c4a29-103">List lists</span><span class="sxs-lookup"><span data-stu-id="c4a29-103">List lists</span></span>
<span data-ttu-id="c4a29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4a29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4a29-105">Obter uma lista dos [objetos todoTaskList](../resources/todotasklist.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c4a29-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4a29-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4a29-106">Permissions</span></span>
<span data-ttu-id="c4a29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a29-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4a29-109">Permission type</span></span>|<span data-ttu-id="c4a29-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4a29-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a29-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4a29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a29-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4a29-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="c4a29-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4a29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a29-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4a29-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="c4a29-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4a29-115">Application</span></span>|<span data-ttu-id="c4a29-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4a29-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4a29-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a29-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4a29-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4a29-118">Optional query parameters</span></span>
<span data-ttu-id="c4a29-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a29-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c4a29-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c4a29-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4a29-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a29-121">Request headers</span></span>
|<span data-ttu-id="c4a29-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c4a29-122">Name</span></span>|<span data-ttu-id="c4a29-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4a29-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4a29-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4a29-124">Authorization</span></span>|<span data-ttu-id="c4a29-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4a29-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a29-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a29-127">Request body</span></span>
<span data-ttu-id="c4a29-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4a29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a29-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a29-129">Response</span></span>

<span data-ttu-id="c4a29-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a29-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4a29-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4a29-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4a29-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a29-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4a29-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a29-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="c4a29-134">C#</span><span class="sxs-lookup"><span data-stu-id="c4a29-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4a29-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4a29-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4a29-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4a29-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4a29-137">Java</span><span class="sxs-lookup"><span data-stu-id="c4a29-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4a29-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a29-138">Response</span></span>
<span data-ttu-id="c4a29-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4a29-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



