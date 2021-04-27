---
title: Criar tokenIssuancePolicy
description: Crie um novo tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b99aed5506bab54072838d5d48ed0b51c3e4292d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051792"
---
# <a name="create-tokenissuancepolicy"></a><span data-ttu-id="a4b9a-103">Criar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="a4b9a-103">Create tokenIssuancePolicy</span></span>

<span data-ttu-id="a4b9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4b9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4b9a-105">Crie um novo [objeto tokenIssuancePolicy.](../resources/tokenissuancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a4b9a-105">Create a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4b9a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4b9a-106">Permissions</span></span>

<span data-ttu-id="a4b9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4b9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4b9a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4b9a-109">Permission type</span></span>                        | <span data-ttu-id="a4b9a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4b9a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a4b9a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4b9a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4b9a-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4b9a-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a4b9a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4b9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4b9a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-114">Not supported.</span></span> |
| <span data-ttu-id="a4b9a-115">Application</span><span class="sxs-lookup"><span data-stu-id="a4b9a-115">Application</span></span>                            | <span data-ttu-id="a4b9a-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4b9a-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4b9a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4b9a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a4b9a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b9a-118">Request headers</span></span>

| <span data-ttu-id="a4b9a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a4b9a-119">Name</span></span>          | <span data-ttu-id="a4b9a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4b9a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a4b9a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4b9a-121">Authorization</span></span> | <span data-ttu-id="a4b9a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4b9a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a4b9a-124">Content-type</span></span> | <span data-ttu-id="a4b9a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4b9a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b9a-127">Request body</span></span>

<span data-ttu-id="a4b9a-128">No corpo da solicitação, fornece uma representação JSON de [um objeto tokenIssuancePolicy.](../resources/tokenissuancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a4b9a-128">In the request body, supply a JSON representation of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a4b9a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4b9a-129">Response</span></span>

<span data-ttu-id="a4b9a-130">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto tokenIssuancePolicy](../resources/tokenissuancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-130">If successful, this method returns a `201 Created` response code and a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4b9a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4b9a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4b9a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4b9a-132">Request</span></span>

<span data-ttu-id="a4b9a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4b9a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4b9a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenIssuancePolicies_from_tokenIssuancePolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="a4b9a-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4b9a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicies-from-tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4b9a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4b9a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicies-from-tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4b9a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4b9a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicies-from-tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4b9a-138">Java</span><span class="sxs-lookup"><span data-stu-id="a4b9a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenissuancepolicies-from-tokenissuancepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="a4b9a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4b9a-139">Response</span></span>

<span data-ttu-id="a4b9a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a4b9a-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4b9a-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Create tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


