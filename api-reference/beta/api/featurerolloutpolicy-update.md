---
title: Atualizar featureRolloutPolicy
description: Atualize as propriedades do objeto featurerolloutpolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 26d5f16bd6d61689ff4cfe73b83c4a45add9c2f7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471079"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="eaaa5-103">Atualizar featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="eaaa5-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="eaaa5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaaa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaaa5-105">Atualize as propriedades do [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa5-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaaa5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaaa5-106">Permissions</span></span>

<span data-ttu-id="eaaa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaaa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eaaa5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaaa5-109">Permission type</span></span>                        | <span data-ttu-id="eaaa5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaaa5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eaaa5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaaa5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eaaa5-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaaa5-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="eaaa5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaaa5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaaa5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-114">Not supported.</span></span> |
| <span data-ttu-id="eaaa5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaaa5-115">Application</span></span>                            | <span data-ttu-id="eaaa5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaaa5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaaa5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eaaa5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaaa5-118">Request headers</span></span>

| <span data-ttu-id="eaaa5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eaaa5-119">Name</span></span>       | <span data-ttu-id="eaaa5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaaa5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eaaa5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaaa5-121">Authorization</span></span> | <span data-ttu-id="eaaa5-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="eaaa5-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaaa5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaaa5-123">Request body</span></span>

<span data-ttu-id="eaaa5-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eaaa5-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eaaa5-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eaaa5-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaaa5-127">Property</span></span>     | <span data-ttu-id="eaaa5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaaa5-128">Type</span></span>        | <span data-ttu-id="eaaa5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaaa5-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eaaa5-130">description</span><span class="sxs-lookup"><span data-stu-id="eaaa5-130">description</span></span>|<span data-ttu-id="eaaa5-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaaa5-131">String</span></span>|<span data-ttu-id="eaaa5-132">Uma descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-132">A description for this policy.</span></span>|
|<span data-ttu-id="eaaa5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eaaa5-133">displayName</span></span>|<span data-ttu-id="eaaa5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaaa5-134">String</span></span>|<span data-ttu-id="eaaa5-135">O nome de exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-135">The display name for this policy.</span></span>|
|<span data-ttu-id="eaaa5-136">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="eaaa5-136">isAppliedToOrganization</span></span>|<span data-ttu-id="eaaa5-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaaa5-137">Boolean</span></span>|<span data-ttu-id="eaaa5-138">Indica se essa política de lançamento de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="eaaa5-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="eaaa5-139">isEnabled</span></span>|<span data-ttu-id="eaaa5-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="eaaa5-140">Boolean</span></span>|<span data-ttu-id="eaaa5-141">Indica se a adoção de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="eaaa5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaaa5-142">Response</span></span>

<span data-ttu-id="eaaa5-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eaaa5-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eaaa5-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eaaa5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaaa5-145">Request</span></span>

<span data-ttu-id="eaaa5-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-146">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eaaa5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaaa5-147">Response</span></span>

<span data-ttu-id="eaaa5-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-148">The following is an example of the response.</span></span>

> <span data-ttu-id="eaaa5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaaa5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


