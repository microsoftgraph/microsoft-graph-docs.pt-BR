---
title: Token de listaIssuancePolicy
description: Obter uma lista de objetos tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 693579c25c7e96ccbdfceecee44791ba23ffeefa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054340"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="2ba6c-103">Token de listaIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="2ba6c-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="2ba6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba6c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="2ba6c-105">Obter uma lista de [objetos tokenIssuancePolicy.](../resources/tokenIssuancePolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ba6c-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ba6c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ba6c-106">Permissions</span></span>

<span data-ttu-id="2ba6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ba6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ba6c-109">Permission type</span></span>                        | <span data-ttu-id="2ba6c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ba6c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ba6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ba6c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ba6c-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ba6c-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="2ba6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ba6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ba6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-114">Not supported.</span></span> |
| <span data-ttu-id="2ba6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ba6c-115">Application</span></span>                            | <span data-ttu-id="2ba6c-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ba6c-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ba6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ba6c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ba6c-118">Optional query parameters</span></span>

<span data-ttu-id="2ba6c-119">Este método dá suporte `$expand` aos `$filter` parâmetros de consulta , , e OData para ajudar a `$select` personalizar a `$top` resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ba6c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ba6c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="2ba6c-121">Ao usar `$expand` , certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ba6c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba6c-122">Request headers</span></span>

| <span data-ttu-id="2ba6c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2ba6c-123">Name</span></span>      |<span data-ttu-id="2ba6c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba6c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ba6c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ba6c-125">Authorization</span></span> | <span data-ttu-id="2ba6c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ba6c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba6c-128">Request body</span></span>

<span data-ttu-id="2ba6c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ba6c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba6c-130">Response</span></span>

<span data-ttu-id="2ba6c-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ba6c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ba6c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ba6c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ba6c-133">Request</span></span>

<span data-ttu-id="2ba6c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ba6c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba6c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="2ba6c-136">C#</span><span class="sxs-lookup"><span data-stu-id="2ba6c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ba6c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ba6c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ba6c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ba6c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ba6c-139">Java</span><span class="sxs-lookup"><span data-stu-id="2ba6c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tokenissuancepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ba6c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ba6c-140">Response</span></span>

<span data-ttu-id="2ba6c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-141">The following is an example of the response.</span></span>

> <span data-ttu-id="2ba6c-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ba6c-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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

