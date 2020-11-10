---
title: Excluir identityProvider
description: Excluir um identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53950e1c839b70e84c924d39c0943c8d2ffe34a1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953438"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="c83b8-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="c83b8-103">Delete identityProvider</span></span>

<span data-ttu-id="c83b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c83b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c83b8-105">Excluir um [identityprovider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="c83b8-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c83b8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c83b8-106">Permissions</span></span>

<span data-ttu-id="c83b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c83b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c83b8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c83b8-109">Permission type</span></span>      | <span data-ttu-id="c83b8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c83b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c83b8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c83b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c83b8-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83b8-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c83b8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c83b8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c83b8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c83b8-114">Not supported.</span></span>|
|<span data-ttu-id="c83b8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c83b8-115">Application</span></span>|<span data-ttu-id="c83b8-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83b8-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="c83b8-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c83b8-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="c83b8-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c83b8-118">Global administrator</span></span>
* <span data-ttu-id="c83b8-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c83b8-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c83b8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c83b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c83b8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c83b8-121">Request headers</span></span>

|<span data-ttu-id="c83b8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c83b8-122">Name</span></span>|<span data-ttu-id="c83b8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c83b8-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c83b8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c83b8-124">Authorization</span></span>|<span data-ttu-id="c83b8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c83b8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c83b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c83b8-127">Request body</span></span>

<span data-ttu-id="c83b8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c83b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c83b8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c83b8-129">Response</span></span>

<span data-ttu-id="c83b8-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c83b8-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c83b8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c83b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c83b8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c83b8-132">Request</span></span>

<span data-ttu-id="c83b8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c83b8-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c83b8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c83b8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="c83b8-135">C#</span><span class="sxs-lookup"><span data-stu-id="c83b8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c83b8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c83b8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c83b8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c83b8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c83b8-138">Java</span><span class="sxs-lookup"><span data-stu-id="c83b8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c83b8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c83b8-139">Response</span></span>

<span data-ttu-id="c83b8-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c83b8-140">The following is an example of the response.</span></span>

<span data-ttu-id="c83b8-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c83b8-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


