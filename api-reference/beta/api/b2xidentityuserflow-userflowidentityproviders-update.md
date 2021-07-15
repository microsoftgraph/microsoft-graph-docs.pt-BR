---
title: Atualizar um userFlowIdentityProvider
description: Atualize um identityProvider em um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4b0640cd6843873d720ddc6547e15beb89f7f0f8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439522"
---
# <a name="update-a-userflowidentityprovider"></a><span data-ttu-id="bf9a7-103">Atualizar um userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="bf9a7-103">Update a userFlowIdentityProvider</span></span>

<span data-ttu-id="bf9a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf9a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf9a7-105">Atualize um provedor de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="bf9a7-105">Update an identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf9a7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bf9a7-106">Permissions</span></span>

<span data-ttu-id="bf9a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf9a7-109">Permission type</span></span>      | <span data-ttu-id="bf9a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf9a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf9a7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf9a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf9a7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9a7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bf9a7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf9a7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bf9a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-114">Not supported.</span></span>|
|<span data-ttu-id="bf9a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf9a7-115">Application</span></span>| <span data-ttu-id="bf9a7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9a7-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bf9a7-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="bf9a7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bf9a7-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bf9a7-118">Global administrator</span></span>
* <span data-ttu-id="bf9a7-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="bf9a7-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bf9a7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9a7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bf9a7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9a7-121">Request headers</span></span>

|<span data-ttu-id="bf9a7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bf9a7-122">Name</span></span>|<span data-ttu-id="bf9a7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf9a7-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bf9a7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf9a7-124">Authorization</span></span>|<span data-ttu-id="bf9a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf9a7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf9a7-127">Content-Type</span></span>|<span data-ttu-id="bf9a7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf9a7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9a7-130">Request body</span></span>

<span data-ttu-id="bf9a7-131">No corpo da solicitação, forneça uma representação JSON com a `id` [identidadeProvider](../resources/identityproviderbase.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="bf9a7-132">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="bf9a7-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="bf9a7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf9a7-133">Response</span></span>

<span data-ttu-id="bf9a7-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="bf9a7-135">Se não tiver êxito, `4xx` um erro será retornado com os detalhes de erro específicos.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="bf9a7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf9a7-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf9a7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf9a7-137">Request</span></span>

<span data-ttu-id="bf9a7-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf9a7-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bf9a7-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9a7-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_userflowidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"
}
```
# <a name="c"></a>[<span data-ttu-id="bf9a7-140">C#</span><span class="sxs-lookup"><span data-stu-id="bf9a7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-userflowidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf9a7-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf9a7-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-userflowidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf9a7-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf9a7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-userflowidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf9a7-143">Java</span><span class="sxs-lookup"><span data-stu-id="bf9a7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2xuserflows-userflowidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf9a7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf9a7-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
