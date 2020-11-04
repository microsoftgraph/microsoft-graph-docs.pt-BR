---
title: Excluir linkedResource
description: Exclui um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c6ca34116903301200b7cf3d04de9f6c6069087
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903443"
---
# <a name="delete-linkedresource"></a><span data-ttu-id="da7e0-103">Excluir linkedResource</span><span class="sxs-lookup"><span data-stu-id="da7e0-103">Delete linkedResource</span></span>
<span data-ttu-id="da7e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da7e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da7e0-105">Exclui um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="da7e0-105">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da7e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da7e0-106">Permissions</span></span>
<span data-ttu-id="da7e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da7e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da7e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da7e0-109">Permission type</span></span>|<span data-ttu-id="da7e0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da7e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7e0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da7e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da7e0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da7e0-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="da7e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da7e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7e0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da7e0-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="da7e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da7e0-115">Application</span></span>|<span data-ttu-id="da7e0-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da7e0-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da7e0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="da7e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da7e0-118">Request headers</span></span>
|<span data-ttu-id="da7e0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="da7e0-119">Name</span></span>|<span data-ttu-id="da7e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da7e0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da7e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da7e0-121">Authorization</span></span>|<span data-ttu-id="da7e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da7e0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7e0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da7e0-124">Request body</span></span>
<span data-ttu-id="da7e0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da7e0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da7e0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="da7e0-126">Response</span></span>

<span data-ttu-id="da7e0-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da7e0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="da7e0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da7e0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da7e0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da7e0-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="da7e0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="da7e0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "delete_linkedresource"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="da7e0-131">C#</span><span class="sxs-lookup"><span data-stu-id="da7e0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da7e0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da7e0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da7e0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da7e0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da7e0-134">Java</span><span class="sxs-lookup"><span data-stu-id="da7e0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="da7e0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="da7e0-135">Response</span></span>
<span data-ttu-id="da7e0-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da7e0-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



