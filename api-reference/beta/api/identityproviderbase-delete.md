---
title: Excluir identityProvider
description: Exclua um identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: d78aff8a604f42b7efbc1f87269a87acbb29656c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508797"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="b2d3b-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="b2d3b-103">Delete identityProvider</span></span>
<span data-ttu-id="b2d3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2d3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d3b-105">[Exclua um objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-105">Delete a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="b2d3b-106">No Azure AD B2C, exclua [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um objeto appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="b2d3b-106">In Azure AD B2C, delete a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2d3b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b2d3b-107">Permissions</span></span>

<span data-ttu-id="b2d3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2d3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2d3b-110">Permission type</span></span>      | <span data-ttu-id="b2d3b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2d3b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2d3b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2d3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2d3b-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d3b-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b2d3b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2d3b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b2d3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-115">Not supported.</span></span>|
|<span data-ttu-id="b2d3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2d3b-116">Application</span></span>|<span data-ttu-id="b2d3b-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d3b-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b2d3b-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="b2d3b-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b2d3b-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="b2d3b-119">Global Administrator</span></span>
* <span data-ttu-id="b2d3b-120">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="b2d3b-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b2d3b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d3b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b2d3b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d3b-122">Request headers</span></span>

|<span data-ttu-id="b2d3b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b2d3b-123">Name</span></span>|<span data-ttu-id="b2d3b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d3b-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b2d3b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2d3b-125">Authorization</span></span>|<span data-ttu-id="b2d3b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2d3b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d3b-128">Request body</span></span>

<span data-ttu-id="b2d3b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2d3b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d3b-130">Response</span></span>

<span data-ttu-id="b2d3b-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b2d3b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2d3b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2d3b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d3b-133">Request</span></span>

<span data-ttu-id="b2d3b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-134">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="b2d3b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d3b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="b2d3b-136">C#</span><span class="sxs-lookup"><span data-stu-id="b2d3b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2d3b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2d3b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2d3b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2d3b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2d3b-139">Java</span><span class="sxs-lookup"><span data-stu-id="b2d3b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2d3b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d3b-140">Response</span></span>

<span data-ttu-id="b2d3b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-141">The following is an example of the response.</span></span>

<span data-ttu-id="b2d3b-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2d3b-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
