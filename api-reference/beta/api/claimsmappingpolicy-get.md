---
title: Obter claimsMappingPolicy
description: Recupere as propriedades e as relações do objeto claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5cc63184b5486614f2b8b73c4e3f176eb4dbd110
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047277"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="1c401-103">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1c401-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="1c401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c401-105">Recupere as propriedades e as relações de um [objeto claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1c401-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c401-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c401-106">Permissions</span></span>

<span data-ttu-id="1c401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c401-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c401-109">Permission type</span></span>                        | <span data-ttu-id="1c401-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c401-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c401-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c401-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c401-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c401-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1c401-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c401-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c401-114">Not supported.</span></span> |
| <span data-ttu-id="1c401-115">Application</span><span class="sxs-lookup"><span data-stu-id="1c401-115">Application</span></span>                            | <span data-ttu-id="1c401-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c401-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c401-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c401-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c401-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c401-118">Optional query parameters</span></span>

<span data-ttu-id="1c401-119">Este método dá suporte aos `$expand` `$select` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c401-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1c401-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1c401-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="1c401-121">Ao `$expand` usar, certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="1c401-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c401-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c401-122">Request headers</span></span>

| <span data-ttu-id="1c401-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1c401-123">Name</span></span>      |<span data-ttu-id="1c401-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c401-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c401-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c401-125">Authorization</span></span> | <span data-ttu-id="1c401-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1c401-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c401-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c401-127">Request body</span></span>

<span data-ttu-id="1c401-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c401-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c401-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c401-129">Response</span></span>

<span data-ttu-id="1c401-130">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c401-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c401-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c401-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c401-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c401-132">Request</span></span>

<span data-ttu-id="1c401-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c401-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c401-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c401-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="1c401-135">C#</span><span class="sxs-lookup"><span data-stu-id="1c401-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c401-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c401-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c401-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c401-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c401-138">Java</span><span class="sxs-lookup"><span data-stu-id="1c401-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c401-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c401-139">Response</span></span>

<span data-ttu-id="1c401-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c401-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1c401-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c401-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Get claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


