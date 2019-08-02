---
title: Criar featureRolloutPolicy
description: Criar um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 716fa19e8fcccc69a33e53a22360638545ec81f5
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062089"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="e8287-103">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e8287-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8287-104">Criar um novo objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e8287-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8287-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8287-105">Permissions</span></span>

<span data-ttu-id="e8287-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8287-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8287-108">Permission type</span></span>                        | <span data-ttu-id="e8287-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8287-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8287-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8287-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8287-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="e8287-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="e8287-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8287-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8287-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8287-113">Not supported.</span></span> |
| <span data-ttu-id="e8287-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8287-114">Application</span></span>                            | <span data-ttu-id="e8287-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8287-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8287-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8287-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e8287-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8287-117">Request headers</span></span>

| <span data-ttu-id="e8287-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e8287-118">Name</span></span>          | <span data-ttu-id="e8287-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8287-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e8287-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8287-120">Authorization</span></span> | <span data-ttu-id="e8287-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e8287-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8287-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8287-122">Request body</span></span>

<span data-ttu-id="e8287-123">No corpo da solicitação, forneça uma representação JSON do objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e8287-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="e8287-124">A tabela a seguir mostra as propriedades que são necessárias ao criar [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e8287-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="e8287-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e8287-125">Parameter</span></span> | <span data-ttu-id="e8287-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8287-126">Type</span></span> | <span data-ttu-id="e8287-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8287-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8287-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e8287-128">displayName</span></span> |<span data-ttu-id="e8287-129">string</span><span class="sxs-lookup"><span data-stu-id="e8287-129">string</span></span> |<span data-ttu-id="e8287-130">O nome de exibição desta política de distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="e8287-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="e8287-131">apresentam</span><span class="sxs-lookup"><span data-stu-id="e8287-131">feature</span></span> |<span data-ttu-id="e8287-132">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="e8287-132">stagedFeatureName</span></span> |<span data-ttu-id="e8287-133">O recurso que seria implantado usando esta política.</span><span class="sxs-lookup"><span data-stu-id="e8287-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="e8287-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e8287-134">isEnabled</span></span> |<span data-ttu-id="e8287-135">string</span><span class="sxs-lookup"><span data-stu-id="e8287-135">string</span></span> |<span data-ttu-id="e8287-136">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="e8287-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="e8287-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8287-137">Response</span></span>

<span data-ttu-id="e8287-138">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8287-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8287-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8287-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8287-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8287-140">Request</span></span>

<span data-ttu-id="e8287-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8287-141">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8287-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8287-142">Response</span></span>

<span data-ttu-id="e8287-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8287-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e8287-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8287-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
