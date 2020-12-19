---
title: Atualizar featureRolloutPolicy
description: Atualize as propriedades do objeto featurerolloutpolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 676983e4fbffcbe9edf3feae83c8344c52cf4596
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719941"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="0cc56-103">Atualizar featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="0cc56-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="0cc56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cc56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cc56-105">Atualize as propriedades do objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0cc56-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cc56-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cc56-106">Permissions</span></span>

<span data-ttu-id="0cc56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cc56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0cc56-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cc56-109">Permission type</span></span>                        | <span data-ttu-id="0cc56-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cc56-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0cc56-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cc56-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0cc56-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="0cc56-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="0cc56-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cc56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cc56-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cc56-114">Not supported.</span></span> |
| <span data-ttu-id="0cc56-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cc56-115">Application</span></span>                            | <span data-ttu-id="0cc56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cc56-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cc56-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cc56-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0cc56-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc56-118">Request headers</span></span>

| <span data-ttu-id="0cc56-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0cc56-119">Name</span></span>       | <span data-ttu-id="0cc56-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cc56-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0cc56-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cc56-121">Authorization</span></span> | <span data-ttu-id="0cc56-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0cc56-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cc56-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc56-123">Request body</span></span>

<span data-ttu-id="0cc56-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0cc56-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0cc56-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0cc56-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0cc56-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0cc56-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0cc56-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cc56-127">Property</span></span>     | <span data-ttu-id="0cc56-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cc56-128">Type</span></span>        | <span data-ttu-id="0cc56-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cc56-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0cc56-130">description</span><span class="sxs-lookup"><span data-stu-id="0cc56-130">description</span></span>|<span data-ttu-id="0cc56-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cc56-131">String</span></span>|<span data-ttu-id="0cc56-132">Uma descrição para esta política.</span><span class="sxs-lookup"><span data-stu-id="0cc56-132">A description for this policy.</span></span>|
|<span data-ttu-id="0cc56-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0cc56-133">displayName</span></span>|<span data-ttu-id="0cc56-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cc56-134">String</span></span>|<span data-ttu-id="0cc56-135">O nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="0cc56-135">The display name for this policy.</span></span>|
|<span data-ttu-id="0cc56-136">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="0cc56-136">isAppliedToOrganization</span></span>|<span data-ttu-id="0cc56-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="0cc56-137">Boolean</span></span>|<span data-ttu-id="0cc56-138">Indica se esta política de distribuição de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="0cc56-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="0cc56-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0cc56-139">isEnabled</span></span>|<span data-ttu-id="0cc56-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="0cc56-140">Boolean</span></span>|<span data-ttu-id="0cc56-141">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="0cc56-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="0cc56-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cc56-142">Response</span></span>

<span data-ttu-id="0cc56-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cc56-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cc56-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0cc56-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0cc56-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc56-145">Request</span></span>

<span data-ttu-id="0cc56-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cc56-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a
Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="0cc56-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cc56-147">Response</span></span>

<span data-ttu-id="0cc56-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0cc56-148">The following is an example of the response.</span></span>

> <span data-ttu-id="0cc56-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cc56-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update featurerolloutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


