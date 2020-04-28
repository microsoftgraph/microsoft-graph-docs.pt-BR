---
title: Listar activityBasedTimeoutPolicies
description: Obtenha uma lista de objetos activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9d8b8968ffcabdcc2ff67a280dafe06bdbd0f541
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917087"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="3e740-103">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="3e740-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="3e740-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e740-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="3e740-105">Obtenha uma lista de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3e740-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e740-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e740-106">Permissions</span></span>

<span data-ttu-id="3e740-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e740-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e740-109">Permission type</span></span>                        | <span data-ttu-id="3e740-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e740-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e740-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e740-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e740-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e740-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="3e740-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e740-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e740-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e740-114">Not supported.</span></span> |
| <span data-ttu-id="3e740-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e740-115">Application</span></span>                            | <span data-ttu-id="3e740-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e740-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e740-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e740-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e740-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e740-118">Optional query parameters</span></span>

<span data-ttu-id="3e740-119">Este método oferece suporte `$filter`ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e740-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="3e740-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3e740-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e740-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e740-121">Request headers</span></span>

| <span data-ttu-id="3e740-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3e740-122">Name</span></span>      |<span data-ttu-id="3e740-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e740-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e740-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e740-124">Authorization</span></span> | <span data-ttu-id="3e740-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e740-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e740-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e740-127">Request body</span></span>

<span data-ttu-id="3e740-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e740-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e740-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e740-129">Response</span></span>

<span data-ttu-id="3e740-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e740-130">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e740-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e740-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e740-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e740-132">Request</span></span>

<span data-ttu-id="3e740-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e740-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3e740-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e740-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="3e740-135">C#</span><span class="sxs-lookup"><span data-stu-id="3e740-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e740-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e740-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e740-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e740-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e740-138">Java</span><span class="sxs-lookup"><span data-stu-id="3e740-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e740-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e740-139">Response</span></span>

<span data-ttu-id="3e740-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e740-140">The following is an example of the response.</span></span>

> <span data-ttu-id="3e740-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e740-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
