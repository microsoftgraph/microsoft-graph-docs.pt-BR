---
title: Listar activityBasedTimeoutPolicies
description: Obtenha uma lista de objetos activityBasedTimeoutPolicy.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81ea78bab6a1725711696aefb9d0a46656248212
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217943"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="79598-103">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="79598-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="79598-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79598-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79598-105">Obtenha uma lista de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="79598-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="79598-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79598-106">Permissions</span></span>

<span data-ttu-id="79598-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79598-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79598-109">Permission type</span></span>                        | <span data-ttu-id="79598-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79598-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79598-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79598-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79598-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="79598-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="79598-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79598-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79598-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79598-114">Not supported.</span></span> |
| <span data-ttu-id="79598-115">Application</span><span class="sxs-lookup"><span data-stu-id="79598-115">Application</span></span>                            | <span data-ttu-id="79598-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="79598-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="79598-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79598-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79598-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79598-118">Optional query parameters</span></span>

<span data-ttu-id="79598-119">Este método oferece suporte `$filter`ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79598-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="79598-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="79598-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79598-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79598-121">Request headers</span></span>

| <span data-ttu-id="79598-122">Nome</span><span class="sxs-lookup"><span data-stu-id="79598-122">Name</span></span>      |<span data-ttu-id="79598-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="79598-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79598-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="79598-124">Authorization</span></span> | <span data-ttu-id="79598-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="79598-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="79598-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79598-126">Request body</span></span>

<span data-ttu-id="79598-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79598-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79598-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79598-128">Response</span></span>

<span data-ttu-id="79598-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79598-129">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79598-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79598-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79598-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79598-131">Request</span></span>

<span data-ttu-id="79598-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79598-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79598-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="79598-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="79598-134">C#</span><span class="sxs-lookup"><span data-stu-id="79598-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79598-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79598-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79598-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79598-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79598-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="79598-137">Response</span></span>

<span data-ttu-id="79598-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79598-138">The following is an example of the response.</span></span>

> <span data-ttu-id="79598-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79598-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
