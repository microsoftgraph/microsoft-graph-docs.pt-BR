---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e as relações de um objeto featurerolloutpolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d7f73b5c584f5862d272807876d6cd0d76ecc0ea
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471217"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="d1107-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1107-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="d1107-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1107-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1107-105">Recupere as propriedades e as relações de um [objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d1107-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1107-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1107-106">Permissions</span></span>

<span data-ttu-id="d1107-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1107-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1107-109">Permission type</span></span>                        | <span data-ttu-id="d1107-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1107-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1107-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1107-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1107-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1107-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="d1107-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1107-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1107-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1107-114">Not supported.</span></span> |
| <span data-ttu-id="d1107-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1107-115">Application</span></span>                            | <span data-ttu-id="d1107-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1107-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1107-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1107-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1107-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1107-118">Optional query parameters</span></span>

<span data-ttu-id="d1107-119">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1107-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="d1107-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d1107-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1107-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1107-121">Request headers</span></span>

| <span data-ttu-id="d1107-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d1107-122">Name</span></span>      |<span data-ttu-id="d1107-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1107-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1107-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1107-124">Authorization</span></span> | <span data-ttu-id="d1107-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d1107-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1107-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1107-126">Request body</span></span>

<span data-ttu-id="d1107-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1107-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1107-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1107-128">Response</span></span>

<span data-ttu-id="d1107-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1107-129">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1107-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1107-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1107-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1107-131">Request</span></span>

<span data-ttu-id="d1107-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1107-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1107-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1107-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="d1107-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1107-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1107-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1107-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1107-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1107-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1107-137">Java</span><span class="sxs-lookup"><span data-stu-id="d1107-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1107-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1107-138">Response</span></span>

<span data-ttu-id="d1107-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1107-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d1107-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1107-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="d1107-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1107-142">Request</span></span>

<span data-ttu-id="d1107-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1107-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1107-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1107-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="d1107-145">C#</span><span class="sxs-lookup"><span data-stu-id="d1107-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1107-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1107-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1107-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1107-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1107-148">Java</span><span class="sxs-lookup"><span data-stu-id="d1107-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1107-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1107-149">Response</span></span>

<span data-ttu-id="d1107-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1107-150">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d1107-151">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="d1107-151">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d1107-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1107-152">All the properties will be returned from an actual call.</span></span>

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


