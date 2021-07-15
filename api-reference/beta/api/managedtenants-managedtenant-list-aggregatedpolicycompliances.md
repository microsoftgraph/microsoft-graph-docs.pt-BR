---
title: Listar aggregatedPolicyCompliances
description: Obter uma lista dos objetos aggregatedPolicyCompliance e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 160292f38035390d7b5ed769bbea42847bba71b2
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441491"
---
# <a name="list-aggregatedpolicycompliances"></a><span data-ttu-id="af291-103">Listar aggregatedPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="af291-103">List aggregatedPolicyCompliances</span></span>
<span data-ttu-id="af291-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="af291-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af291-105">Obter uma lista dos [objetos aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="af291-105">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="af291-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="af291-106">Permissions</span></span>
<span data-ttu-id="af291-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af291-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af291-109">Permission type</span></span>|<span data-ttu-id="af291-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af291-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af291-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af291-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af291-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af291-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af291-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af291-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af291-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af291-114">Not supported.</span></span>|
|<span data-ttu-id="af291-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af291-115">Application</span></span>|<span data-ttu-id="af291-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af291-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af291-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af291-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af291-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af291-118">Optional query parameters</span></span>
<span data-ttu-id="af291-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="af291-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af291-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af291-120">Request headers</span></span>
|<span data-ttu-id="af291-121">Nome</span><span class="sxs-lookup"><span data-stu-id="af291-121">Name</span></span>|<span data-ttu-id="af291-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="af291-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af291-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="af291-123">Authorization</span></span>|<span data-ttu-id="af291-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af291-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af291-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af291-126">Request body</span></span>
<span data-ttu-id="af291-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af291-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af291-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af291-128">Response</span></span>

<span data-ttu-id="af291-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af291-129">If successful, this method returns a `200 OK` response code and a collection of [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af291-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af291-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af291-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af291-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="af291-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="af291-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```
# <a name="c"></a>[<span data-ttu-id="af291-133">C#</span><span class="sxs-lookup"><span data-stu-id="af291-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-aggregatedpolicycompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af291-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af291-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-aggregatedpolicycompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af291-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af291-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-aggregatedpolicycompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af291-136">Java</span><span class="sxs-lookup"><span data-stu-id="af291-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-aggregatedpolicycompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="af291-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="af291-137">Response</span></span>
><span data-ttu-id="af291-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="af291-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.aggregatedPolicyCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#aggregatedPolicyCompliances",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyName": "Baseline - Setup Compliance Policy for Windows devices",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 0,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-06-22T17:01:46Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyId": "3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyName": "Windows Level 2 Compliance Policy",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 4,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-04-20T22:27:20Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
