---
title: Atualizar featureRolloutPolicy
description: Atualize as propriedades do objeto featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8d30e3df9d807289787f599e436427a02544c055
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508584"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="7544e-103">Atualizar featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="7544e-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="7544e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7544e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7544e-105">Atualize as propriedades do [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7544e-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7544e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7544e-106">Permissions</span></span>

<span data-ttu-id="7544e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7544e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7544e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7544e-109">Permission type</span></span>                        | <span data-ttu-id="7544e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7544e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7544e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7544e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7544e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7544e-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7544e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7544e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7544e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7544e-114">Not supported.</span></span> |
| <span data-ttu-id="7544e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7544e-115">Application</span></span>                            | <span data-ttu-id="7544e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7544e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7544e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7544e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7544e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7544e-118">Request headers</span></span>

| <span data-ttu-id="7544e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7544e-119">Name</span></span>       | <span data-ttu-id="7544e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7544e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7544e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7544e-121">Authorization</span></span> | <span data-ttu-id="7544e-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="7544e-122">Bearer {token}.</span></span> <span data-ttu-id="7544e-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7544e-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="7544e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7544e-124">Request body</span></span>

<span data-ttu-id="7544e-125">No corpo da solicitação, fornece os valores para propriedades relevantes que devem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="7544e-125">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="7544e-126">As propriedades existentes que não estão incluídas no corpo da solicitação mantêm os valores anteriores ou recalcula-os com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7544e-126">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="7544e-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7544e-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7544e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7544e-128">Property</span></span>     | <span data-ttu-id="7544e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7544e-129">Type</span></span>        | <span data-ttu-id="7544e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7544e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7544e-131">description</span><span class="sxs-lookup"><span data-stu-id="7544e-131">description</span></span>|<span data-ttu-id="7544e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7544e-132">String</span></span>|<span data-ttu-id="7544e-133">Uma descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="7544e-133">A description for this policy.</span></span>|
|<span data-ttu-id="7544e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7544e-134">displayName</span></span>|<span data-ttu-id="7544e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7544e-135">String</span></span>|<span data-ttu-id="7544e-136">O nome de exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="7544e-136">The display name for this policy.</span></span>|
|<span data-ttu-id="7544e-137">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="7544e-137">isAppliedToOrganization</span></span>|<span data-ttu-id="7544e-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="7544e-138">Boolean</span></span>|<span data-ttu-id="7544e-139">Indica se essa política de lançamento de recursos deve ser aplicada a toda a organização.</span><span class="sxs-lookup"><span data-stu-id="7544e-139">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="7544e-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7544e-140">isEnabled</span></span>|<span data-ttu-id="7544e-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="7544e-141">Boolean</span></span>|<span data-ttu-id="7544e-142">Indica se a adoção de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="7544e-142">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="7544e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7544e-143">Response</span></span>

<span data-ttu-id="7544e-144">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="7544e-144">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7544e-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7544e-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7544e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7544e-146">Request</span></span>

<span data-ttu-id="7544e-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7544e-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7544e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7544e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy_policies"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a
Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="7544e-149">C#</span><span class="sxs-lookup"><span data-stu-id="7544e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7544e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7544e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7544e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7544e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7544e-152">Java</span><span class="sxs-lookup"><span data-stu-id="7544e-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7544e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7544e-153">Response</span></span>

<span data-ttu-id="7544e-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7544e-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
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


