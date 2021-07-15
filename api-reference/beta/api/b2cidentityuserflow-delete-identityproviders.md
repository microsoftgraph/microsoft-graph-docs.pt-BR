---
title: Excluir identityProvider de um b2cIdentityUserFlow (preterido)
description: Exclua um identityProvider de um b2cIdentityUserFlow. (preterido)
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 64a72b0d286ff9e794d8ca654d498ee95f1a52de
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439809"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="7e1aa-104">Excluir um identityProvider de um b2cIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="7e1aa-104">Delete an identityProvider from a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="7e1aa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e1aa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="7e1aa-106">Exclua um provedor de identidade de um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7e1aa-106">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="7e1aa-107">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="7e1aa-107">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e1aa-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e1aa-108">Permissions</span></span>

<span data-ttu-id="7e1aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e1aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e1aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e1aa-111">Permission type</span></span>      | <span data-ttu-id="7e1aa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e1aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e1aa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e1aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e1aa-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e1aa-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7e1aa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e1aa-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7e1aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-116">Not supported.</span></span>|
|<span data-ttu-id="7e1aa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e1aa-117">Application</span></span>| <span data-ttu-id="7e1aa-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e1aa-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7e1aa-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="7e1aa-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7e1aa-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7e1aa-120">Global administrator</span></span>
* <span data-ttu-id="7e1aa-121">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="7e1aa-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7e1aa-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e1aa-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7e1aa-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e1aa-123">Request headers</span></span>

|<span data-ttu-id="7e1aa-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7e1aa-124">Name</span></span>|<span data-ttu-id="7e1aa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e1aa-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7e1aa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e1aa-126">Authorization</span></span>|<span data-ttu-id="7e1aa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e1aa-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e1aa-129">Request body</span></span>

<span data-ttu-id="7e1aa-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e1aa-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e1aa-131">Response</span></span>

<span data-ttu-id="7e1aa-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="7e1aa-133">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7e1aa-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e1aa-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e1aa-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e1aa-135">Request</span></span>

<span data-ttu-id="7e1aa-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e1aa-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e1aa-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="7e1aa-138">C#</span><span class="sxs-lookup"><span data-stu-id="7e1aa-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e1aa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e1aa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e1aa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e1aa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e1aa-141">Java</span><span class="sxs-lookup"><span data-stu-id="7e1aa-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e1aa-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e1aa-142">Response</span></span>

<span data-ttu-id="7e1aa-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e1aa-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
