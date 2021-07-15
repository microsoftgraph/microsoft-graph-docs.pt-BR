---
title: Adicionar um userFlowIdentityProvider
description: Adicione um identityProvider a um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: c183cd97377004d60485dcacf0bf372f8957f0b8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439658"
---
# <a name="add-a-userflowidentityprovider"></a><span data-ttu-id="ace55-103">Adicionar um userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="ace55-103">Add a userFlowIdentityProvider</span></span>

<span data-ttu-id="ace55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ace55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ace55-105">Adicione um provedor de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ace55-105">Add an identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ace55-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ace55-106">Permissions</span></span>

<span data-ttu-id="ace55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ace55-109">Permission type</span></span>      | <span data-ttu-id="ace55-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ace55-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace55-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ace55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ace55-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace55-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ace55-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ace55-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ace55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ace55-114">Not supported.</span></span>|
|<span data-ttu-id="ace55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ace55-115">Application</span></span>| <span data-ttu-id="ace55-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace55-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ace55-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ace55-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ace55-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ace55-118">Global administrator</span></span>
* <span data-ttu-id="ace55-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="ace55-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ace55-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ace55-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ace55-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ace55-121">Request headers</span></span>

|<span data-ttu-id="ace55-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ace55-122">Name</span></span>|<span data-ttu-id="ace55-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ace55-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ace55-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ace55-124">Authorization</span></span>|<span data-ttu-id="ace55-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ace55-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ace55-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ace55-127">Content-Type</span></span>|<span data-ttu-id="ace55-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ace55-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace55-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ace55-130">Request body</span></span>

<span data-ttu-id="ace55-131">No corpo da solicitação, forneça uma representação JSON com a `id` [identidadeProvider](../resources/identityproviderbase.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="ace55-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="ace55-132">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte o [recurso identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="ace55-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="ace55-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace55-133">Response</span></span>

<span data-ttu-id="ace55-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ace55-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ace55-135">Se não tiver êxito, `4xx` um erro será retornado com os detalhes de erro específicos.</span><span class="sxs-lookup"><span data-stu-id="ace55-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="ace55-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ace55-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ace55-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ace55-137">Request</span></span>

<span data-ttu-id="ace55-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ace55-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ace55-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ace55-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_userflowIdentityProviders"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="ace55-140">C#</span><span class="sxs-lookup"><span data-stu-id="ace55-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ace55-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ace55-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ace55-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ace55-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ace55-143">Java</span><span class="sxs-lookup"><span data-stu-id="ace55-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ace55-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace55-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
