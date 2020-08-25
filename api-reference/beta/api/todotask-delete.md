---
title: Excluir todoTask
description: Exclui um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5cb89bc7e21ca777f36ca846e186f741b7b5667
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873340"
---
# <a name="delete-todotask"></a><span data-ttu-id="435a1-103">Excluir todoTask</span><span class="sxs-lookup"><span data-stu-id="435a1-103">Delete todoTask</span></span>
<span data-ttu-id="435a1-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="435a1-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="435a1-105">Exclui um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="435a1-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="435a1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="435a1-106">Permissions</span></span>
<span data-ttu-id="435a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="435a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="435a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="435a1-109">Permission type</span></span>|<span data-ttu-id="435a1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="435a1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="435a1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="435a1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="435a1-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="435a1-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="435a1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="435a1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="435a1-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="435a1-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="435a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="435a1-115">Application</span></span>|<span data-ttu-id="435a1-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="435a1-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="435a1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="435a1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="435a1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="435a1-118">Request headers</span></span>
|<span data-ttu-id="435a1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="435a1-119">Name</span></span>|<span data-ttu-id="435a1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="435a1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="435a1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="435a1-121">Authorization</span></span>|<span data-ttu-id="435a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="435a1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="435a1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="435a1-124">Request body</span></span>
<span data-ttu-id="435a1-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="435a1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="435a1-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="435a1-126">Response</span></span>

<span data-ttu-id="435a1-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="435a1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="435a1-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="435a1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="435a1-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="435a1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="435a1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="435a1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="435a1-131">C#</span><span class="sxs-lookup"><span data-stu-id="435a1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="435a1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="435a1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="435a1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="435a1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="435a1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="435a1-134">Response</span></span>
<span data-ttu-id="435a1-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="435a1-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

