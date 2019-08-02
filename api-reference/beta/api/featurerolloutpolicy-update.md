---
title: Atualizar featureRolloutPolicy
description: Atualize as propriedades do objeto featurerolloutpolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdbe19a401f10acead10884f02de5d380465e0a
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062091"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="c7189-103">Atualizar featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="c7189-103">Update featurerolloutpolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7189-104">Atualize as propriedades do objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c7189-104">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7189-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7189-105">Permissions</span></span>

<span data-ttu-id="c7189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7189-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7189-108">Permission type</span></span>                        | <span data-ttu-id="c7189-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7189-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7189-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7189-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7189-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="c7189-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="c7189-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7189-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7189-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7189-113">Not supported.</span></span> |
| <span data-ttu-id="c7189-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7189-114">Application</span></span>                            | <span data-ttu-id="c7189-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7189-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7189-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7189-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7189-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7189-117">Request headers</span></span>

| <span data-ttu-id="c7189-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c7189-118">Name</span></span>       | <span data-ttu-id="c7189-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7189-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c7189-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7189-120">Authorization</span></span> | <span data-ttu-id="c7189-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c7189-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7189-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7189-122">Request body</span></span>

<span data-ttu-id="c7189-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c7189-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c7189-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c7189-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c7189-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c7189-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c7189-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7189-126">Property</span></span>     | <span data-ttu-id="c7189-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7189-127">Type</span></span>        | <span data-ttu-id="c7189-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7189-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7189-129">description</span><span class="sxs-lookup"><span data-stu-id="c7189-129">description</span></span>|<span data-ttu-id="c7189-130">String</span><span class="sxs-lookup"><span data-stu-id="c7189-130">String</span></span>|<span data-ttu-id="c7189-131">Uma descrição para esta política.</span><span class="sxs-lookup"><span data-stu-id="c7189-131">A description for this policy.</span></span>|
|<span data-ttu-id="c7189-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c7189-132">displayName</span></span>|<span data-ttu-id="c7189-133">String</span><span class="sxs-lookup"><span data-stu-id="c7189-133">String</span></span>|<span data-ttu-id="c7189-134">O nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="c7189-134">The display name for this policy.</span></span>|
|<span data-ttu-id="c7189-135">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="c7189-135">isAppliedToOrganization</span></span>|<span data-ttu-id="c7189-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c7189-136">Boolean</span></span>|<span data-ttu-id="c7189-137">Indica se esta política de distribuição de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="c7189-137">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="c7189-138">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c7189-138">isEnabled</span></span>|<span data-ttu-id="c7189-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7189-139">Boolean</span></span>|<span data-ttu-id="c7189-140">Indica se a distribuição de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="c7189-140">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="c7189-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7189-141">Response</span></span>

<span data-ttu-id="c7189-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7189-142">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7189-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c7189-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7189-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7189-144">Request</span></span>

<span data-ttu-id="c7189-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7189-145">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7189-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7189-146">Response</span></span>

<span data-ttu-id="c7189-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7189-147">The following is an example of the response.</span></span>

> <span data-ttu-id="c7189-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7189-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
