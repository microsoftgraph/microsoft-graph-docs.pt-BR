---
title: Obter cloudPcDevice
description: Leia as propriedades e as relações de um objeto cloudPcDevice.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 26d9b438bf366a0a3b4b367bc96ea74441d5324d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401928"
---
# <a name="get-cloudpcdevice"></a><span data-ttu-id="47ff3-103">Obter cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="47ff3-103">Get cloudPcDevice</span></span>
<span data-ttu-id="47ff3-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="47ff3-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47ff3-105">Leia as propriedades e as relações de um [objeto cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="47ff3-105">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47ff3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47ff3-106">Permissions</span></span>
<span data-ttu-id="47ff3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47ff3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47ff3-109">Permission type</span></span>|<span data-ttu-id="47ff3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47ff3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47ff3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47ff3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47ff3-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47ff3-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="47ff3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47ff3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47ff3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47ff3-114">Not supported.</span></span>|
|<span data-ttu-id="47ff3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47ff3-115">Application</span></span>|<span data-ttu-id="47ff3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47ff3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47ff3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47ff3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47ff3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47ff3-118">Optional query parameters</span></span>
<span data-ttu-id="47ff3-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="47ff3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47ff3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47ff3-120">Request headers</span></span>
|<span data-ttu-id="47ff3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="47ff3-121">Name</span></span>|<span data-ttu-id="47ff3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="47ff3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47ff3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47ff3-123">Authorization</span></span>|<span data-ttu-id="47ff3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47ff3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47ff3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47ff3-126">Request body</span></span>
<span data-ttu-id="47ff3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47ff3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47ff3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="47ff3-128">Response</span></span>

<span data-ttu-id="47ff3-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47ff3-129">If successful, this method returns a `200 OK` response code and a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47ff3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47ff3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47ff3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47ff3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```


### <a name="response"></a><span data-ttu-id="47ff3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="47ff3-132">Response</span></span>
><span data-ttu-id="47ff3-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47ff3-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
    "id": "1307ab1b-63ee-4942-bdef-bcd4f415c635",
    "lastUpdated": "2021-07-10T23:05:03.2564744Z",
    "policyId": "",
    "displayName": "device01",
    "managedDeviceId": "",
    "managedDeviceName": "",
    "userPrincipalName": "sally@lucernepublishing001.onmicrosoft.com",
    "servicePlanName": "CloudPC_Standard",
    "status": "NotProvisioned",
    "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
    "tenantDisplayName": "Lucerne Publishing",
    "lastRefreshedDateTime": "2021-07-10T23:05:03.2564744Z",
    "provisioningPolicyId": "",
    "cloudPcStatus": "NotProvisioned"
}
```
