---
title: Listar tokenLifetimePolicies
description: Obtenha uma lista de objetos tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12ccf89d8110c8449bac5e23259fe902e667cd4b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916303"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="6ba89-103">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="6ba89-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="6ba89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ba89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ba89-105">Obtenha uma lista de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6ba89-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ba89-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ba89-106">Permissions</span></span>

<span data-ttu-id="6ba89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ba89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ba89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ba89-109">Permission type</span></span>                        | <span data-ttu-id="6ba89-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ba89-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6ba89-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ba89-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ba89-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ba89-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6ba89-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ba89-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ba89-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ba89-114">Not supported.</span></span> |
| <span data-ttu-id="6ba89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ba89-115">Application</span></span>                            | <span data-ttu-id="6ba89-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ba89-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ba89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ba89-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ba89-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ba89-118">Optional query parameters</span></span>

<span data-ttu-id="6ba89-119">Este método oferece suporte `$expand`a `$filter`, `$select` e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba89-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="6ba89-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6ba89-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="6ba89-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="6ba89-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ba89-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba89-122">Request headers</span></span>

| <span data-ttu-id="6ba89-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6ba89-123">Name</span></span>      |<span data-ttu-id="6ba89-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ba89-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ba89-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ba89-125">Authorization</span></span> | <span data-ttu-id="6ba89-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6ba89-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ba89-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba89-127">Request body</span></span>

<span data-ttu-id="6ba89-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ba89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ba89-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ba89-129">Response</span></span>

<span data-ttu-id="6ba89-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba89-130">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ba89-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6ba89-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ba89-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba89-132">Request</span></span>

<span data-ttu-id="6ba89-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ba89-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ba89-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ba89-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="6ba89-135">C#</span><span class="sxs-lookup"><span data-stu-id="6ba89-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ba89-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ba89-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ba89-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ba89-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ba89-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ba89-138">Response</span></span>

<span data-ttu-id="6ba89-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba89-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6ba89-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ba89-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
