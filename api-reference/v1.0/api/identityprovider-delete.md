---
title: Excluir identityProvider
description: Excluir um identityProvider existente.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: deb255656748a43af87a219e3a094b7cc897273d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516777"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="94a46-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="94a46-103">Delete identityProvider</span></span>

<span data-ttu-id="94a46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94a46-105">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="94a46-105">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94a46-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a46-106">Permissions</span></span>

<span data-ttu-id="94a46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a46-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a46-109">Permission type</span></span>      | <span data-ttu-id="94a46-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a46-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94a46-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a46-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="94a46-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a46-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="94a46-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a46-114">Not supported.</span></span>|
|<span data-ttu-id="94a46-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a46-115">Application</span></span>|<span data-ttu-id="94a46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a46-116">Not supported.</span></span>|

<span data-ttu-id="94a46-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="94a46-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="94a46-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a46-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94a46-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a46-119">Request headers</span></span>

|<span data-ttu-id="94a46-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94a46-120">Name</span></span>|<span data-ttu-id="94a46-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a46-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="94a46-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a46-122">Authorization</span></span>|<span data-ttu-id="94a46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a46-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a46-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a46-125">Request body</span></span>

<span data-ttu-id="94a46-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94a46-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a46-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a46-127">Response</span></span>

<span data-ttu-id="94a46-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94a46-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="94a46-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a46-129">Example</span></span>

<span data-ttu-id="94a46-130">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="94a46-130">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="94a46-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a46-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="94a46-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="94a46-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="94a46-133">C#</span><span class="sxs-lookup"><span data-stu-id="94a46-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94a46-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94a46-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94a46-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94a46-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94a46-136">Java</span><span class="sxs-lookup"><span data-stu-id="94a46-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94a46-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a46-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
