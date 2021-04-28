---
title: Criar featureRolloutPolicy
description: Crie um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5d1d55faa62ea070287692298c568b0db48f8d15
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052387"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="a8906-103">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="a8906-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="a8906-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8906-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8906-105">Crie um novo [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a8906-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8906-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8906-106">Permissions</span></span>

<span data-ttu-id="a8906-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8906-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8906-109">Permission type</span></span>                        | <span data-ttu-id="a8906-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8906-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8906-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8906-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8906-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8906-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="a8906-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8906-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8906-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8906-114">Not supported.</span></span> |
| <span data-ttu-id="a8906-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8906-115">Application</span></span>                            | <span data-ttu-id="a8906-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8906-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8906-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8906-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a8906-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8906-118">Request headers</span></span>

| <span data-ttu-id="a8906-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a8906-119">Name</span></span>          | <span data-ttu-id="a8906-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8906-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a8906-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8906-121">Authorization</span></span> | <span data-ttu-id="a8906-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="a8906-122">Bearer {token}.</span></span> <span data-ttu-id="a8906-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a8906-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8906-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8906-124">Request body</span></span>

<span data-ttu-id="a8906-125">No corpo da solicitação, fornece uma representação JSON do [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a8906-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="a8906-126">A tabela a seguir mostra as propriedades que são necessárias ao criar [um featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a8906-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="a8906-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a8906-127">Parameter</span></span> | <span data-ttu-id="a8906-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8906-128">Type</span></span> | <span data-ttu-id="a8906-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8906-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8906-130">displayName</span><span class="sxs-lookup"><span data-stu-id="a8906-130">displayName</span></span> |<span data-ttu-id="a8906-131">string</span><span class="sxs-lookup"><span data-stu-id="a8906-131">string</span></span> |<span data-ttu-id="a8906-132">O nome de exibição dessa política de lançamento de recursos.</span><span class="sxs-lookup"><span data-stu-id="a8906-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="a8906-133">feature</span><span class="sxs-lookup"><span data-stu-id="a8906-133">feature</span></span> |<span data-ttu-id="a8906-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="a8906-134">stagedFeatureName</span></span> |<span data-ttu-id="a8906-135">O recurso que seria lançado usando essa política.</span><span class="sxs-lookup"><span data-stu-id="a8906-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="a8906-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a8906-136">isEnabled</span></span> |<span data-ttu-id="a8906-137">string</span><span class="sxs-lookup"><span data-stu-id="a8906-137">string</span></span> |<span data-ttu-id="a8906-138">Indica se a adoção de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="a8906-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="a8906-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8906-139">Response</span></span>

<span data-ttu-id="a8906-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8906-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8906-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8906-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8906-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8906-142">Request</span></span>

<span data-ttu-id="a8906-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8906-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8906-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8906-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a8906-145">C#</span><span class="sxs-lookup"><span data-stu-id="a8906-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8906-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8906-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8906-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8906-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8906-148">Java</span><span class="sxs-lookup"><span data-stu-id="a8906-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8906-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8906-149">Response</span></span>

<span data-ttu-id="a8906-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8906-150">The following is an example of the response.</span></span>

> <span data-ttu-id="a8906-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8906-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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


