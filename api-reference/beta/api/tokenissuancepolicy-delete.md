---
title: Excluir tokenIssuancePolicy
description: Exclua tokenIssuancePolicy.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 974c1e912d0934c03080af4d8c80fd7f388b575d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219267"
---
# <a name="delete-tokenissuancepolicy"></a><span data-ttu-id="addb4-103">Excluir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="addb4-103">Delete tokenIssuancePolicy</span></span>

<span data-ttu-id="addb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="addb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="addb4-105">Excluir um objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="addb4-105">Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="addb4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="addb4-106">Permissions</span></span>

<span data-ttu-id="addb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="addb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="addb4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="addb4-109">Permission type</span></span>                        | <span data-ttu-id="addb4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="addb4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="addb4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="addb4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="addb4-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="addb4-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="addb4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="addb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="addb4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="addb4-114">Not supported.</span></span> |
| <span data-ttu-id="addb4-115">Application</span><span class="sxs-lookup"><span data-stu-id="addb4-115">Application</span></span>                            | <span data-ttu-id="addb4-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="addb4-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="addb4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="addb4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="addb4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="addb4-118">Request headers</span></span>

| <span data-ttu-id="addb4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="addb4-119">Name</span></span>          | <span data-ttu-id="addb4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="addb4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="addb4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="addb4-121">Authorization</span></span> | <span data-ttu-id="addb4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="addb4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="addb4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="addb4-124">Request body</span></span>

<span data-ttu-id="addb4-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="addb4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="addb4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="addb4-126">Response</span></span>

<span data-ttu-id="addb4-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="addb4-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="addb4-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="addb4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="addb4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="addb4-129">Request</span></span>

<span data-ttu-id="addb4-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="addb4-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="addb4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="addb4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="addb4-132">C#</span><span class="sxs-lookup"><span data-stu-id="addb4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="addb4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="addb4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="addb4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="addb4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="addb4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="addb4-135">Response</span></span>

<span data-ttu-id="addb4-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="addb4-136">The following is an example of the response.</span></span>

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
  "description": "Delete tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
