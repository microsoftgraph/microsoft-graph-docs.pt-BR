---
title: Obter managedDeviceComplianceTrend
description: Leia as propriedades e as relações de um objeto managedDeviceComplianceTrend.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 21e6583fe4e4f5840409e4153d47b0a945bd3ba9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441608"
---
# <a name="get-manageddevicecompliancetrend"></a><span data-ttu-id="35071-103">Obter managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="35071-103">Get managedDeviceComplianceTrend</span></span>
<span data-ttu-id="35071-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="35071-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35071-105">Leia as propriedades e as relações de [um objeto managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="35071-105">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="35071-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="35071-106">Permissions</span></span>
<span data-ttu-id="35071-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35071-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35071-109">Permission type</span></span>|<span data-ttu-id="35071-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35071-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35071-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35071-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35071-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35071-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="35071-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35071-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35071-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35071-114">Not supported.</span></span>|
|<span data-ttu-id="35071-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35071-115">Application</span></span>|<span data-ttu-id="35071-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35071-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35071-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35071-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35071-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="35071-118">Optional query parameters</span></span>
<span data-ttu-id="35071-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="35071-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35071-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35071-120">Request headers</span></span>
|<span data-ttu-id="35071-121">Nome</span><span class="sxs-lookup"><span data-stu-id="35071-121">Name</span></span>|<span data-ttu-id="35071-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="35071-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="35071-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35071-123">Authorization</span></span>|<span data-ttu-id="35071-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35071-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35071-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35071-126">Request body</span></span>
<span data-ttu-id="35071-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35071-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35071-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="35071-128">Response</span></span>

<span data-ttu-id="35071-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35071-129">If successful, this method returns a `200 OK` response code and a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35071-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="35071-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35071-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35071-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="35071-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="35071-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliancetrend"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```
# <a name="c"></a>[<span data-ttu-id="35071-133">C#</span><span class="sxs-lookup"><span data-stu-id="35071-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manageddevicecompliancetrend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35071-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35071-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manageddevicecompliancetrend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35071-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35071-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manageddevicecompliancetrend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35071-136">Java</span><span class="sxs-lookup"><span data-stu-id="35071-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manageddevicecompliancetrend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="35071-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="35071-137">Response</span></span>
><span data-ttu-id="35071-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="35071-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
