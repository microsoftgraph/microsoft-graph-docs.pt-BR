---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e os relacionamentos de um objeto featurerolloutpolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aabff4be2ceeffbb687029cce0e5c6e6150e911e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325264"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="60a6d-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="60a6d-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a6d-104">Recupere as propriedades e os relacionamentos de um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="60a6d-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60a6d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="60a6d-105">Permissions</span></span>

<span data-ttu-id="60a6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60a6d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60a6d-108">Permission type</span></span>                        | <span data-ttu-id="60a6d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60a6d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60a6d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60a6d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="60a6d-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a6d-111">Policy.Read.All</span></span> |
| <span data-ttu-id="60a6d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60a6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a6d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a6d-113">Not supported.</span></span> |
| <span data-ttu-id="60a6d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60a6d-114">Application</span></span>                            | <span data-ttu-id="60a6d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60a6d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60a6d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60a6d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60a6d-117">Optional query parameters</span></span>

<span data-ttu-id="60a6d-118">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60a6d-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="60a6d-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60a6d-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60a6d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60a6d-120">Request headers</span></span>

| <span data-ttu-id="60a6d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="60a6d-121">Name</span></span>      |<span data-ttu-id="60a6d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a6d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60a6d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a6d-123">Authorization</span></span> | <span data-ttu-id="60a6d-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="60a6d-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60a6d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60a6d-125">Request body</span></span>

<span data-ttu-id="60a6d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60a6d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60a6d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a6d-127">Response</span></span>

<span data-ttu-id="60a6d-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60a6d-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60a6d-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60a6d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60a6d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60a6d-130">Request</span></span>

<span data-ttu-id="60a6d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60a6d-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60a6d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="60a6d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a6d-133">C#</span><span class="sxs-lookup"><span data-stu-id="60a6d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a6d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a6d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a6d-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="60a6d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60a6d-136">Java</span><span class="sxs-lookup"><span data-stu-id="60a6d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60a6d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a6d-137">Response</span></span>

<span data-ttu-id="60a6d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60a6d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="60a6d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60a6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="request"></a><span data-ttu-id="60a6d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60a6d-141">Request</span></span>

<span data-ttu-id="60a6d-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60a6d-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60a6d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="60a6d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a6d-144">C#</span><span class="sxs-lookup"><span data-stu-id="60a6d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a6d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a6d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a6d-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="60a6d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60a6d-147">Java</span><span class="sxs-lookup"><span data-stu-id="60a6d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60a6d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a6d-148">Response</span></span>

<span data-ttu-id="60a6d-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60a6d-149">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="60a6d-150">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="60a6d-150">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60a6d-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60a6d-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
