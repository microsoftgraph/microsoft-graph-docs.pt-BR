---
title: Excluir homeRealmDiscoveryPolicy
description: Exclua homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d18b0f018eb23bf0513507884ede82cc6a9fd234
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435725"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="2ed7b-103">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="2ed7b-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="2ed7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ed7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ed7b-105">[Exclua um objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ed7b-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ed7b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ed7b-106">Permissions</span></span>

<span data-ttu-id="2ed7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ed7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ed7b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ed7b-109">Permission type</span></span>                        | <span data-ttu-id="2ed7b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ed7b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ed7b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ed7b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ed7b-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ed7b-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="2ed7b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ed7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ed7b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ed7b-114">Not supported.</span></span> |
| <span data-ttu-id="2ed7b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ed7b-115">Application</span></span>                            | <span data-ttu-id="2ed7b-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ed7b-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ed7b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed7b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ed7b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed7b-118">Request headers</span></span>

| <span data-ttu-id="2ed7b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ed7b-119">Name</span></span>          | <span data-ttu-id="2ed7b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed7b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ed7b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ed7b-121">Authorization</span></span> | <span data-ttu-id="2ed7b-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2ed7b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ed7b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed7b-123">Request body</span></span>

<span data-ttu-id="2ed7b-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ed7b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed7b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed7b-125">Response</span></span>

<span data-ttu-id="2ed7b-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ed7b-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2ed7b-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ed7b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ed7b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed7b-128">Request</span></span>

<span data-ttu-id="2ed7b-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ed7b-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ed7b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed7b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="2ed7b-131">C#</span><span class="sxs-lookup"><span data-stu-id="2ed7b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ed7b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ed7b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ed7b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ed7b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ed7b-134">Java</span><span class="sxs-lookup"><span data-stu-id="2ed7b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ed7b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed7b-135">Response</span></span>

<span data-ttu-id="2ed7b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ed7b-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


