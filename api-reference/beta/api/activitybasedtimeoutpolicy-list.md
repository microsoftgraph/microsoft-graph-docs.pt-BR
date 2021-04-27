---
title: Listar activityBasedTimeoutPolicies
description: Obter uma lista de objetos activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c81726f5218fdfd3f8e11bf1914b1f9ca7867868
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048327"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="229ab-103">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="229ab-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="229ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="229ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="229ab-105">Obter uma lista de [objetos activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="229ab-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="229ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="229ab-106">Permissions</span></span>

<span data-ttu-id="229ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="229ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="229ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="229ab-109">Permission type</span></span>                        | <span data-ttu-id="229ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="229ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="229ab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="229ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="229ab-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="229ab-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="229ab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="229ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="229ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="229ab-114">Not supported.</span></span> |
| <span data-ttu-id="229ab-115">Application</span><span class="sxs-lookup"><span data-stu-id="229ab-115">Application</span></span>                            | <span data-ttu-id="229ab-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="229ab-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="229ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="229ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="229ab-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="229ab-118">Optional query parameters</span></span>

<span data-ttu-id="229ab-119">Este método dá suporte aos `$filter` parâmetros de consulta , `$select` e `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="229ab-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="229ab-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="229ab-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="229ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="229ab-121">Request headers</span></span>

| <span data-ttu-id="229ab-122">Nome</span><span class="sxs-lookup"><span data-stu-id="229ab-122">Name</span></span>      |<span data-ttu-id="229ab-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="229ab-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="229ab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="229ab-124">Authorization</span></span> | <span data-ttu-id="229ab-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="229ab-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="229ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="229ab-126">Request body</span></span>

<span data-ttu-id="229ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="229ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="229ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="229ab-128">Response</span></span>

<span data-ttu-id="229ab-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="229ab-129">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="229ab-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="229ab-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="229ab-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="229ab-131">Request</span></span>

<span data-ttu-id="229ab-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="229ab-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="229ab-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="229ab-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="229ab-134">C#</span><span class="sxs-lookup"><span data-stu-id="229ab-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="229ab-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="229ab-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="229ab-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="229ab-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="229ab-137">Java</span><span class="sxs-lookup"><span data-stu-id="229ab-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="229ab-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="229ab-138">Response</span></span>

<span data-ttu-id="229ab-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="229ab-139">The following is an example of the response.</span></span>

> <span data-ttu-id="229ab-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="229ab-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


