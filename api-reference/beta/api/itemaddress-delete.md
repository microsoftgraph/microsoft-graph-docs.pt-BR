---
title: Excluir itemAddress
description: Exclui um objeto itemAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1469633fd4cff278914bc4aa6cb6a757fd20c36f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774713"
---
# <a name="delete-itemaddress"></a><span data-ttu-id="0f4b3-103">Excluir itemAddress</span><span class="sxs-lookup"><span data-stu-id="0f4b3-103">Delete itemAddress</span></span>
<span data-ttu-id="0f4b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f4b3-105">Exclui um [objeto itemAddress.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="0f4b3-105">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f4b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f4b3-106">Permissions</span></span>

<span data-ttu-id="0f4b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f4b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f4b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f4b3-109">Permission type</span></span>                        | <span data-ttu-id="0f4b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f4b3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0f4b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f4b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f4b3-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4b3-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0f4b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f4b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f4b3-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4b3-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0f4b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f4b3-115">Application</span></span>                            | <span data-ttu-id="0f4b3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4b3-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="0f4b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/addresses/{id}
DELETE /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f4b3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4b3-118">Request headers</span></span>
|<span data-ttu-id="0f4b3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0f4b3-119">Name</span></span>|<span data-ttu-id="0f4b3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4b3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f4b3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f4b3-121">Authorization</span></span>|<span data-ttu-id="0f4b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f4b3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f4b3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4b3-124">Request body</span></span>
<span data-ttu-id="0f4b3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f4b3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f4b3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4b3-126">Response</span></span>

<span data-ttu-id="0f4b3-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f4b3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0f4b3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f4b3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f4b3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4b3-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="0f4b3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4b3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemaddress"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="0f4b3-131">C#</span><span class="sxs-lookup"><span data-stu-id="0f4b3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f4b3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f4b3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f4b3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f4b3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f4b3-134">Java</span><span class="sxs-lookup"><span data-stu-id="0f4b3-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itemaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0f4b3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4b3-135">Response</span></span>
<span data-ttu-id="0f4b3-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f4b3-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


