---
title: List lists
description: Obtenha uma lista dos objetos todoTaskList e suas propriedades.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a90a531941df90fad37fc2d999f27429394df911
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904142"
---
# <a name="list-lists"></a><span data-ttu-id="ba714-103">List lists</span><span class="sxs-lookup"><span data-stu-id="ba714-103">List lists</span></span>
<span data-ttu-id="ba714-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba714-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba714-105">Obtenha uma lista dos objetos [todoTaskList](../resources/todotasklist.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ba714-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba714-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba714-106">Permissions</span></span>
<span data-ttu-id="ba714-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba714-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba714-109">Permission type</span></span>|<span data-ttu-id="ba714-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba714-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba714-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba714-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba714-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba714-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ba714-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba714-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba714-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba714-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ba714-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba714-115">Application</span></span>|<span data-ttu-id="ba714-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ba714-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba714-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba714-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba714-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba714-118">Optional query parameters</span></span>
<span data-ttu-id="ba714-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba714-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba714-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ba714-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba714-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba714-121">Request headers</span></span>
|<span data-ttu-id="ba714-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ba714-122">Name</span></span>|<span data-ttu-id="ba714-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba714-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba714-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba714-124">Authorization</span></span>|<span data-ttu-id="ba714-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba714-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba714-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba714-127">Request body</span></span>
<span data-ttu-id="ba714-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba714-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba714-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba714-129">Response</span></span>

<span data-ttu-id="ba714-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba714-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba714-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba714-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba714-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba714-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ba714-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba714-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="ba714-134">C#</span><span class="sxs-lookup"><span data-stu-id="ba714-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba714-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba714-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba714-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba714-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba714-137">Java</span><span class="sxs-lookup"><span data-stu-id="ba714-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ba714-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba714-138">Response</span></span>
<span data-ttu-id="ba714-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba714-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



