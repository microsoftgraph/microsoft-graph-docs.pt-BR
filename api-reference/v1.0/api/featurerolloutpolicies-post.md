---
title: Criar featureRolloutPolicy
description: Crie um novo objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bbd11d73cf8453eac184708324b1001144c1a36c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201572"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="2fe0b-103">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="2fe0b-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="2fe0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fe0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2fe0b-105">Crie um novo [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fe0b-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fe0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fe0b-106">Permissions</span></span>

<span data-ttu-id="2fe0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fe0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fe0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fe0b-109">Permission type</span></span>                        | <span data-ttu-id="2fe0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fe0b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2fe0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fe0b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fe0b-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fe0b-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="2fe0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fe0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fe0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-114">Not supported.</span></span> |
| <span data-ttu-id="2fe0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fe0b-115">Application</span></span>                            | <span data-ttu-id="2fe0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fe0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fe0b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2fe0b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fe0b-118">Request headers</span></span>

| <span data-ttu-id="2fe0b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2fe0b-119">Name</span></span>          | <span data-ttu-id="2fe0b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fe0b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2fe0b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fe0b-121">Authorization</span></span> | <span data-ttu-id="2fe0b-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-122">Bearer {token}.</span></span> <span data-ttu-id="2fe0b-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="2fe0b-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fe0b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fe0b-124">Request body</span></span>

<span data-ttu-id="2fe0b-125">No corpo da solicitação, fornece uma representação JSON do [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fe0b-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="2fe0b-126">A tabela a seguir mostra as propriedades que são necessárias ao criar [um featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2fe0b-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="2fe0b-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2fe0b-127">Parameter</span></span> | <span data-ttu-id="2fe0b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fe0b-128">Type</span></span> | <span data-ttu-id="2fe0b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fe0b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fe0b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2fe0b-130">displayName</span></span> |<span data-ttu-id="2fe0b-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fe0b-131">string</span></span> |<span data-ttu-id="2fe0b-132">O nome de exibição dessa política de lançamento de recursos.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="2fe0b-133">feature</span><span class="sxs-lookup"><span data-stu-id="2fe0b-133">feature</span></span> |<span data-ttu-id="2fe0b-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="2fe0b-134">stagedFeatureName</span></span> |<span data-ttu-id="2fe0b-135">O recurso que seria lançado usando essa política.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="2fe0b-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2fe0b-136">isEnabled</span></span> |<span data-ttu-id="2fe0b-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fe0b-137">string</span></span> |<span data-ttu-id="2fe0b-138">Indica se a adoção de recursos está habilitada.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="2fe0b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fe0b-139">Response</span></span>

<span data-ttu-id="2fe0b-140">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2fe0b-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2fe0b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2fe0b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fe0b-142">Request</span></span>

<span data-ttu-id="2fe0b-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2fe0b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fe0b-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2fe0b-145">C#</span><span class="sxs-lookup"><span data-stu-id="2fe0b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fe0b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fe0b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fe0b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fe0b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fe0b-148">Java</span><span class="sxs-lookup"><span data-stu-id="2fe0b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2fe0b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fe0b-149">Response</span></span>

<span data-ttu-id="2fe0b-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-150">The following is an example of the response.</span></span>

> <span data-ttu-id="2fe0b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fe0b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


