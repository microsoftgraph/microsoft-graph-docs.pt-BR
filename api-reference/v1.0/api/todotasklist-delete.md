---
title: Excluir todoTaskList
description: Exclui um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f8029417e841d2bebdf6224946342a7d9ea8797
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904963"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="f2c9d-103">Excluir todoTaskList</span><span class="sxs-lookup"><span data-stu-id="f2c9d-103">Delete todoTaskList</span></span>
<span data-ttu-id="f2c9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c9d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2c9d-105">Exclui um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="f2c9d-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c9d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2c9d-106">Permissions</span></span>
<span data-ttu-id="f2c9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2c9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c9d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2c9d-109">Permission type</span></span>|<span data-ttu-id="f2c9d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2c9d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2c9d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2c9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2c9d-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f2c9d-112">Tasks.Read</span></span>|
|<span data-ttu-id="f2c9d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2c9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2c9d-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f2c9d-114">Tasks.Read</span></span>|
|<span data-ttu-id="f2c9d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c9d-115">Application</span></span>|<span data-ttu-id="f2c9d-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f2c9d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2c9d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c9d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="f2c9d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c9d-118">Request headers</span></span>
|<span data-ttu-id="f2c9d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f2c9d-119">Name</span></span>|<span data-ttu-id="f2c9d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c9d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2c9d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2c9d-121">Authorization</span></span>|<span data-ttu-id="f2c9d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2c9d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c9d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c9d-124">Request body</span></span>
<span data-ttu-id="f2c9d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2c9d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2c9d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c9d-126">Response</span></span>

<span data-ttu-id="f2c9d-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2c9d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2c9d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2c9d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2c9d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c9d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f2c9d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c9d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="f2c9d-131">C#</span><span class="sxs-lookup"><span data-stu-id="f2c9d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2c9d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2c9d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2c9d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2c9d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2c9d-134">Java</span><span class="sxs-lookup"><span data-stu-id="f2c9d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2c9d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c9d-135">Response</span></span>
<span data-ttu-id="f2c9d-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c9d-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



