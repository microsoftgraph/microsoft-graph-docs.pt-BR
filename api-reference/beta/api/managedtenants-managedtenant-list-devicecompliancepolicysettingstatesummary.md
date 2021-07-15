---
title: Listar deviceCompliancePolicySettingStateSummary
description: Obter uma lista dos objetos deviceCompliancePolicySettingStateSummary e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ec117e3f93732e3134f6451c83477eb342a98d39
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441994"
---
# <a name="list-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="2b5e6-103">Listar deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="2b5e6-103">List deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="2b5e6-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2b5e6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b5e6-105">Obter uma lista dos [objetos deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-105">Get a list of the [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b5e6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2b5e6-106">Permissions</span></span>
<span data-ttu-id="2b5e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b5e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b5e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b5e6-109">Permission type</span></span>|<span data-ttu-id="2b5e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b5e6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b5e6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b5e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b5e6-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5e6-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2b5e6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b5e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b5e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-114">Not supported.</span></span>|
|<span data-ttu-id="2b5e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b5e6-115">Application</span></span>|<span data-ttu-id="2b5e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b5e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b5e6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b5e6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b5e6-118">Optional query parameters</span></span>
<span data-ttu-id="2b5e6-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="2b5e6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b5e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b5e6-120">Request headers</span></span>
|<span data-ttu-id="2b5e6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2b5e6-121">Name</span></span>|<span data-ttu-id="2b5e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b5e6-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b5e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b5e6-123">Authorization</span></span>|<span data-ttu-id="2b5e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b5e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b5e6-126">Request body</span></span>
<span data-ttu-id="2b5e6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b5e6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b5e6-128">Response</span></span>

<span data-ttu-id="2b5e6-129">Se tiver êxito, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b5e6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2b5e6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b5e6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b5e6-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2b5e6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b5e6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```
# <a name="c"></a>[<span data-ttu-id="2b5e6-133">C#</span><span class="sxs-lookup"><span data-stu-id="2b5e6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-devicecompliancepolicysettingstatesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b5e6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b5e6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-devicecompliancepolicysettingstatesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b5e6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b5e6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-devicecompliancepolicysettingstatesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b5e6-136">Java</span><span class="sxs-lookup"><span data-stu-id="2b5e6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-devicecompliancepolicysettingstatesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2b5e6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b5e6-137">Response</span></span>
><span data-ttu-id="2b5e6-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2b5e6-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
      "id": "9f6922d9-5a58-4f4d-b6e3-708f7659e5b2",
      "tenantId": "String",
      "tenantDisplayName": "String",
      "conflictDeviceCount": "Integer",
      "errorDeviceCount": "Integer",
      "failedDeviceCount": "Integer",
      "intuneAccountId": "String",
      "intuneSettingId": "String",
      "notApplicableDeviceCount": "Integer",
      "pendingDeviceCount": "Integer",
      "policyType": "String",
      "settingName": "String",
      "succeededDeviceCount": "Integer",
      "lastRefreshedDateTime": "String (timestamp)"
    }
  ]
}
```
