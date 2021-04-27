---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e as relações de um objeto featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9a2f650ae6c71e18e5dd69eaeb015dbd5f87c4e9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042328"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="8ad9c-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="8ad9c-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="8ad9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ad9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad9c-105">Recupere as propriedades e as relações de um [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ad9c-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ad9c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ad9c-106">Permissions</span></span>

<span data-ttu-id="8ad9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ad9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ad9c-109">Permission type</span></span>                        | <span data-ttu-id="8ad9c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ad9c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ad9c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ad9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ad9c-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad9c-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="8ad9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ad9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ad9c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-114">Not supported.</span></span> |
| <span data-ttu-id="8ad9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ad9c-115">Application</span></span>                            | <span data-ttu-id="8ad9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ad9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ad9c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ad9c-118">Optional query parameters</span></span>

<span data-ttu-id="8ad9c-119">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="8ad9c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8ad9c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ad9c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad9c-121">Request headers</span></span>

| <span data-ttu-id="8ad9c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8ad9c-122">Name</span></span>      |<span data-ttu-id="8ad9c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ad9c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ad9c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ad9c-124">Authorization</span></span> | <span data-ttu-id="8ad9c-125">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-125">Bearer {token}.</span></span> <span data-ttu-id="8ad9c-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8ad9c-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ad9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad9c-127">Request body</span></span>

<span data-ttu-id="8ad9c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ad9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad9c-129">Response</span></span>

<span data-ttu-id="8ad9c-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ad9c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ad9c-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="8ad9c-132">Exemplo 1: obter uma política de lançamento de recursos</span><span class="sxs-lookup"><span data-stu-id="8ad9c-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="8ad9c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad9c-133">Request</span></span>

<span data-ttu-id="8ad9c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ad9c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad9c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="8ad9c-136">C#</span><span class="sxs-lookup"><span data-stu-id="8ad9c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ad9c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ad9c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ad9c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ad9c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ad9c-139">Java</span><span class="sxs-lookup"><span data-stu-id="8ad9c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8ad9c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad9c-140">Response</span></span>

<span data-ttu-id="8ad9c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-141">The following is an example of the response.</span></span>

> <span data-ttu-id="8ad9c-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="8ad9c-143">Exemplo 2: obter uma política de lançamento de recursos e expandir appliesTo</span><span class="sxs-lookup"><span data-stu-id="8ad9c-143">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="8ad9c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ad9c-144">Request</span></span>

<span data-ttu-id="8ad9c-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ad9c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad9c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expandAppliesTo_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="8ad9c-147">C#</span><span class="sxs-lookup"><span data-stu-id="8ad9c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-expandappliesto-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ad9c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ad9c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-expandappliesto-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ad9c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ad9c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-expandappliesto-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ad9c-150">Java</span><span class="sxs-lookup"><span data-stu-id="8ad9c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-expandappliesto-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8ad9c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ad9c-151">Response</span></span>

<span data-ttu-id="8ad9c-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-152">The following is an example of the response.</span></span>

> <span data-ttu-id="8ad9c-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ad9c-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


