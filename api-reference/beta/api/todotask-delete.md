---
title: Excluir todoTask
description: Exclui um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9f0642a6a8c41f56d1fe8c8a5497d71393c1cad1
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873910"
---
# <a name="delete-todotask"></a><span data-ttu-id="74df7-103">Excluir todoTask</span><span class="sxs-lookup"><span data-stu-id="74df7-103">Delete todoTask</span></span>
<span data-ttu-id="74df7-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="74df7-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="74df7-105">Exclui um [objeto todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="74df7-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74df7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="74df7-106">Permissions</span></span>
<span data-ttu-id="74df7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74df7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74df7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74df7-109">Permission type</span></span>|<span data-ttu-id="74df7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74df7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74df7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74df7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74df7-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74df7-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="74df7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74df7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74df7-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74df7-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="74df7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74df7-115">Application</span></span>|<span data-ttu-id="74df7-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="74df7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="74df7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74df7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="74df7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74df7-118">Request headers</span></span>
|<span data-ttu-id="74df7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="74df7-119">Name</span></span>|<span data-ttu-id="74df7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="74df7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="74df7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="74df7-121">Authorization</span></span>|<span data-ttu-id="74df7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74df7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74df7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74df7-124">Request body</span></span>
<span data-ttu-id="74df7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74df7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74df7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="74df7-126">Response</span></span>

<span data-ttu-id="74df7-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74df7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="74df7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="74df7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74df7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74df7-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="74df7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="74df7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="74df7-131">C#</span><span class="sxs-lookup"><span data-stu-id="74df7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74df7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74df7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74df7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74df7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74df7-134">Java</span><span class="sxs-lookup"><span data-stu-id="74df7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="74df7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="74df7-135">Response</span></span>
<span data-ttu-id="74df7-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74df7-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



