---
title: Listar featureRolloutPolicies
description: Recupere uma lista de objetos featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6324c4bc324015b573789e415e46d0a4d784a264
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472507"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="3e0be-103">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="3e0be-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="3e0be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e0be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e0be-105">Recupere uma lista de [objetos featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e0be-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e0be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e0be-106">Permissions</span></span>

<span data-ttu-id="3e0be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e0be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e0be-109">Permission type</span></span>                        | <span data-ttu-id="3e0be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e0be-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e0be-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e0be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e0be-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e0be-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3e0be-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e0be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e0be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e0be-114">Not supported.</span></span> |
| <span data-ttu-id="3e0be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e0be-115">Application</span></span>                            | <span data-ttu-id="3e0be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e0be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e0be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e0be-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e0be-118">Optional query parameters</span></span>

<span data-ttu-id="3e0be-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta: `$count` , , , , , , `$expand` `$filter` `$orderby` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="3e0be-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="3e0be-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3e0be-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e0be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0be-121">Request headers</span></span>

| <span data-ttu-id="3e0be-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3e0be-122">Name</span></span>      |<span data-ttu-id="3e0be-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e0be-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e0be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e0be-124">Authorization</span></span> | <span data-ttu-id="3e0be-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3e0be-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e0be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0be-126">Request body</span></span>

<span data-ttu-id="3e0be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e0be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e0be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0be-128">Response</span></span>

<span data-ttu-id="3e0be-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-129">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e0be-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e0be-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e0be-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0be-131">Request</span></span>

<span data-ttu-id="3e0be-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e0be-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e0be-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0be-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="3e0be-134">C#</span><span class="sxs-lookup"><span data-stu-id="3e0be-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e0be-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e0be-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e0be-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e0be-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e0be-137">Java</span><span class="sxs-lookup"><span data-stu-id="3e0be-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e0be-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0be-138">Response</span></span>

<span data-ttu-id="3e0be-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0be-139">The following is an example of the response.</span></span>

> <span data-ttu-id="3e0be-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e0be-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


