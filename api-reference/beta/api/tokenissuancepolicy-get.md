---
title: Obter tokenIssuancePolicy
description: Recupere as propriedades e as relações do objeto tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f4a7025ea69e9224d04efc81f86c038eb20a3465
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433758"
---
# <a name="get-tokenissuancepolicy"></a><span data-ttu-id="61cda-103">Obter tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="61cda-103">Get tokenIssuancePolicy</span></span>

<span data-ttu-id="61cda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61cda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61cda-105">Recupere as propriedades e as relações de um [objeto tokenIssuancePolicy.](../resources/tokenIssuancePolicy.md)</span><span class="sxs-lookup"><span data-stu-id="61cda-105">Retrieve the properties and relationships of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="61cda-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61cda-106">Permissions</span></span>

<span data-ttu-id="61cda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61cda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61cda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61cda-109">Permission type</span></span>                        | <span data-ttu-id="61cda-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61cda-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61cda-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61cda-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="61cda-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="61cda-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="61cda-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61cda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61cda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61cda-114">Not supported.</span></span> |
| <span data-ttu-id="61cda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61cda-115">Application</span></span>                            | <span data-ttu-id="61cda-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="61cda-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="61cda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61cda-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61cda-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61cda-118">Optional query parameters</span></span>

<span data-ttu-id="61cda-119">Este método dá suporte aos `$expand` `$select` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61cda-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="61cda-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="61cda-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="61cda-121">Ao usar `$expand` , certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="61cda-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61cda-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61cda-122">Request headers</span></span>

| <span data-ttu-id="61cda-123">Nome</span><span class="sxs-lookup"><span data-stu-id="61cda-123">Name</span></span>      |<span data-ttu-id="61cda-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cda-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61cda-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="61cda-125">Authorization</span></span> | <span data-ttu-id="61cda-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61cda-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61cda-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61cda-128">Request body</span></span>

<span data-ttu-id="61cda-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61cda-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61cda-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cda-130">Response</span></span>

<span data-ttu-id="61cda-131">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61cda-131">If successful, this method returns a `200 OK` response code and the requested [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61cda-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61cda-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61cda-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cda-133">Request</span></span>

<span data-ttu-id="61cda-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61cda-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61cda-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="61cda-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenIssuancePolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="61cda-136">C#</span><span class="sxs-lookup"><span data-stu-id="61cda-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61cda-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61cda-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61cda-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61cda-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61cda-139">Java</span><span class="sxs-lookup"><span data-stu-id="61cda-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="61cda-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cda-140">Response</span></span>

<span data-ttu-id="61cda-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61cda-141">The following is an example of the response.</span></span>

> <span data-ttu-id="61cda-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61cda-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


