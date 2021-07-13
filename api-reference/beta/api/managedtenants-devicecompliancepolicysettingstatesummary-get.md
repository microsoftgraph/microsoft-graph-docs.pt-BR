---
title: Acessar deviceCompliancePolicySettingStateSummary
description: Leia as propriedades e as relações de um objeto deviceCompliancePolicySettingStateSummary.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e1396b66dda6925be6c895aac741d81122d64c98
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401922"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="8d0f4-103">Acessar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="8d0f4-103">Get deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="8d0f4-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8d0f4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d0f4-105">Leia as propriedades e as relações de um [objeto deviceCompliancePolicySettingStateSummary.](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="8d0f4-105">Read the properties and relationships of a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d0f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d0f4-106">Permissions</span></span>
<span data-ttu-id="8d0f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d0f4-109">Permission type</span></span>|<span data-ttu-id="8d0f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d0f4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d0f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0f4-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0f4-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d0f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d0f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d0f4-114">Not supported.</span></span>|
|<span data-ttu-id="8d0f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d0f4-115">Application</span></span>|<span data-ttu-id="8d0f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d0f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d0f4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d0f4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d0f4-118">Optional query parameters</span></span>
<span data-ttu-id="8d0f4-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="8d0f4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d0f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d0f4-120">Request headers</span></span>
|<span data-ttu-id="8d0f4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8d0f4-121">Name</span></span>|<span data-ttu-id="8d0f4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d0f4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d0f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d0f4-123">Authorization</span></span>|<span data-ttu-id="8d0f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d0f4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d0f4-126">Request body</span></span>
<span data-ttu-id="8d0f4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d0f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d0f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d0f4-128">Response</span></span>

<span data-ttu-id="8d0f4-129">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d0f4-129">If successful, this method returns a `200 OK` response code and a [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d0f4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d0f4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d0f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d0f4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummarys/{deviceCompliancePolicySettingStateSummaryId}
```


### <a name="response"></a><span data-ttu-id="8d0f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d0f4-132">Response</span></span>
><span data-ttu-id="8d0f4-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d0f4-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_277f9230-81f7-ffc3-af78-4662ec3dca09",
    "intuneAccountId": "6f3e6534-b466-4fac-9a31-4c305cc40833",
    "intuneSettingId": "277f9230-81f7-ffc3-af78-4662ec3dca09",
    "policyType": "DefaultDeviceCompliancePolicy",
    "settingName": "RequireDeviceCompliancePolicyAssigned",
    "failedDeviceCount": 0,
    "errorDeviceCount": 4,
    "conflictDeviceCount": 0,
    "lastRefreshedDateTime": "2021-07-11T00:00:00Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
