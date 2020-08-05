---
title: Excluir identityProvider
description: Excluir um identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f138dd61b8674151fd3ac2ec7ddd1f340570e994
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566802"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="106c2-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="106c2-103">Delete identityProvider</span></span>

<span data-ttu-id="106c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="106c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="106c2-105">Excluir um [identityprovider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="106c2-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="106c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="106c2-106">Permissions</span></span>

<span data-ttu-id="106c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="106c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="106c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="106c2-109">Permission type</span></span>      | <span data-ttu-id="106c2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="106c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="106c2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="106c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="106c2-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106c2-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="106c2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="106c2-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="106c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="106c2-114">Not supported.</span></span>|
|<span data-ttu-id="106c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="106c2-115">Application</span></span>|<span data-ttu-id="106c2-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106c2-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="106c2-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="106c2-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="106c2-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="106c2-118">Global administrator</span></span>
* <span data-ttu-id="106c2-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="106c2-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="106c2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="106c2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="106c2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="106c2-121">Request headers</span></span>

|<span data-ttu-id="106c2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="106c2-122">Name</span></span>|<span data-ttu-id="106c2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="106c2-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="106c2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="106c2-124">Authorization</span></span>|<span data-ttu-id="106c2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="106c2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="106c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="106c2-127">Request body</span></span>

<span data-ttu-id="106c2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="106c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="106c2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="106c2-129">Response</span></span>

<span data-ttu-id="106c2-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="106c2-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="106c2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="106c2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="106c2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="106c2-132">Request</span></span>

<span data-ttu-id="106c2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="106c2-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="106c2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="106c2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="106c2-135">C#</span><span class="sxs-lookup"><span data-stu-id="106c2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="106c2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="106c2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="106c2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="106c2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="106c2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="106c2-138">Response</span></span>

<span data-ttu-id="106c2-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="106c2-139">The following is an example of the response.</span></span>

<span data-ttu-id="106c2-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="106c2-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
