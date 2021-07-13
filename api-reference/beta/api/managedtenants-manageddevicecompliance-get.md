---
title: Obter managedDeviceCompliance
description: Leia as propriedades e as relações de um objeto managedDeviceCompliance.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: be93e13c483e11327bfe5725d9b779cfccd89354
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401921"
---
# <a name="get-manageddevicecompliance"></a><span data-ttu-id="1101e-103">Obter managedDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="1101e-103">Get managedDeviceCompliance</span></span>
<span data-ttu-id="1101e-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="1101e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1101e-105">Leia as propriedades e as relações de um [objeto managedDeviceCompliance.](../resources/managedtenants-manageddevicecompliance.md)</span><span class="sxs-lookup"><span data-stu-id="1101e-105">Read the properties and relationships of a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1101e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1101e-106">Permissions</span></span>
<span data-ttu-id="1101e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1101e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1101e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1101e-109">Permission type</span></span>|<span data-ttu-id="1101e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1101e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1101e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1101e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1101e-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1101e-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1101e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1101e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1101e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1101e-114">Not supported.</span></span>|
|<span data-ttu-id="1101e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1101e-115">Application</span></span>|<span data-ttu-id="1101e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1101e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1101e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1101e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1101e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1101e-118">Optional query parameters</span></span>
<span data-ttu-id="1101e-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="1101e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1101e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1101e-120">Request headers</span></span>
|<span data-ttu-id="1101e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1101e-121">Name</span></span>|<span data-ttu-id="1101e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1101e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1101e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1101e-123">Authorization</span></span>|<span data-ttu-id="1101e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1101e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1101e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1101e-126">Request body</span></span>
<span data-ttu-id="1101e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1101e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1101e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1101e-128">Response</span></span>

<span data-ttu-id="1101e-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1101e-129">If successful, this method returns a `200 OK` response code and a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1101e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1101e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1101e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1101e-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```


### <a name="response"></a><span data-ttu-id="1101e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1101e-132">Response</span></span>
><span data-ttu-id="1101e-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1101e-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceCompliance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managedDeviceCompliances/$entity",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceName": "vm11",
    "complianceStatus": "Compliant",
    "osDescription": "Windows",
    "osVersion": "10.0.19042.1083",
    "lastSyncDateTime": "2021-07-09T14:41:21.9130091Z",
    "ownerType": "Company",
    "model": "Virtual Machine",
    "manufacturer": "Microsoft Corporation",
    "inGracePeriodUntilDateTime": "9999-12-31T23:59:59.9999999Z",
    "lastRefreshedDateTime": "2021-07-11T07:12:41.0336556Z",
    "deviceType": "WindowsRT",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
