---
title: Listar credentialUserRegistrationsSummaries
description: Obter uma lista dos objetos credentialUserRegistrationsSummary e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0b6df505752378f35f1594fac7d59239bb9d0dfd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442917"
---
# <a name="list-credentialuserregistrationssummaries"></a><span data-ttu-id="d4d4e-103">Listar credentialUserRegistrationsSummaries</span><span class="sxs-lookup"><span data-stu-id="d4d4e-103">List credentialUserRegistrationsSummaries</span></span>
<span data-ttu-id="d4d4e-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d4d4e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4d4e-105">Obter uma lista dos [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-105">Get a list of the [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4d4e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d4d4e-106">Permissions</span></span>
<span data-ttu-id="d4d4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d4e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4d4e-109">Permission type</span></span>|<span data-ttu-id="d4d4e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4d4e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4d4e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4d4e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4d4e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4d4e-112">Reports.Read.All</span></span>|
|<span data-ttu-id="d4d4e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4d4e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4d4e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-114">Not supported.</span></span>|
|<span data-ttu-id="d4d4e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4d4e-115">Application</span></span>|<span data-ttu-id="d4d4e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4d4e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4d4e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4d4e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4d4e-118">Optional query parameters</span></span>
<span data-ttu-id="d4d4e-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="d4d4e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4d4e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d4e-120">Request headers</span></span>
|<span data-ttu-id="d4d4e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d4d4e-121">Name</span></span>|<span data-ttu-id="d4d4e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4d4e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4d4e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4d4e-123">Authorization</span></span>|<span data-ttu-id="d4d4e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4d4e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d4e-126">Request body</span></span>
<span data-ttu-id="d4d4e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4d4e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4d4e-128">Response</span></span>

<span data-ttu-id="d4d4e-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-129">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4d4e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4d4e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4d4e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d4e-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d4d4e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4d4e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```
# <a name="c"></a>[<span data-ttu-id="d4d4e-133">C#</span><span class="sxs-lookup"><span data-stu-id="d4d4e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-credentialuserregistrationssummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4d4e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4d4e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-credentialuserregistrationssummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4d4e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4d4e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-credentialuserregistrationssummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4d4e-136">Java</span><span class="sxs-lookup"><span data-stu-id="d4d4e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-credentialuserregistrationssummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d4d4e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4d4e-137">Response</span></span>
><span data-ttu-id="d4d4e-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4d4e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.credentialUserRegistrationsSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#credentialUserRegistrationsSummaries",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "mfaAndSsprCapableUserCount": 2,
      "ssprEnabledUserCount": 9,
      "mfaRegisteredUserCount": 3,
      "ssprRegisteredUserCount": 2,
      "totalUserCount": 9,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabled",
      "lastRefreshedDateTime": "2021-07-11T09:58:11.5730661Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "mfaAndSsprCapableUserCount": 0,
      "ssprEnabledUserCount": 1,
      "mfaRegisteredUserCount": 0,
      "ssprRegisteredUserCount": 0,
      "totalUserCount": 7,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
      "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
