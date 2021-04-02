---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e as relações de um objeto featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6cb7f140e29e15643850352ea2107b77b9a96495
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508629"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="e8995-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e8995-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="e8995-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8995-105">Recupere as propriedades e as relações de um [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8995-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8995-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8995-106">Permissions</span></span>

<span data-ttu-id="e8995-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8995-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8995-109">Permission type</span></span>                        | <span data-ttu-id="e8995-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8995-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8995-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8995-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8995-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8995-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="e8995-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8995-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8995-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8995-114">Not supported.</span></span> |
| <span data-ttu-id="e8995-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8995-115">Application</span></span>                            | <span data-ttu-id="e8995-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8995-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8995-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8995-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8995-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8995-118">Optional query parameters</span></span>

<span data-ttu-id="e8995-119">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8995-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e8995-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8995-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8995-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8995-121">Request headers</span></span>

| <span data-ttu-id="e8995-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8995-122">Name</span></span>      |<span data-ttu-id="e8995-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8995-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8995-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8995-124">Authorization</span></span> | <span data-ttu-id="e8995-125">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="e8995-125">Bearer {token}.</span></span> <span data-ttu-id="e8995-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e8995-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8995-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8995-127">Request body</span></span>

<span data-ttu-id="e8995-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8995-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8995-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8995-129">Response</span></span>

<span data-ttu-id="e8995-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8995-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8995-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8995-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="e8995-132">Exemplo 1: obter uma política de lançamento de recursos</span><span class="sxs-lookup"><span data-stu-id="e8995-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="e8995-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8995-133">Request</span></span>

<span data-ttu-id="e8995-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8995-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8995-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8995-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="e8995-136">C#</span><span class="sxs-lookup"><span data-stu-id="e8995-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8995-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8995-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8995-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8995-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8995-139">Java</span><span class="sxs-lookup"><span data-stu-id="e8995-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e8995-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8995-140">Response</span></span>

<span data-ttu-id="e8995-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8995-141">The following is an example of the response.</span></span>

> <span data-ttu-id="e8995-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8995-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="e8995-144">Exemplo 2: obter uma política de lançamento de recursos e expandir appliesTo</span><span class="sxs-lookup"><span data-stu-id="e8995-144">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="e8995-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8995-145">Request</span></span>

<span data-ttu-id="e8995-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8995-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8995-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8995-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expandAppliesTo_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="e8995-148">C#</span><span class="sxs-lookup"><span data-stu-id="e8995-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-expandappliesto-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8995-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8995-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-expandappliesto-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8995-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8995-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-expandappliesto-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8995-151">Java</span><span class="sxs-lookup"><span data-stu-id="e8995-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-expandappliesto-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e8995-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8995-152">Response</span></span>

<span data-ttu-id="e8995-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8995-153">The following is an example of the response.</span></span>

> <span data-ttu-id="e8995-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8995-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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


