---
title: Criar featureRolloutPolicy
description: Criar um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d7d670303748893fdb7e5825369861dea502178
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963203"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="3a271-103">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="3a271-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="3a271-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a271-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a271-105">Criar um novo objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3a271-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a271-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a271-106">Permissions</span></span>

<span data-ttu-id="3a271-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a271-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a271-109">Permission type</span></span>                        | <span data-ttu-id="3a271-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a271-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a271-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a271-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a271-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="3a271-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="3a271-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a271-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a271-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a271-114">Not supported.</span></span> |
| <span data-ttu-id="3a271-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a271-115">Application</span></span>                            | <span data-ttu-id="3a271-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a271-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a271-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a271-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3a271-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a271-118">Request headers</span></span>

| <span data-ttu-id="3a271-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3a271-119">Name</span></span>          | <span data-ttu-id="3a271-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a271-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3a271-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a271-121">Authorization</span></span> | <span data-ttu-id="3a271-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3a271-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a271-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a271-123">Request body</span></span>

<span data-ttu-id="3a271-124">No corpo da solicitação, forneça uma representação JSON do objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3a271-124">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="3a271-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a271-125">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="3a271-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a271-126">Parameter</span></span> | <span data-ttu-id="3a271-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a271-127">Type</span></span> | <span data-ttu-id="3a271-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a271-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a271-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3a271-129">displayName</span></span> |<span data-ttu-id="3a271-130">string</span><span class="sxs-lookup"><span data-stu-id="3a271-130">string</span></span> |<span data-ttu-id="3a271-131">O nome de exibição desta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="3a271-131">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="3a271-132">apresentam</span><span class="sxs-lookup"><span data-stu-id="3a271-132">feature</span></span> |<span data-ttu-id="3a271-133">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="3a271-133">stagedFeatureName</span></span> |<span data-ttu-id="3a271-134">O recurso que seria implantado usando esta política.</span><span class="sxs-lookup"><span data-stu-id="3a271-134">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="3a271-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3a271-135">isEnabled</span></span> |<span data-ttu-id="3a271-136">string</span><span class="sxs-lookup"><span data-stu-id="3a271-136">string</span></span> |<span data-ttu-id="3a271-137">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="3a271-137">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="3a271-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a271-138">Response</span></span>

<span data-ttu-id="3a271-139">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a271-139">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a271-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a271-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a271-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a271-141">Request</span></span>

<span data-ttu-id="3a271-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a271-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a271-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a271-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3a271-144">C#</span><span class="sxs-lookup"><span data-stu-id="3a271-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a271-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a271-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a271-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a271-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a271-147">Java</span><span class="sxs-lookup"><span data-stu-id="3a271-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a271-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a271-148">Response</span></span>

<span data-ttu-id="3a271-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a271-149">The following is an example of the response.</span></span>

> <span data-ttu-id="3a271-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a271-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


