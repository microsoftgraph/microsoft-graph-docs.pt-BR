---
title: Listar appConsentRequests
description: Recupere objetos appConsentRequest e suas propriedades.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 44920e65285701f365a7d1a2b465900816bd5012
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201145"
---
# <a name="list-appconsentrequests"></a><span data-ttu-id="e44c2-103">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="e44c2-103">List appConsentRequests</span></span>
<span data-ttu-id="e44c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e44c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e44c2-105">Recupere [objetos appConsentRequest](../resources/appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e44c2-105">Retrieve [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e44c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e44c2-106">Permissions</span></span>
<span data-ttu-id="e44c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e44c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e44c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e44c2-109">Permission type</span></span>|<span data-ttu-id="e44c2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e44c2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44c2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e44c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e44c2-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e44c2-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="e44c2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e44c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44c2-114">Not supported.</span></span>|
|<span data-ttu-id="e44c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e44c2-115">Application</span></span>|<span data-ttu-id="e44c2-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e44c2-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e44c2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e44c2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e44c2-118">Optional query parameters</span></span>
<span data-ttu-id="e44c2-119">Este método dá suporte aos parâmetros de consulta , , , e OData para  `$select` ajudar a personalizar a `$skip` `$top` `$filter` `$orderby` resposta.</span><span class="sxs-lookup"><span data-stu-id="e44c2-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="e44c2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e44c2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e44c2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e44c2-121">Request headers</span></span>
|<span data-ttu-id="e44c2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e44c2-122">Name</span></span>|<span data-ttu-id="e44c2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e44c2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e44c2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e44c2-124">Authorization</span></span>|<span data-ttu-id="e44c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e44c2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e44c2-127">Request body</span></span>
<span data-ttu-id="e44c2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e44c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e44c2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44c2-129">Response</span></span>

<span data-ttu-id="e44c2-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e44c2-130">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="example-1-list-all-appconsentrequests"></a><span data-ttu-id="e44c2-131">Exemplo 1: Listar todos os appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="e44c2-131">Example 1: List all appConsentRequests</span></span>

### <a name="request"></a><span data-ttu-id="e44c2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e44c2-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e44c2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e44c2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests
```
# <a name="c"></a>[<span data-ttu-id="e44c2-134">C#</span><span class="sxs-lookup"><span data-stu-id="e44c2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appconsentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e44c2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e44c2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appconsentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e44c2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e44c2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appconsentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e44c2-137">Java</span><span class="sxs-lookup"><span data-stu-id="e44c2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appconsentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e44c2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44c2-138">Response</span></span>
<span data-ttu-id="e44c2-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e44c2-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

## <a name="example-2-list-all-appconsentrequests-with-at-least-one-userconsentrequest-whose-status-is-inprogress"></a><span data-ttu-id="e44c2-140">Exemplo 2: listar todos os appConsentRequests com pelo menos um userConsentRequest cujo status é InProgress</span><span class="sxs-lookup"><span data-stu-id="e44c2-140">Example 2: List all appConsentRequests with at least one userConsentRequest whose status is InProgress</span></span>

### <a name="request"></a><span data-ttu-id="e44c2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e44c2-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e44c2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e44c2-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest_userconsentrequest_InProgress"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests?$filter=userConsentRequests/any (u:u/status eq 'InProgress')
```
# <a name="c"></a>[<span data-ttu-id="e44c2-143">C#</span><span class="sxs-lookup"><span data-stu-id="e44c2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appconsentrequest-userconsentrequest-inprogress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e44c2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e44c2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appconsentrequest-userconsentrequest-inprogress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e44c2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e44c2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appconsentrequest-userconsentrequest-inprogress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e44c2-146">Java</span><span class="sxs-lookup"><span data-stu-id="e44c2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appconsentrequest-userconsentrequest-inprogress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e44c2-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44c2-147">Response</span></span>
<span data-ttu-id="e44c2-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e44c2-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests",
    "@odata.count": 1,
    "value": [
      {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

