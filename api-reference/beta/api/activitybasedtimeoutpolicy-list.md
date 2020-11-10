---
title: Listar activityBasedTimeoutPolicies
description: Obtenha uma lista de objetos activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb717e8e499f321c48cd1a8f9626d5dd4017d684
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952511"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="f67cc-103">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="f67cc-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="f67cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f67cc-105">Obtenha uma lista de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f67cc-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f67cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f67cc-106">Permissions</span></span>

<span data-ttu-id="f67cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f67cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f67cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f67cc-109">Permission type</span></span>                        | <span data-ttu-id="f67cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f67cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f67cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f67cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f67cc-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f67cc-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f67cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f67cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f67cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f67cc-114">Not supported.</span></span> |
| <span data-ttu-id="f67cc-115">Application</span><span class="sxs-lookup"><span data-stu-id="f67cc-115">Application</span></span>                            | <span data-ttu-id="f67cc-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f67cc-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f67cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f67cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f67cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f67cc-118">Optional query parameters</span></span>

<span data-ttu-id="f67cc-119">Este método oferece suporte `$filter` ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f67cc-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f67cc-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f67cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f67cc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f67cc-121">Request headers</span></span>

| <span data-ttu-id="f67cc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f67cc-122">Name</span></span>      |<span data-ttu-id="f67cc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67cc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f67cc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f67cc-124">Authorization</span></span> | <span data-ttu-id="f67cc-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f67cc-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f67cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f67cc-126">Request body</span></span>

<span data-ttu-id="f67cc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f67cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f67cc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67cc-128">Response</span></span>

<span data-ttu-id="f67cc-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f67cc-129">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f67cc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f67cc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f67cc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f67cc-131">Request</span></span>

<span data-ttu-id="f67cc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f67cc-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f67cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f67cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="f67cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="f67cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f67cc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f67cc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f67cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f67cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f67cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="f67cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f67cc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f67cc-138">Response</span></span>

<span data-ttu-id="f67cc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f67cc-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f67cc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f67cc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
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
  "description": "List activityBasedTimeoutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


