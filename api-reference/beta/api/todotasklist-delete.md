---
title: Excluir todoTaskList
description: Exclui um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8e4b61deb0f3eb1ad0a7029029f0b06c1b2c6338
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967249"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="984c3-103">Excluir todoTaskList</span><span class="sxs-lookup"><span data-stu-id="984c3-103">Delete todoTaskList</span></span>
<span data-ttu-id="984c3-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="984c3-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="984c3-105">Exclui um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="984c3-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="984c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="984c3-106">Permissions</span></span>
<span data-ttu-id="984c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="984c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="984c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="984c3-109">Permission type</span></span>|<span data-ttu-id="984c3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="984c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="984c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="984c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="984c3-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="984c3-112">Tasks.Read</span></span>|
|<span data-ttu-id="984c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="984c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="984c3-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="984c3-114">Tasks.Read</span></span>|
|<span data-ttu-id="984c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="984c3-115">Application</span></span>|<span data-ttu-id="984c3-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="984c3-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="984c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="984c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="984c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="984c3-118">Request headers</span></span>
|<span data-ttu-id="984c3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="984c3-119">Name</span></span>|<span data-ttu-id="984c3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="984c3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="984c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="984c3-121">Authorization</span></span>|<span data-ttu-id="984c3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="984c3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="984c3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="984c3-124">Request body</span></span>
<span data-ttu-id="984c3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="984c3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="984c3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="984c3-126">Response</span></span>

<span data-ttu-id="984c3-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="984c3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="984c3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="984c3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="984c3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="984c3-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="984c3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="984c3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="984c3-131">C#</span><span class="sxs-lookup"><span data-stu-id="984c3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="984c3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="984c3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="984c3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="984c3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="984c3-134">Java</span><span class="sxs-lookup"><span data-stu-id="984c3-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="984c3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="984c3-135">Response</span></span>
<span data-ttu-id="984c3-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="984c3-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



