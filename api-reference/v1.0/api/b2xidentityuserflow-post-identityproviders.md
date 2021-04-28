---
title: Adicionar identityProvider
description: Adicione um provedor de identidade a um fluxo de usuário B2X.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 6ec01ec32cedf3bd1464058c9a8261e925505422
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054613"
---
# <a name="add-identityprovider"></a><span data-ttu-id="bc4f9-103">Adicionar identityProvider</span><span class="sxs-lookup"><span data-stu-id="bc4f9-103">Add identityProvider</span></span>

<span data-ttu-id="bc4f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc4f9-105">Atualize os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="bc4f9-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc4f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc4f9-106">Permissions</span></span>

<span data-ttu-id="bc4f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc4f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc4f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc4f9-109">Permission type</span></span>      | <span data-ttu-id="bc4f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc4f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc4f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc4f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc4f9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc4f9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bc4f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc4f9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bc4f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-114">Not supported.</span></span>|
|<span data-ttu-id="bc4f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc4f9-115">Application</span></span>| <span data-ttu-id="bc4f9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc4f9-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bc4f9-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="bc4f9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bc4f9-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bc4f9-118">Global administrator</span></span>
* <span data-ttu-id="bc4f9-119">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="bc4f9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bc4f9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc4f9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bc4f9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc4f9-121">Request headers</span></span>

|<span data-ttu-id="bc4f9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bc4f9-122">Name</span></span>|<span data-ttu-id="bc4f9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc4f9-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bc4f9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc4f9-124">Authorization</span></span>|<span data-ttu-id="bc4f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bc4f9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc4f9-127">Content-Type</span></span>|<span data-ttu-id="bc4f9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc4f9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc4f9-130">Request body</span></span>

<span data-ttu-id="bc4f9-131">No corpo da solicitação, forneça uma representação JSON da `id` [identidadeProvider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="bc4f9-132">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="bc4f9-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="bc4f9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc4f9-133">Response</span></span>

<span data-ttu-id="bc4f9-134">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="bc4f9-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="bc4f9-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc4f9-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc4f9-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc4f9-137">Request</span></span>

<span data-ttu-id="bc4f9-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bc4f9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc4f9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"
}
```
# <a name="c"></a>[<span data-ttu-id="bc4f9-140">C#</span><span class="sxs-lookup"><span data-stu-id="bc4f9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc4f9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc4f9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc4f9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc4f9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc4f9-143">Java</span><span class="sxs-lookup"><span data-stu-id="bc4f9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2xuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc4f9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc4f9-144">Response</span></span>

<span data-ttu-id="bc4f9-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc4f9-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
