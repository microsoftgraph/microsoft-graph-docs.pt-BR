---
title: Excluir um userFlowIdentityProvider
description: Exclua um identityProvider de um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 85fff2d0fab5d9d098aa7cae780c99faece3916f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439641"
---
# <a name="delete-a-userflowidentityprovider"></a><span data-ttu-id="e01cf-103">Excluir um userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="e01cf-103">Delete a userFlowIdentityProvider</span></span>

<span data-ttu-id="e01cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e01cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e01cf-105">Exclua um provedor de identidade de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e01cf-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="e01cf-106">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="e01cf-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e01cf-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e01cf-107">Permissions</span></span>

<span data-ttu-id="e01cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e01cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e01cf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e01cf-110">Permission type</span></span>      | <span data-ttu-id="e01cf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e01cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e01cf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e01cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e01cf-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e01cf-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e01cf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e01cf-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e01cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e01cf-115">Not supported.</span></span>|
|<span data-ttu-id="e01cf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e01cf-116">Application</span></span>| <span data-ttu-id="e01cf-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e01cf-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e01cf-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e01cf-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e01cf-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e01cf-119">Global administrator</span></span>
* <span data-ttu-id="e01cf-120">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="e01cf-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e01cf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e01cf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e01cf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e01cf-122">Request headers</span></span>

|<span data-ttu-id="e01cf-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e01cf-123">Name</span></span>|<span data-ttu-id="e01cf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01cf-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e01cf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e01cf-125">Authorization</span></span>|<span data-ttu-id="e01cf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e01cf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e01cf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e01cf-128">Request body</span></span>

<span data-ttu-id="e01cf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e01cf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e01cf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01cf-130">Response</span></span>

<span data-ttu-id="e01cf-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e01cf-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="e01cf-132">Se não tiver êxito, `4xx` um erro será retornado com os detalhes de erro específicos.</span><span class="sxs-lookup"><span data-stu-id="e01cf-132">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="e01cf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e01cf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e01cf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e01cf-134">Request</span></span>

<span data-ttu-id="e01cf-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e01cf-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e01cf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e01cf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="e01cf-137">C#</span><span class="sxs-lookup"><span data-stu-id="e01cf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e01cf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e01cf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e01cf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e01cf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e01cf-140">Java</span><span class="sxs-lookup"><span data-stu-id="e01cf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e01cf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01cf-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
