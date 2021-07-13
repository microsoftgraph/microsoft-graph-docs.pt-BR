---
title: Listar cloudPcDevices
description: Obter uma lista dos objetos cloudPcDevice e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 7ecb462727541ab591e921ff9cac5cbafcac612c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401900"
---
# <a name="list-cloudpcdevices"></a><span data-ttu-id="fa142-103">Listar cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="fa142-103">List cloudPcDevices</span></span>
<span data-ttu-id="fa142-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="fa142-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa142-105">Obter uma lista dos objetos [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="fa142-105">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa142-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa142-106">Permissions</span></span>
<span data-ttu-id="fa142-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa142-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa142-109">Permission type</span></span>|<span data-ttu-id="fa142-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa142-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa142-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa142-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa142-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa142-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="fa142-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa142-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa142-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa142-114">Not supported.</span></span>|
|<span data-ttu-id="fa142-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa142-115">Application</span></span>|<span data-ttu-id="fa142-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa142-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa142-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa142-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa142-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa142-118">Optional query parameters</span></span>
<span data-ttu-id="fa142-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="fa142-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa142-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa142-120">Request headers</span></span>
|<span data-ttu-id="fa142-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fa142-121">Name</span></span>|<span data-ttu-id="fa142-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa142-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa142-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa142-123">Authorization</span></span>|<span data-ttu-id="fa142-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa142-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa142-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa142-126">Request body</span></span>
<span data-ttu-id="fa142-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa142-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa142-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa142-128">Response</span></span>

<span data-ttu-id="fa142-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa142-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa142-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa142-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa142-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa142-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices
```


### <a name="response"></a><span data-ttu-id="fa142-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa142-132">Response</span></span>
><span data-ttu-id="fa142-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa142-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "00089754-92d2-483c-a073-420723aac8bc_6b97ad6a-be15-4cbe-afbb-4eb74ecb0243",
      "lastUpdated": "2021-07-10T23:05:03.2565097Z",
      "policyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "displayName": "ImageProd - ImageRunner4PROD",
      "managedDeviceId": "f3a8e53b-0a9f-42f1-be73-4fd30d801f62",
      "managedDeviceName": "A0000060000",
      "userPrincipalName": "ImageRunner4PROD@fourthcoffee001.onmicrosoft.com",
      "servicePlanName": "CloudPC_Lite",
      "status": "Provisioned",
      "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
      "tenantDisplayName": "Fourth Coffee Publishing",
      "lastRefreshedDateTime": "2021-07-10T23:05:03.2565097Z",
      "provisioningPolicyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "cloudPcStatus": "Provisioned"
    }
  ]
}
```
