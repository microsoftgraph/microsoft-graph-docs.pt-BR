---
title: Obter activityBasedTimeoutPolicy
description: Obter as propriedades de um objeto activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a74fb8c530a4faaab95c29c7f4ab0ae654bf30c9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048334"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="86c2f-103">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="86c2f-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="86c2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86c2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c2f-105">Obter as propriedades de [um objeto activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86c2f-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86c2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86c2f-106">Permissions</span></span>

<span data-ttu-id="86c2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86c2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86c2f-109">Permission type</span></span>                        | <span data-ttu-id="86c2f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86c2f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86c2f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86c2f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86c2f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="86c2f-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="86c2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86c2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c2f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86c2f-114">Not supported.</span></span> |
| <span data-ttu-id="86c2f-115">Application</span><span class="sxs-lookup"><span data-stu-id="86c2f-115">Application</span></span>                            | <span data-ttu-id="86c2f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="86c2f-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="86c2f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86c2f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86c2f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86c2f-118">Optional query parameters</span></span>

<span data-ttu-id="86c2f-119">Este método dá suporte aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86c2f-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="86c2f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="86c2f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="86c2f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86c2f-121">Request headers</span></span>

| <span data-ttu-id="86c2f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="86c2f-122">Name</span></span>      |<span data-ttu-id="86c2f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="86c2f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86c2f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="86c2f-124">Authorization</span></span> | <span data-ttu-id="86c2f-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="86c2f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86c2f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86c2f-126">Request body</span></span>

<span data-ttu-id="86c2f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86c2f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86c2f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c2f-128">Response</span></span>

<span data-ttu-id="86c2f-129">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86c2f-129">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86c2f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="86c2f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86c2f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86c2f-131">Request</span></span>

<span data-ttu-id="86c2f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86c2f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86c2f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="86c2f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="86c2f-134">C#</span><span class="sxs-lookup"><span data-stu-id="86c2f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86c2f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86c2f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86c2f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86c2f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86c2f-137">Java</span><span class="sxs-lookup"><span data-stu-id="86c2f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86c2f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="86c2f-138">Response</span></span>

<span data-ttu-id="86c2f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86c2f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="86c2f-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86c2f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


