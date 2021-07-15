---
title: Obter managedDeviceCompliance
description: Leia as propriedades e as relações de um objeto managedDeviceCompliance.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c755a480a8b188042053c112f323fd1a372671c6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439942"
---
# <a name="get-manageddevicecompliance"></a><span data-ttu-id="6ccd8-103">Obter managedDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="6ccd8-103">Get managedDeviceCompliance</span></span>
<span data-ttu-id="6ccd8-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6ccd8-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ccd8-105">Leia as propriedades e as relações de um [objeto managedDeviceCompliance.](../resources/managedtenants-manageddevicecompliance.md)</span><span class="sxs-lookup"><span data-stu-id="6ccd8-105">Read the properties and relationships of a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ccd8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6ccd8-106">Permissions</span></span>
<span data-ttu-id="6ccd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ccd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ccd8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ccd8-109">Permission type</span></span>|<span data-ttu-id="6ccd8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ccd8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ccd8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ccd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ccd8-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ccd8-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6ccd8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ccd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ccd8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ccd8-114">Not supported.</span></span>|
|<span data-ttu-id="6ccd8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ccd8-115">Application</span></span>|<span data-ttu-id="6ccd8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ccd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ccd8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ccd8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ccd8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ccd8-118">Optional query parameters</span></span>
<span data-ttu-id="6ccd8-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="6ccd8-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ccd8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ccd8-120">Request headers</span></span>
|<span data-ttu-id="6ccd8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6ccd8-121">Name</span></span>|<span data-ttu-id="6ccd8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ccd8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6ccd8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ccd8-123">Authorization</span></span>|<span data-ttu-id="6ccd8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ccd8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ccd8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ccd8-126">Request body</span></span>
<span data-ttu-id="6ccd8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ccd8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ccd8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ccd8-128">Response</span></span>

<span data-ttu-id="6ccd8-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ccd8-129">If successful, this method returns a `200 OK` response code and a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ccd8-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6ccd8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ccd8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ccd8-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6ccd8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ccd8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```
# <a name="c"></a>[<span data-ttu-id="6ccd8-133">C#</span><span class="sxs-lookup"><span data-stu-id="6ccd8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manageddevicecompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ccd8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ccd8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manageddevicecompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ccd8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ccd8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manageddevicecompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ccd8-136">Java</span><span class="sxs-lookup"><span data-stu-id="6ccd8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manageddevicecompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6ccd8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ccd8-137">Response</span></span>
><span data-ttu-id="6ccd8-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ccd8-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
