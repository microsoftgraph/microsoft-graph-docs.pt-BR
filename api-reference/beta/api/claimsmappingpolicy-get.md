---
title: Obter claimsMappingPolicy
description: Recupere as propriedades e os relacionamentos do objeto claimsMappingPolicy.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8423830753a6b8c19334d53b210b1874d09256e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217978"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="a93d2-103">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="a93d2-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="a93d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a93d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a93d2-105">Recupere as propriedades e os relacionamentos de um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a93d2-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a93d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a93d2-106">Permissions</span></span>

<span data-ttu-id="a93d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a93d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a93d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a93d2-109">Permission type</span></span>                        | <span data-ttu-id="a93d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a93d2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a93d2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a93d2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a93d2-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a93d2-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a93d2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a93d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a93d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a93d2-114">Not supported.</span></span> |
| <span data-ttu-id="a93d2-115">Application</span><span class="sxs-lookup"><span data-stu-id="a93d2-115">Application</span></span>                            | <span data-ttu-id="a93d2-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a93d2-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a93d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a93d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a93d2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a93d2-118">Optional query parameters</span></span>

<span data-ttu-id="a93d2-119">Este método oferece suporte `$expand` aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a93d2-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a93d2-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a93d2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="a93d2-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="a93d2-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a93d2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a93d2-122">Request headers</span></span>

| <span data-ttu-id="a93d2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a93d2-123">Name</span></span>      |<span data-ttu-id="a93d2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a93d2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a93d2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a93d2-125">Authorization</span></span> | <span data-ttu-id="a93d2-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a93d2-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a93d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a93d2-127">Request body</span></span>

<span data-ttu-id="a93d2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a93d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a93d2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a93d2-129">Response</span></span>

<span data-ttu-id="a93d2-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a93d2-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a93d2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a93d2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a93d2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a93d2-132">Request</span></span>

<span data-ttu-id="a93d2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a93d2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a93d2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a93d2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="a93d2-135">C#</span><span class="sxs-lookup"><span data-stu-id="a93d2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a93d2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a93d2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a93d2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a93d2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a93d2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a93d2-138">Response</span></span>

<span data-ttu-id="a93d2-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a93d2-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a93d2-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a93d2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
