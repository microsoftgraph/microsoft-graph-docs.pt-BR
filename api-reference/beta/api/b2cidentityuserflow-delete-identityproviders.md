---
title: Excluir identityProvider de um b2cIdentityUserFlow
description: Exclua um identityProvider de um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 290a2e7597f0211bf4aefbda70273efb5003aa69
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944864"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow"></a><span data-ttu-id="2973a-103">Excluir um identityProvider de um b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="2973a-103">Delete an identityProvider from a b2cIdentityUserFlow</span></span>

<span data-ttu-id="2973a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2973a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2973a-105">Exclua um provedor de identidade de um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="2973a-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="2973a-106">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="2973a-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="2973a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2973a-107">Permissions</span></span>

<span data-ttu-id="2973a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2973a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2973a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2973a-110">Permission type</span></span>      | <span data-ttu-id="2973a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2973a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2973a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2973a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2973a-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2973a-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2973a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2973a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2973a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2973a-115">Not supported.</span></span>|
|<span data-ttu-id="2973a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2973a-116">Application</span></span>| <span data-ttu-id="2973a-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2973a-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="2973a-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="2973a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2973a-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2973a-119">Global administrator</span></span>
* <span data-ttu-id="2973a-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="2973a-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2973a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2973a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2973a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2973a-122">Request headers</span></span>

|<span data-ttu-id="2973a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2973a-123">Name</span></span>|<span data-ttu-id="2973a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2973a-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2973a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2973a-125">Authorization</span></span>|<span data-ttu-id="2973a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2973a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2973a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2973a-128">Request body</span></span>

<span data-ttu-id="2973a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2973a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2973a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2973a-130">Response</span></span>

<span data-ttu-id="2973a-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2973a-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="2973a-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="2973a-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2973a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2973a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2973a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2973a-134">Request</span></span>

<span data-ttu-id="2973a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2973a-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2973a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2973a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="2973a-137">C#</span><span class="sxs-lookup"><span data-stu-id="2973a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2973a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2973a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2973a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2973a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2973a-140">Java</span><span class="sxs-lookup"><span data-stu-id="2973a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2973a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2973a-141">Response</span></span>

<span data-ttu-id="2973a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2973a-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


