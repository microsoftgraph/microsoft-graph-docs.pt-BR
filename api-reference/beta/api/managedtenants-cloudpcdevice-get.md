---
title: Obter cloudPcDevice
description: Leia as propriedades e as relações de um objeto cloudPcDevice.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 7ac75ce4b9ae607d3a616bc630f10d4e7c4e7fa3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440159"
---
# <a name="get-cloudpcdevice"></a><span data-ttu-id="f2907-103">Obter cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="f2907-103">Get cloudPcDevice</span></span>
<span data-ttu-id="f2907-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f2907-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2907-105">Leia as propriedades e as relações de um [objeto cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="f2907-105">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2907-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f2907-106">Permissions</span></span>
<span data-ttu-id="f2907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2907-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2907-109">Permission type</span></span>|<span data-ttu-id="f2907-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2907-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2907-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2907-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2907-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2907-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f2907-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2907-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2907-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2907-114">Not supported.</span></span>|
|<span data-ttu-id="f2907-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2907-115">Application</span></span>|<span data-ttu-id="f2907-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2907-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2907-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2907-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2907-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2907-118">Optional query parameters</span></span>
<span data-ttu-id="f2907-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f2907-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2907-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2907-120">Request headers</span></span>
|<span data-ttu-id="f2907-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f2907-121">Name</span></span>|<span data-ttu-id="f2907-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2907-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2907-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2907-123">Authorization</span></span>|<span data-ttu-id="f2907-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2907-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2907-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2907-126">Request body</span></span>
<span data-ttu-id="f2907-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2907-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2907-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2907-128">Response</span></span>

<span data-ttu-id="f2907-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2907-129">If successful, this method returns a `200 OK` response code and a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2907-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2907-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2907-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2907-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2907-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2907-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```
# <a name="c"></a>[<span data-ttu-id="f2907-133">C#</span><span class="sxs-lookup"><span data-stu-id="f2907-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2907-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2907-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2907-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2907-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2907-136">Java</span><span class="sxs-lookup"><span data-stu-id="f2907-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2907-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2907-137">Response</span></span>
><span data-ttu-id="f2907-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f2907-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
