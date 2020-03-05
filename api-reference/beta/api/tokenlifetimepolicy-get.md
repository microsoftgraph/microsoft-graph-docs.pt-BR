---
title: Obter tokenLifetimePolicy
description: Recupere as propriedades e os relacionamentos do objeto tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0bbd72ebddb221bc7bc82e1676180048e57d9994
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452222"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="a9b21-103">Obter tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a9b21-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="a9b21-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9b21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9b21-105">Recupere as propriedades e os relacionamentos de um objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a9b21-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9b21-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9b21-106">Permissions</span></span>

<span data-ttu-id="a9b21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9b21-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9b21-109">Permission type</span></span>                        | <span data-ttu-id="a9b21-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9b21-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9b21-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9b21-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9b21-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9b21-112">Policy.Read.All</span></span> |
| <span data-ttu-id="a9b21-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9b21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9b21-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9b21-114">Not supported.</span></span> |
| <span data-ttu-id="a9b21-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9b21-115">Application</span></span>                            | <span data-ttu-id="a9b21-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9b21-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9b21-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b21-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9b21-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9b21-118">Optional query parameters</span></span>

<span data-ttu-id="a9b21-119">Este método oferece suporte `$expand` aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b21-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a9b21-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9b21-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="a9b21-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="a9b21-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9b21-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b21-122">Request headers</span></span>

| <span data-ttu-id="a9b21-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a9b21-123">Name</span></span>      |<span data-ttu-id="a9b21-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9b21-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9b21-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9b21-125">Authorization</span></span> | <span data-ttu-id="a9b21-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a9b21-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9b21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b21-127">Request body</span></span>

<span data-ttu-id="a9b21-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9b21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9b21-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b21-129">Response</span></span>

<span data-ttu-id="a9b21-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b21-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9b21-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9b21-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9b21-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b21-132">Request</span></span>

<span data-ttu-id="a9b21-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9b21-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9b21-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b21-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="a9b21-135">C#</span><span class="sxs-lookup"><span data-stu-id="a9b21-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9b21-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9b21-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9b21-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9b21-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9b21-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b21-138">Response</span></span>

<span data-ttu-id="a9b21-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b21-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a9b21-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9b21-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
