---
title: Criar featureRolloutPolicy
description: Criar um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc2ed04abef450415cc4ee9802cceed687dc324b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435196"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="86a5a-103">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="86a5a-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="86a5a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="86a5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a5a-105">Criar um novo objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="86a5a-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86a5a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86a5a-106">Permissions</span></span>

<span data-ttu-id="86a5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86a5a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86a5a-109">Permission type</span></span>                        | <span data-ttu-id="86a5a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86a5a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86a5a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86a5a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86a5a-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="86a5a-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="86a5a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86a5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86a5a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a5a-114">Not supported.</span></span> |
| <span data-ttu-id="86a5a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86a5a-115">Application</span></span>                            | <span data-ttu-id="86a5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a5a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86a5a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86a5a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="86a5a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86a5a-118">Request headers</span></span>

| <span data-ttu-id="86a5a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="86a5a-119">Name</span></span>          | <span data-ttu-id="86a5a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a5a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="86a5a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86a5a-121">Authorization</span></span> | <span data-ttu-id="86a5a-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="86a5a-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86a5a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86a5a-123">Request body</span></span>

<span data-ttu-id="86a5a-124">No corpo da solicitação, forneça uma representação JSON do objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="86a5a-124">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="86a5a-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86a5a-125">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="86a5a-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86a5a-126">Parameter</span></span> | <span data-ttu-id="86a5a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a5a-127">Type</span></span> | <span data-ttu-id="86a5a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a5a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86a5a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="86a5a-129">displayName</span></span> |<span data-ttu-id="86a5a-130">string</span><span class="sxs-lookup"><span data-stu-id="86a5a-130">string</span></span> |<span data-ttu-id="86a5a-131">O nome de exibição desta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="86a5a-131">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="86a5a-132">apresentam</span><span class="sxs-lookup"><span data-stu-id="86a5a-132">feature</span></span> |<span data-ttu-id="86a5a-133">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="86a5a-133">stagedFeatureName</span></span> |<span data-ttu-id="86a5a-134">O recurso que seria implantado usando esta política.</span><span class="sxs-lookup"><span data-stu-id="86a5a-134">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="86a5a-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="86a5a-135">isEnabled</span></span> |<span data-ttu-id="86a5a-136">string</span><span class="sxs-lookup"><span data-stu-id="86a5a-136">string</span></span> |<span data-ttu-id="86a5a-137">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="86a5a-137">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="86a5a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a5a-138">Response</span></span>

<span data-ttu-id="86a5a-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86a5a-139">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86a5a-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="86a5a-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86a5a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86a5a-141">Request</span></span>

<span data-ttu-id="86a5a-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86a5a-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86a5a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="86a5a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_directory"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="86a5a-144">C#</span><span class="sxs-lookup"><span data-stu-id="86a5a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86a5a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86a5a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86a5a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86a5a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86a5a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a5a-147">Response</span></span>

<span data-ttu-id="86a5a-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86a5a-148">The following is an example of the response.</span></span>

> <span data-ttu-id="86a5a-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86a5a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
