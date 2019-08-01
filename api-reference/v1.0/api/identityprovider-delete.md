---
title: Excluir identityProvider
description: Excluir um identityProvider existente.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1917a0d799e170636afb521ffecf4c024e431c9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002710"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="0b61e-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="0b61e-103">Delete identityProvider</span></span>

<span data-ttu-id="0b61e-104">Excluir o [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="0b61e-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b61e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b61e-105">Permissions</span></span>

<span data-ttu-id="0b61e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b61e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b61e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b61e-108">Permission type</span></span>      | <span data-ttu-id="0b61e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b61e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b61e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b61e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0b61e-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b61e-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="0b61e-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b61e-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0b61e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b61e-113">Not supported.</span></span>|
|<span data-ttu-id="0b61e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b61e-114">Application</span></span>|<span data-ttu-id="0b61e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b61e-115">Not supported.</span></span>|

<span data-ttu-id="0b61e-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="0b61e-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b61e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b61e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b61e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b61e-118">Request headers</span></span>

|<span data-ttu-id="0b61e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0b61e-119">Name</span></span>|<span data-ttu-id="0b61e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b61e-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0b61e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b61e-121">Authorization</span></span>|<span data-ttu-id="0b61e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b61e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b61e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b61e-124">Request body</span></span>

<span data-ttu-id="0b61e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b61e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b61e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b61e-126">Response</span></span>

<span data-ttu-id="0b61e-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b61e-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b61e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b61e-128">Example</span></span>

<span data-ttu-id="0b61e-129">O exemplo a seguir exclui um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="0b61e-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="0b61e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b61e-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b61e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b61e-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b61e-132">C#</span><span class="sxs-lookup"><span data-stu-id="0b61e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b61e-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b61e-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b61e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b61e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b61e-135">Java</span><span class="sxs-lookup"><span data-stu-id="0b61e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0b61e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b61e-136">Response</span></span>

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
