---
title: Excluir identityprovider de b2xIdentityUserFlow
description: Excluir um identityprovider de um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25db32f3f84a705f167fe1216b2a68554d9e3e9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961113"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="807e2-103">Excluir identityprovider de b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="807e2-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="807e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="807e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="807e2-105">Excluir um provedor de identidade de um objeto [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="807e2-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="807e2-106">Para os fluxos de usuário de inscrição de autoatendimento, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="807e2-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="807e2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="807e2-107">Permissions</span></span>

<span data-ttu-id="807e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="807e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="807e2-110">Permission type</span></span>      | <span data-ttu-id="807e2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="807e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="807e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="807e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="807e2-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="807e2-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="807e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="807e2-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="807e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="807e2-115">Not supported.</span></span>|
|<span data-ttu-id="807e2-116">Application</span><span class="sxs-lookup"><span data-stu-id="807e2-116">Application</span></span>| <span data-ttu-id="807e2-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="807e2-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="807e2-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="807e2-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="807e2-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="807e2-119">Global administrator</span></span>
* <span data-ttu-id="807e2-120">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="807e2-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="807e2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="807e2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="807e2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="807e2-122">Request headers</span></span>

|<span data-ttu-id="807e2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="807e2-123">Name</span></span>|<span data-ttu-id="807e2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="807e2-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="807e2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="807e2-125">Authorization</span></span>|<span data-ttu-id="807e2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="807e2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="807e2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="807e2-128">Request body</span></span>

<span data-ttu-id="807e2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="807e2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="807e2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="807e2-130">Response</span></span>

<span data-ttu-id="807e2-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="807e2-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="807e2-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="807e2-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="807e2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="807e2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="807e2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="807e2-134">Request</span></span>

<span data-ttu-id="807e2-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="807e2-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="807e2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="807e2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="807e2-137">C#</span><span class="sxs-lookup"><span data-stu-id="807e2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="807e2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="807e2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="807e2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="807e2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="807e2-140">Java</span><span class="sxs-lookup"><span data-stu-id="807e2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="807e2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="807e2-141">Response</span></span>

<span data-ttu-id="807e2-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="807e2-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


