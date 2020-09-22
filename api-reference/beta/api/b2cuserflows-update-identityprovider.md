---
title: Adicionar identityprovider a um b2cUserFlow
description: Adicionar identityprovider a um b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 155524d9c84759028dfa630888722b896a603e25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991450"
---
# <a name="add-identityprovider-to-a-b2cuserflow"></a><span data-ttu-id="5e953-103">Adicionar identityprovider a um b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="5e953-103">Add identityProvider to a b2cUserFlow</span></span>

<span data-ttu-id="5e953-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e953-105">Adicionar provedores de identidade em um objeto [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="5e953-105">Add identity providers in a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e953-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e953-106">Permissions</span></span>

<span data-ttu-id="5e953-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e953-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e953-109">Permission type</span></span>      | <span data-ttu-id="5e953-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e953-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e953-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e953-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e953-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5e953-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5e953-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e953-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5e953-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e953-114">Not supported.</span></span>|
|<span data-ttu-id="5e953-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e953-115">Application</span></span>| <span data-ttu-id="5e953-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5e953-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5e953-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="5e953-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5e953-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5e953-118">Global administrator</span></span>
* <span data-ttu-id="5e953-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="5e953-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5e953-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e953-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5e953-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e953-121">Request headers</span></span>

|<span data-ttu-id="5e953-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5e953-122">Name</span></span>|<span data-ttu-id="5e953-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e953-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5e953-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e953-124">Authorization</span></span>|<span data-ttu-id="5e953-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e953-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5e953-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e953-127">Content-Type</span></span>|<span data-ttu-id="5e953-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e953-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e953-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e953-130">Request body</span></span>

<span data-ttu-id="5e953-131">No corpo da solicitação, forneça uma representação JSON do `id` [identityprovider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="5e953-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="5e953-132">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuário, consulte a referência da API [identityProviders](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="5e953-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="5e953-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e953-133">Response</span></span>

<span data-ttu-id="5e953-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5e953-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="5e953-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="5e953-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="5e953-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e953-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e953-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e953-137">Request</span></span>

<span data-ttu-id="5e953-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e953-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5e953-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e953-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5e953-140">C#</span><span class="sxs-lookup"><span data-stu-id="5e953-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e953-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e953-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e953-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e953-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e953-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e953-143">Response</span></span>

<span data-ttu-id="5e953-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e953-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


