---
title: Adicionar identityprovider a um b2xUserFlow
description: Adicionar identityprovider em um b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 792b3ccd9d8020af7139108efd93e0cb430385d7
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329495"
---
# <a name="add-identityprovider-to-a-b2xuserflow"></a><span data-ttu-id="bbe03-103">Adicionar identityprovider a um b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="bbe03-103">Add identityProvider to a b2xUserFlow</span></span>

<span data-ttu-id="bbe03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbe03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe03-105">Atualize os provedores de identidade em um objeto [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="bbe03-105">Update the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbe03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbe03-106">Permissions</span></span>

<span data-ttu-id="bbe03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbe03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbe03-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbe03-109">Permission type</span></span>      | <span data-ttu-id="bbe03-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbe03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbe03-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbe03-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bbe03-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bbe03-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bbe03-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbe03-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bbe03-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbe03-114">Not supported.</span></span>|
|<span data-ttu-id="bbe03-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbe03-115">Application</span></span>| <span data-ttu-id="bbe03-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bbe03-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bbe03-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="bbe03-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bbe03-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bbe03-118">Global administrator</span></span>
* <span data-ttu-id="bbe03-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="bbe03-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bbe03-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbe03-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bbe03-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe03-121">Request headers</span></span>

|<span data-ttu-id="bbe03-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bbe03-122">Name</span></span>|<span data-ttu-id="bbe03-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbe03-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bbe03-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbe03-124">Authorization</span></span>|<span data-ttu-id="bbe03-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbe03-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bbe03-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbe03-127">Content-Type</span></span>|<span data-ttu-id="bbe03-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbe03-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbe03-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe03-130">Request body</span></span>

<span data-ttu-id="bbe03-131">No corpo da solicitação, forneça uma representação JSON do `id` [identityprovider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="bbe03-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="bbe03-132">Para os fluxos de usuário de inscrição de autoatendimento, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="bbe03-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="bbe03-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe03-133">Response</span></span>

<span data-ttu-id="bbe03-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bbe03-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="bbe03-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="bbe03-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="bbe03-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbe03-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbe03-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbe03-137">Request</span></span>

<span data-ttu-id="bbe03-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbe03-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bbe03-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbe03-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="bbe03-140">C#</span><span class="sxs-lookup"><span data-stu-id="bbe03-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbe03-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbe03-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbe03-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbe03-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbe03-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbe03-143">Response</span></span>

<span data-ttu-id="bbe03-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bbe03-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
