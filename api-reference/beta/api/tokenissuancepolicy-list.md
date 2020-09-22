---
title: Listar tokenIssuancePolicy
description: Obtenha uma lista de objetos tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 70b0e7875a2634f6f06cea2de9bc2bf0a10ab348
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074010"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="1343b-103">Listar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="1343b-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="1343b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1343b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1343b-105">Obtenha uma lista de objetos [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1343b-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1343b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1343b-106">Permissions</span></span>

<span data-ttu-id="1343b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1343b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1343b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1343b-109">Permission type</span></span>                        | <span data-ttu-id="1343b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1343b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1343b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1343b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1343b-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1343b-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1343b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1343b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1343b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1343b-114">Not supported.</span></span> |
| <span data-ttu-id="1343b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1343b-115">Application</span></span>                            | <span data-ttu-id="1343b-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1343b-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1343b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1343b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1343b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1343b-118">Optional query parameters</span></span>

<span data-ttu-id="1343b-119">Este método oferece suporte `$expand` aos `$filter` parâmetros de `$select` consulta OData,, e `$top` OData, para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1343b-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1343b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1343b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="1343b-121">Ao usar o `$expand` , certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="1343b-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1343b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1343b-122">Request headers</span></span>

| <span data-ttu-id="1343b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1343b-123">Name</span></span>      |<span data-ttu-id="1343b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1343b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1343b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1343b-125">Authorization</span></span> | <span data-ttu-id="1343b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1343b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1343b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1343b-128">Request body</span></span>

<span data-ttu-id="1343b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1343b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1343b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1343b-130">Response</span></span>

<span data-ttu-id="1343b-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1343b-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1343b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1343b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1343b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1343b-133">Request</span></span>

<span data-ttu-id="1343b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1343b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1343b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1343b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="1343b-136">C#</span><span class="sxs-lookup"><span data-stu-id="1343b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1343b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1343b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1343b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1343b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="1343b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1343b-139">Response</span></span>

<span data-ttu-id="1343b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1343b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1343b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1343b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


