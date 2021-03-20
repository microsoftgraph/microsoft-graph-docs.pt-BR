---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e as relações de um objeto featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 956f5cada595471a1e9425b1399c69b4f4bc728c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955921"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="ba280-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="ba280-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="ba280-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba280-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba280-105">Recupere as propriedades e as relações de um [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba280-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba280-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba280-106">Permissions</span></span>

<span data-ttu-id="ba280-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba280-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba280-109">Permission type</span></span>                        | <span data-ttu-id="ba280-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba280-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba280-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba280-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba280-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba280-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="ba280-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba280-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba280-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba280-114">Not supported.</span></span> |
| <span data-ttu-id="ba280-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba280-115">Application</span></span>                            | <span data-ttu-id="ba280-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba280-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba280-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba280-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba280-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba280-118">Optional query parameters</span></span>

<span data-ttu-id="ba280-119">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba280-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="ba280-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ba280-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba280-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba280-121">Request headers</span></span>

| <span data-ttu-id="ba280-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ba280-122">Name</span></span>      |<span data-ttu-id="ba280-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba280-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba280-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba280-124">Authorization</span></span> | <span data-ttu-id="ba280-125">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="ba280-125">Bearer {token}.</span></span> <span data-ttu-id="ba280-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ba280-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba280-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba280-127">Request body</span></span>

<span data-ttu-id="ba280-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba280-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba280-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba280-129">Response</span></span>

<span data-ttu-id="ba280-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba280-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba280-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba280-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="ba280-132">Exemplo 1: obter uma política de lançamento de recursos</span><span class="sxs-lookup"><span data-stu-id="ba280-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="ba280-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba280-133">Request</span></span>

<span data-ttu-id="ba280-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba280-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
#### <a name="response"></a><span data-ttu-id="ba280-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba280-135">Response</span></span>

<span data-ttu-id="ba280-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba280-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ba280-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba280-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="ba280-139">Exemplo 2: obter uma política de lançamento de recursos e expandir appliesTo</span><span class="sxs-lookup"><span data-stu-id="ba280-139">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="ba280-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba280-140">Request</span></span>

<span data-ttu-id="ba280-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba280-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expandAppliesTo_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```

#### <a name="response"></a><span data-ttu-id="ba280-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba280-142">Response</span></span>

<span data-ttu-id="ba280-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba280-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ba280-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba280-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


