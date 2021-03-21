---
title: Criar featureRolloutPolicy
description: Crie um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0a88d66594d9fa345c54a999f6452a7a287d0b08
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964607"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="cfaf8-103">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="cfaf8-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="cfaf8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfaf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfaf8-105">Crie um novo [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cfaf8-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfaf8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfaf8-106">Permissions</span></span>

<span data-ttu-id="cfaf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfaf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfaf8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfaf8-109">Permission type</span></span>                        | <span data-ttu-id="cfaf8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfaf8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfaf8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfaf8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfaf8-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfaf8-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="cfaf8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfaf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfaf8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-114">Not supported.</span></span> |
| <span data-ttu-id="cfaf8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfaf8-115">Application</span></span>                            | <span data-ttu-id="cfaf8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfaf8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfaf8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cfaf8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfaf8-118">Request headers</span></span>

| <span data-ttu-id="cfaf8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cfaf8-119">Name</span></span>          | <span data-ttu-id="cfaf8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfaf8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cfaf8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfaf8-121">Authorization</span></span> | <span data-ttu-id="cfaf8-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-122">Bearer {token}.</span></span> <span data-ttu-id="cfaf8-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cfaf8-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfaf8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfaf8-124">Request body</span></span>

<span data-ttu-id="cfaf8-125">No corpo da solicitação, fornece uma representação JSON do [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cfaf8-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="cfaf8-126">A tabela a seguir mostra as propriedades que são necessárias ao criar [um featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cfaf8-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="cfaf8-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cfaf8-127">Parameter</span></span> | <span data-ttu-id="cfaf8-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfaf8-128">Type</span></span> | <span data-ttu-id="cfaf8-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfaf8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfaf8-130">displayName</span><span class="sxs-lookup"><span data-stu-id="cfaf8-130">displayName</span></span> |<span data-ttu-id="cfaf8-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfaf8-131">string</span></span> |<span data-ttu-id="cfaf8-132">O nome de exibição dessa política de lançamento de recursos.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="cfaf8-133">feature</span><span class="sxs-lookup"><span data-stu-id="cfaf8-133">feature</span></span> |<span data-ttu-id="cfaf8-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="cfaf8-134">stagedFeatureName</span></span> |<span data-ttu-id="cfaf8-135">O recurso que seria lançado usando essa política.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="cfaf8-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cfaf8-136">isEnabled</span></span> |<span data-ttu-id="cfaf8-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfaf8-137">string</span></span> |<span data-ttu-id="cfaf8-138">Indica se a adoção de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="cfaf8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfaf8-139">Response</span></span>

<span data-ttu-id="cfaf8-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfaf8-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cfaf8-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfaf8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfaf8-142">Request</span></span>

<span data-ttu-id="cfaf8-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_directory"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="cfaf8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfaf8-144">Response</span></span>

<span data-ttu-id="cfaf8-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-145">The following is an example of the response.</span></span>

> <span data-ttu-id="cfaf8-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfaf8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


