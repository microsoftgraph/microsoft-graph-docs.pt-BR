---
title: Obter windowsProtectionState
description: Leia as propriedades e as relações de um objeto windowsProtectionState.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: dc82bbc7dfa7265471cbc6b99f1463d59db5b526
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402109"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="b86a0-103">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="b86a0-103">Get windowsProtectionState</span></span>
<span data-ttu-id="b86a0-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="b86a0-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b86a0-105">Leia as propriedades e as relações de um [objeto windowsProtectionState.](../resources/managedtenants-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="b86a0-105">Read the properties and relationships of a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b86a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b86a0-106">Permissions</span></span>
<span data-ttu-id="b86a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b86a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b86a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b86a0-109">Permission type</span></span>|<span data-ttu-id="b86a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b86a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b86a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b86a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b86a0-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b86a0-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b86a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b86a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b86a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b86a0-114">Not supported.</span></span>|
|<span data-ttu-id="b86a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b86a0-115">Application</span></span>|<span data-ttu-id="b86a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b86a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b86a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b86a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b86a0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b86a0-118">Optional query parameters</span></span>
<span data-ttu-id="b86a0-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="b86a0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b86a0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b86a0-120">Request headers</span></span>
|<span data-ttu-id="b86a0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b86a0-121">Name</span></span>|<span data-ttu-id="b86a0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b86a0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b86a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b86a0-123">Authorization</span></span>|<span data-ttu-id="b86a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b86a0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b86a0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b86a0-126">Request body</span></span>
<span data-ttu-id="b86a0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b86a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b86a0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b86a0-128">Response</span></span>

<span data-ttu-id="b86a0-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b86a0-129">If successful, this method returns a `200 OK` response code and a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b86a0-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b86a0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b86a0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b86a0-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```


### <a name="response"></a><span data-ttu-id="b86a0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b86a0-132">Response</span></span>
><span data-ttu-id="b86a0-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b86a0-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.windowsProtectionState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/windowsProtectionStates/$entity",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceName": "vm11",
    "malwareProtectionEnabled": true,
    "managedDeviceHealthState": "Clean",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": false,
    "fullScanOverdue": false,
    "signatureUpdateOverdue": false,
    "rebootRequired": false,
    "attentionRequired": false,
    "fullScanRequired": false,
    "engineVersion": "1.1.18300.4",
    "signatureVersion": "1.343.642.0",
    "antiMalwareVersion": "4.18.2106.6",
    "lastQuickScanDateTime": "2021-06-24T14:50:28Z",
    "lastFullScanDateTime": null,
    "lastQuickScanSignatureVersion": "1.341.1288.0",
    "lastFullScanSignatureVersion": "0.0.0.0",
    "lastReportedDateTime": "2021-07-09T14:43:45Z",
    "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
    "deviceDeleted": false,
    "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee",
    "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
}
```
