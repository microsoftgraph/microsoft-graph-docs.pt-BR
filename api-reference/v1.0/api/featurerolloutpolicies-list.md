---
title: Listar featureRolloutPolicies
description: Recupere uma lista de objetos featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9e3c3a3b8e9f8914c29701eac9e6b48e26d4f283
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054018"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="f2bf7-103">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="f2bf7-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="f2bf7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2bf7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2bf7-105">Recupere uma lista de [objetos featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f2bf7-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2bf7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2bf7-106">Permissions</span></span>

<span data-ttu-id="f2bf7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2bf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2bf7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2bf7-109">Permission type</span></span>                        | <span data-ttu-id="f2bf7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2bf7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2bf7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2bf7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2bf7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2bf7-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="f2bf7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2bf7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2bf7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-114">Not supported.</span></span> |
| <span data-ttu-id="f2bf7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2bf7-115">Application</span></span>                            | <span data-ttu-id="f2bf7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2bf7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2bf7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2bf7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2bf7-118">Optional query parameters</span></span>

<span data-ttu-id="f2bf7-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta: `$count` , , , , , , `$expand` `$filter` `$orderby` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f2bf7-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="f2bf7-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2bf7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2bf7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2bf7-121">Request headers</span></span>

| <span data-ttu-id="f2bf7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f2bf7-122">Name</span></span>      |<span data-ttu-id="f2bf7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2bf7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2bf7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2bf7-124">Authorization</span></span> | <span data-ttu-id="f2bf7-125">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-125">Bearer {token}.</span></span> <span data-ttu-id="f2bf7-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f2bf7-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2bf7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2bf7-127">Request body</span></span>

<span data-ttu-id="f2bf7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2bf7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2bf7-129">Response</span></span>

<span data-ttu-id="f2bf7-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-130">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2bf7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2bf7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2bf7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2bf7-132">Request</span></span>

<span data-ttu-id="f2bf7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2bf7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2bf7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="f2bf7-135">C#</span><span class="sxs-lookup"><span data-stu-id="f2bf7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2bf7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2bf7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2bf7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2bf7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2bf7-138">Java</span><span class="sxs-lookup"><span data-stu-id="f2bf7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2bf7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2bf7-139">Response</span></span>

<span data-ttu-id="f2bf7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f2bf7-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f2bf7-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


