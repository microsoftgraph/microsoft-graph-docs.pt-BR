---
title: Listar aggregatedPolicyCompliances
description: Obter uma lista dos objetos aggregatedPolicyCompliance e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a9ec9c51db24dc6618eabda1a4d9dda957c23532
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401923"
---
# <a name="list-aggregatedpolicycompliances"></a><span data-ttu-id="ba3b1-103">Listar aggregatedPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="ba3b1-103">List aggregatedPolicyCompliances</span></span>
<span data-ttu-id="ba3b1-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ba3b1-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba3b1-105">Obter uma lista dos [objetos aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-105">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba3b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba3b1-106">Permissions</span></span>
<span data-ttu-id="ba3b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba3b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba3b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba3b1-109">Permission type</span></span>|<span data-ttu-id="ba3b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba3b1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba3b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba3b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba3b1-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba3b1-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba3b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba3b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba3b1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-114">Not supported.</span></span>|
|<span data-ttu-id="ba3b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba3b1-115">Application</span></span>|<span data-ttu-id="ba3b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba3b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba3b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba3b1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba3b1-118">Optional query parameters</span></span>
<span data-ttu-id="ba3b1-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="ba3b1-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba3b1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba3b1-120">Request headers</span></span>
|<span data-ttu-id="ba3b1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ba3b1-121">Name</span></span>|<span data-ttu-id="ba3b1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba3b1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba3b1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba3b1-123">Authorization</span></span>|<span data-ttu-id="ba3b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba3b1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba3b1-126">Request body</span></span>
<span data-ttu-id="ba3b1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba3b1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba3b1-128">Response</span></span>

<span data-ttu-id="ba3b1-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-129">If successful, this method returns a `200 OK` response code and a collection of [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba3b1-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba3b1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba3b1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba3b1-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```


### <a name="response"></a><span data-ttu-id="ba3b1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba3b1-132">Response</span></span>
><span data-ttu-id="ba3b1-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba3b1-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
