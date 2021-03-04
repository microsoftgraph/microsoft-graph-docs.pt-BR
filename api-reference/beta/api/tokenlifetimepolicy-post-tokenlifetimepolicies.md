---
title: Criar tokenLifetimePolicy
description: Crie um novo tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 763b80954e12eb3b3dccb9d5c4a6b365dd9994e1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443361"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="6063f-103">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="6063f-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="6063f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6063f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6063f-105">Crie um novo [objeto tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6063f-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6063f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6063f-106">Permissions</span></span>

<span data-ttu-id="6063f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6063f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6063f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6063f-109">Permission type</span></span>                        | <span data-ttu-id="6063f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6063f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6063f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6063f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6063f-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6063f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6063f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6063f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6063f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6063f-114">Not supported.</span></span> |
| <span data-ttu-id="6063f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6063f-115">Application</span></span>                            | <span data-ttu-id="6063f-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6063f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6063f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6063f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6063f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6063f-118">Request headers</span></span>

| <span data-ttu-id="6063f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6063f-119">Name</span></span>          | <span data-ttu-id="6063f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6063f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6063f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6063f-121">Authorization</span></span> | <span data-ttu-id="6063f-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6063f-122">Bearer {token}</span></span> |
| <span data-ttu-id="6063f-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="6063f-123">Content-type</span></span> | <span data-ttu-id="6063f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6063f-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6063f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6063f-125">Request body</span></span>

<span data-ttu-id="6063f-126">No corpo da solicitação, fornece uma representação JSON do [objeto tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6063f-126">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6063f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6063f-127">Response</span></span>

<span data-ttu-id="6063f-128">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6063f-128">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6063f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6063f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6063f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6063f-130">Request</span></span>

<span data-ttu-id="6063f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6063f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6063f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6063f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="6063f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6063f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6063f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6063f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6063f-135">C#</span><span class="sxs-lookup"><span data-stu-id="6063f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6063f-136">Java</span><span class="sxs-lookup"><span data-stu-id="6063f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6063f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6063f-137">Response</span></span>

<span data-ttu-id="6063f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6063f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="6063f-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6063f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


