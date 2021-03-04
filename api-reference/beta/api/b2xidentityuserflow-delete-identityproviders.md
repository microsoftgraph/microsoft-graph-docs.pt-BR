---
title: Excluir identityProvider de b2xIdentityUserFlow
description: Exclua um identityProvider de um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4359ded92c7bfa54a07f487554be83e17ee3c064
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438171"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="2c002-103">Excluir identityProvider de b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="2c002-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="2c002-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c002-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c002-105">Exclua um provedor de identidade de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="2c002-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="2c002-106">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="2c002-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c002-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c002-107">Permissions</span></span>

<span data-ttu-id="2c002-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c002-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c002-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c002-110">Permission type</span></span>      | <span data-ttu-id="2c002-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c002-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c002-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c002-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c002-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c002-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2c002-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c002-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2c002-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c002-115">Not supported.</span></span>|
|<span data-ttu-id="2c002-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c002-116">Application</span></span>| <span data-ttu-id="2c002-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c002-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="2c002-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="2c002-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2c002-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2c002-119">Global administrator</span></span>
* <span data-ttu-id="2c002-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="2c002-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2c002-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c002-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2c002-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c002-122">Request headers</span></span>

|<span data-ttu-id="2c002-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2c002-123">Name</span></span>|<span data-ttu-id="2c002-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c002-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2c002-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c002-125">Authorization</span></span>|<span data-ttu-id="2c002-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c002-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c002-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c002-128">Request body</span></span>

<span data-ttu-id="2c002-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c002-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c002-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c002-130">Response</span></span>

<span data-ttu-id="2c002-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c002-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="2c002-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="2c002-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2c002-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c002-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c002-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c002-134">Request</span></span>

<span data-ttu-id="2c002-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c002-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c002-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c002-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="2c002-137">C#</span><span class="sxs-lookup"><span data-stu-id="2c002-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c002-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c002-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c002-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c002-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c002-140">Java</span><span class="sxs-lookup"><span data-stu-id="2c002-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c002-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c002-141">Response</span></span>

<span data-ttu-id="2c002-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2c002-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


