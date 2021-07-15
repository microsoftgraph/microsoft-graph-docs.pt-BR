---
title: Obter windowsProtectionState
description: Leia as propriedades e as relações de um objeto windowsProtectionState.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: b05fbf482810180d1ac87b8f84b71bd283e28e7e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441195"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="df67d-103">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="df67d-103">Get windowsProtectionState</span></span>
<span data-ttu-id="df67d-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="df67d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df67d-105">Leia as propriedades e as relações de um [objeto windowsProtectionState.](../resources/managedtenants-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="df67d-105">Read the properties and relationships of a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df67d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="df67d-106">Permissions</span></span>
<span data-ttu-id="df67d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df67d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df67d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df67d-109">Permission type</span></span>|<span data-ttu-id="df67d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df67d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df67d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df67d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df67d-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df67d-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="df67d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df67d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df67d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df67d-114">Not supported.</span></span>|
|<span data-ttu-id="df67d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df67d-115">Application</span></span>|<span data-ttu-id="df67d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df67d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df67d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df67d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df67d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df67d-118">Optional query parameters</span></span>
<span data-ttu-id="df67d-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="df67d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df67d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df67d-120">Request headers</span></span>
|<span data-ttu-id="df67d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="df67d-121">Name</span></span>|<span data-ttu-id="df67d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="df67d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="df67d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df67d-123">Authorization</span></span>|<span data-ttu-id="df67d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df67d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df67d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df67d-126">Request body</span></span>
<span data-ttu-id="df67d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df67d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df67d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="df67d-128">Response</span></span>

<span data-ttu-id="df67d-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df67d-129">If successful, this method returns a `200 OK` response code and a [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df67d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df67d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df67d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df67d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="df67d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="df67d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}
```
# <a name="c"></a>[<span data-ttu-id="df67d-133">C#</span><span class="sxs-lookup"><span data-stu-id="df67d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-windowsprotectionstate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df67d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df67d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-windowsprotectionstate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df67d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df67d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-windowsprotectionstate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df67d-136">Java</span><span class="sxs-lookup"><span data-stu-id="df67d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-windowsprotectionstate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="df67d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="df67d-137">Response</span></span>
><span data-ttu-id="df67d-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df67d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
