---
title: Excluir homeRealmDiscoveryPolicy
description: Exclua homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bae41290ca2395e60cf611c96ccdc46e3e3ff85b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973321"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="4b04e-103">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="4b04e-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="4b04e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b04e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="4b04e-105">Excluir um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4b04e-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b04e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b04e-106">Permissions</span></span>

<span data-ttu-id="4b04e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b04e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b04e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b04e-109">Permission type</span></span>                        | <span data-ttu-id="4b04e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b04e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b04e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b04e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b04e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b04e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="4b04e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b04e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b04e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b04e-114">Not supported.</span></span> |
| <span data-ttu-id="4b04e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b04e-115">Application</span></span>                            | <span data-ttu-id="4b04e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b04e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b04e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b04e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b04e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b04e-118">Request headers</span></span>

| <span data-ttu-id="4b04e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4b04e-119">Name</span></span>          | <span data-ttu-id="4b04e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b04e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b04e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b04e-121">Authorization</span></span> | <span data-ttu-id="4b04e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b04e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b04e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b04e-124">Request body</span></span>

<span data-ttu-id="4b04e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b04e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b04e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b04e-126">Response</span></span>

<span data-ttu-id="4b04e-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4b04e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4b04e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b04e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b04e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b04e-129">Request</span></span>

<span data-ttu-id="4b04e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b04e-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b04e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b04e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="4b04e-132">C#</span><span class="sxs-lookup"><span data-stu-id="4b04e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b04e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b04e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b04e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b04e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b04e-135">Java</span><span class="sxs-lookup"><span data-stu-id="4b04e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b04e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b04e-136">Response</span></span>

<span data-ttu-id="4b04e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b04e-137">The following is an example of the response.</span></span>

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

