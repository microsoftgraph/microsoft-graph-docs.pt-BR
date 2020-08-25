---
title: List lists
description: Obtenha uma lista dos objetos todoTaskList e suas propriedades.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 97ce611af4441027146d2ccd5d951beacd9d20d6
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873269"
---
# <a name="list-lists"></a><span data-ttu-id="d985c-103">List lists</span><span class="sxs-lookup"><span data-stu-id="d985c-103">List lists</span></span>
<span data-ttu-id="d985c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d985c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d985c-105">Obtenha uma lista dos objetos [todoTaskList](../resources/todotasklist.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d985c-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d985c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d985c-106">Permissions</span></span>
<span data-ttu-id="d985c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d985c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d985c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d985c-109">Permission type</span></span>|<span data-ttu-id="d985c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d985c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d985c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d985c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d985c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d985c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d985c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d985c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d985c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d985c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d985c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d985c-115">Application</span></span>|<span data-ttu-id="d985c-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d985c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d985c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d985c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d985c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d985c-118">Optional query parameters</span></span>
<span data-ttu-id="d985c-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d985c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d985c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d985c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d985c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d985c-121">Request headers</span></span>
|<span data-ttu-id="d985c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d985c-122">Name</span></span>|<span data-ttu-id="d985c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d985c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d985c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d985c-124">Authorization</span></span>|<span data-ttu-id="d985c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d985c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d985c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d985c-127">Request body</span></span>
<span data-ttu-id="d985c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d985c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d985c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d985c-129">Response</span></span>

<span data-ttu-id="d985c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [todoTaskList](../resources/todotasklist.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d985c-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d985c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d985c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d985c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d985c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d985c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d985c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="d985c-134">C#</span><span class="sxs-lookup"><span data-stu-id="d985c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d985c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d985c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d985c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d985c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d985c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d985c-137">Response</span></span>
<span data-ttu-id="d985c-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d985c-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

