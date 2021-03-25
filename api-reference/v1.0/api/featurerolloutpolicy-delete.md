---
title: Excluir featureRolloutPolicy
description: Exclua um objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b06a82259d2bd0694cf8bf66807a8625d3b1b84
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201352"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="914f6-103">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="914f6-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="914f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="914f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="914f6-105">[Exclua um objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914f6-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="914f6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="914f6-106">Permissions</span></span>

<span data-ttu-id="914f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="914f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="914f6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="914f6-109">Permission type</span></span>                        | <span data-ttu-id="914f6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="914f6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="914f6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="914f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="914f6-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914f6-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="914f6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="914f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="914f6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="914f6-114">Not supported.</span></span> |
| <span data-ttu-id="914f6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="914f6-115">Application</span></span>                            | <span data-ttu-id="914f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="914f6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="914f6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="914f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="914f6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="914f6-118">Request headers</span></span>

| <span data-ttu-id="914f6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="914f6-119">Name</span></span>          | <span data-ttu-id="914f6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="914f6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="914f6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="914f6-121">Authorization</span></span> | <span data-ttu-id="914f6-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="914f6-122">Bearer {token}.</span></span> <span data-ttu-id="914f6-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="914f6-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="914f6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="914f6-124">Request body</span></span>

<span data-ttu-id="914f6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="914f6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="914f6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="914f6-126">Response</span></span>

<span data-ttu-id="914f6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="914f6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="914f6-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="914f6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="914f6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="914f6-130">Request</span></span>

<span data-ttu-id="914f6-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="914f6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="914f6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="914f6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="914f6-133">C#</span><span class="sxs-lookup"><span data-stu-id="914f6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="914f6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="914f6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="914f6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="914f6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="914f6-136">Java</span><span class="sxs-lookup"><span data-stu-id="914f6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="914f6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="914f6-137">Response</span></span>

<span data-ttu-id="914f6-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="914f6-138">The following is an example of the response.</span></span>

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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


