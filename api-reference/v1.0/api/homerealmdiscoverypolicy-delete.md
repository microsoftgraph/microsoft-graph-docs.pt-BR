---
title: Excluir homeRealmDiscoveryPolicy
description: Exclua homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 803b770daa1a1e8f4aa073a83fc6214e2a862991
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434353"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="50013-103">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="50013-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="50013-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50013-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="50013-105">[Exclua um objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="50013-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50013-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50013-106">Permissions</span></span>

<span data-ttu-id="50013-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50013-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50013-109">Permission type</span></span>                        | <span data-ttu-id="50013-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50013-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50013-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50013-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="50013-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="50013-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="50013-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50013-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50013-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50013-114">Not supported.</span></span> |
| <span data-ttu-id="50013-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50013-115">Application</span></span>                            | <span data-ttu-id="50013-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="50013-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="50013-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50013-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="50013-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50013-118">Request headers</span></span>

| <span data-ttu-id="50013-119">Nome</span><span class="sxs-lookup"><span data-stu-id="50013-119">Name</span></span>          | <span data-ttu-id="50013-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="50013-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="50013-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50013-121">Authorization</span></span> | <span data-ttu-id="50013-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50013-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50013-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50013-124">Request body</span></span>

<span data-ttu-id="50013-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50013-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50013-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="50013-126">Response</span></span>

<span data-ttu-id="50013-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50013-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="50013-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="50013-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50013-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50013-129">Request</span></span>

<span data-ttu-id="50013-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50013-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50013-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="50013-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="50013-132">C#</span><span class="sxs-lookup"><span data-stu-id="50013-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50013-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50013-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50013-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50013-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50013-135">Java</span><span class="sxs-lookup"><span data-stu-id="50013-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50013-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="50013-136">Response</span></span>

<span data-ttu-id="50013-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50013-137">The following is an example of the response.</span></span>

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

