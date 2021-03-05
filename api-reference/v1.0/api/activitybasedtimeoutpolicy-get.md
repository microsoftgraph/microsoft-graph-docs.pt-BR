---
title: Obter activityBasedTimeoutPolicy
description: Obter as propriedades de um objeto activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0830ef84ca3082d5e47deeca9575fd4055d8c358
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442618"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="83c47-103">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="83c47-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="83c47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83c47-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="83c47-105">Obter as propriedades de [um objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83c47-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83c47-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83c47-106">Permissions</span></span>

<span data-ttu-id="83c47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83c47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83c47-109">Permission type</span></span>                        | <span data-ttu-id="83c47-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83c47-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83c47-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83c47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83c47-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="83c47-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="83c47-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83c47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83c47-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83c47-114">Not supported.</span></span> |
| <span data-ttu-id="83c47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83c47-115">Application</span></span>                            | <span data-ttu-id="83c47-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="83c47-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="83c47-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83c47-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83c47-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83c47-118">Optional query parameters</span></span>

<span data-ttu-id="83c47-119">Este método dá suporte aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83c47-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="83c47-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="83c47-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="83c47-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83c47-121">Request headers</span></span>

| <span data-ttu-id="83c47-122">Nome</span><span class="sxs-lookup"><span data-stu-id="83c47-122">Name</span></span>      |<span data-ttu-id="83c47-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="83c47-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83c47-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="83c47-124">Authorization</span></span> | <span data-ttu-id="83c47-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83c47-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83c47-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83c47-127">Request body</span></span>

<span data-ttu-id="83c47-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83c47-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83c47-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="83c47-129">Response</span></span>

<span data-ttu-id="83c47-130">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83c47-130">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83c47-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83c47-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83c47-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83c47-132">Request</span></span>

<span data-ttu-id="83c47-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83c47-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="83c47-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="83c47-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="83c47-135">C#</span><span class="sxs-lookup"><span data-stu-id="83c47-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83c47-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83c47-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83c47-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83c47-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83c47-138">Java</span><span class="sxs-lookup"><span data-stu-id="83c47-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83c47-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="83c47-139">Response</span></span>

<span data-ttu-id="83c47-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83c47-140">The following is an example of the response.</span></span>

> <span data-ttu-id="83c47-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83c47-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

