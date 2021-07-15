---
title: Excluir um userflowidentityproviders
description: Exclua um identityProvider de um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2f8f6f59ea2fcad737dc5fae9bc60d91ec467b31
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439802"
---
# <a name="delete-a-userflowidentityproviders"></a><span data-ttu-id="00f4f-103">Excluir um userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="00f4f-103">Delete a userflowidentityproviders</span></span>

<span data-ttu-id="00f4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f4f-105">Exclua um provedor de identidade de um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="00f4f-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="00f4f-106">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="00f4f-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="00f4f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="00f4f-107">Permissions</span></span>

<span data-ttu-id="00f4f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f4f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00f4f-110">Permission type</span></span>      | <span data-ttu-id="00f4f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00f4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00f4f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00f4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00f4f-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f4f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="00f4f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00f4f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="00f4f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00f4f-115">Not supported.</span></span>|
|<span data-ttu-id="00f4f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00f4f-116">Application</span></span>| <span data-ttu-id="00f4f-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f4f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="00f4f-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="00f4f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="00f4f-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="00f4f-119">Global administrator</span></span>
* <span data-ttu-id="00f4f-120">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="00f4f-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="00f4f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00f4f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="00f4f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00f4f-122">Request headers</span></span>

|<span data-ttu-id="00f4f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="00f4f-123">Name</span></span>|<span data-ttu-id="00f4f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="00f4f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="00f4f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="00f4f-125">Authorization</span></span>|<span data-ttu-id="00f4f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00f4f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00f4f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00f4f-128">Request body</span></span>

<span data-ttu-id="00f4f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00f4f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00f4f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="00f4f-130">Response</span></span>

<span data-ttu-id="00f4f-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="00f4f-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="00f4f-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="00f4f-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="00f4f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00f4f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="00f4f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00f4f-134">Request</span></span>

<span data-ttu-id="00f4f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="00f4f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="00f4f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="00f4f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/MSA-OIDC/$ref
```
# <a name="c"></a>[<span data-ttu-id="00f4f-137">C#</span><span class="sxs-lookup"><span data-stu-id="00f4f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00f4f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00f4f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00f4f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00f4f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00f4f-140">Java</span><span class="sxs-lookup"><span data-stu-id="00f4f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="00f4f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="00f4f-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
