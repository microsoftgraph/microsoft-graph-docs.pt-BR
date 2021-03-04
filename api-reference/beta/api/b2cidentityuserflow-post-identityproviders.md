---
title: Adicionar identityProvider a um b2cIdentityUserFlow
description: Adicione identityProvider a um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: deb2d5bc6984865dcb665404fca9e897899a2df5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438257"
---
# <a name="add-identityprovider-to-a-b2cidentityuserflow"></a><span data-ttu-id="ee5ba-103">Adicionar identityProvider a um b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="ee5ba-103">Add identityProvider to a b2cIdentityUserFlow</span></span>

<span data-ttu-id="ee5ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee5ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee5ba-105">Adicione provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ee5ba-105">Add identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee5ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee5ba-106">Permissions</span></span>

<span data-ttu-id="ee5ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee5ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee5ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee5ba-109">Permission type</span></span>      | <span data-ttu-id="ee5ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee5ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee5ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee5ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee5ba-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee5ba-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ee5ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee5ba-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ee5ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-114">Not supported.</span></span>|
|<span data-ttu-id="ee5ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee5ba-115">Application</span></span>| <span data-ttu-id="ee5ba-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee5ba-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ee5ba-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ee5ba-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ee5ba-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ee5ba-118">Global administrator</span></span>
* <span data-ttu-id="ee5ba-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="ee5ba-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ee5ba-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee5ba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ee5ba-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5ba-121">Request headers</span></span>

|<span data-ttu-id="ee5ba-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ee5ba-122">Name</span></span>|<span data-ttu-id="ee5ba-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5ba-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ee5ba-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee5ba-124">Authorization</span></span>|<span data-ttu-id="ee5ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee5ba-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee5ba-127">Content-Type</span></span>|<span data-ttu-id="ee5ba-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee5ba-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5ba-130">Request body</span></span>

<span data-ttu-id="ee5ba-131">No corpo da solicitação, forneça uma representação JSON da `id` [identidadeProvider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="ee5ba-132">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="ee5ba-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="ee5ba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee5ba-133">Response</span></span>

<span data-ttu-id="ee5ba-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ee5ba-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ee5ba-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee5ba-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee5ba-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee5ba-137">Request</span></span>

<span data-ttu-id="ee5ba-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee5ba-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee5ba-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="ee5ba-140">C#</span><span class="sxs-lookup"><span data-stu-id="ee5ba-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee5ba-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee5ba-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee5ba-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee5ba-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee5ba-143">Java</span><span class="sxs-lookup"><span data-stu-id="ee5ba-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee5ba-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee5ba-144">Response</span></span>

<span data-ttu-id="ee5ba-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee5ba-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


