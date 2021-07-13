---
title: Obter managedDeviceComplianceTrend
description: Leia as propriedades e as relações de um objeto managedDeviceComplianceTrend.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 046b110c0aad542db3994bc6eecbba9b1d414feb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401920"
---
# <a name="get-manageddevicecompliancetrend"></a><span data-ttu-id="f56a9-103">Obter managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="f56a9-103">Get managedDeviceComplianceTrend</span></span>
<span data-ttu-id="f56a9-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f56a9-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f56a9-105">Leia as propriedades e as relações de [um objeto managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="f56a9-105">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f56a9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f56a9-106">Permissions</span></span>
<span data-ttu-id="f56a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f56a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f56a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f56a9-109">Permission type</span></span>|<span data-ttu-id="f56a9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f56a9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f56a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f56a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f56a9-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f56a9-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f56a9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f56a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f56a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f56a9-114">Not supported.</span></span>|
|<span data-ttu-id="f56a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f56a9-115">Application</span></span>|<span data-ttu-id="f56a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f56a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f56a9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f56a9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f56a9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f56a9-118">Optional query parameters</span></span>
<span data-ttu-id="f56a9-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f56a9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f56a9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f56a9-120">Request headers</span></span>
|<span data-ttu-id="f56a9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f56a9-121">Name</span></span>|<span data-ttu-id="f56a9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f56a9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f56a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f56a9-123">Authorization</span></span>|<span data-ttu-id="f56a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f56a9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f56a9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f56a9-126">Request body</span></span>
<span data-ttu-id="f56a9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f56a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f56a9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f56a9-128">Response</span></span>

<span data-ttu-id="f56a9-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f56a9-129">If successful, this method returns a `200 OK` response code and a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f56a9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f56a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f56a9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f56a9-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliancetrend"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```


### <a name="response"></a><span data-ttu-id="f56a9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f56a9-132">Response</span></span>
><span data-ttu-id="f56a9-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f56a9-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b_2021-07-11T00:00:00Z",
  "tenantDisplayName": "Fourth Coffee",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "unknownDeviceCount": 2,
  "compliantDeviceCount": 0,
  "noncompliantDeviceCount": 41,
  "errorDeviceCount": 1,
  "inGracePeriodDeviceCount": 0,
  "configManagerDeviceCount": 0,
  "totalDeviceCount": 44,
  "countDateTime": "2021-07-11T00:00:00Z"
}
```
