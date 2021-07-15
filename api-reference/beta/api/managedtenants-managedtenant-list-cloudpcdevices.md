---
title: Listar cloudPcDevices
description: Obter uma lista dos objetos cloudPcDevice e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 65da1a66a6a423d3df8859d1cf74d16d03f6ded6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441464"
---
# <a name="list-cloudpcdevices"></a><span data-ttu-id="c4b7c-103">Listar cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="c4b7c-103">List cloudPcDevices</span></span>
<span data-ttu-id="c4b7c-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c4b7c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4b7c-105">Obter uma lista dos objetos [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-105">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4b7c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c4b7c-106">Permissions</span></span>
<span data-ttu-id="c4b7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4b7c-109">Permission type</span></span>|<span data-ttu-id="c4b7c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4b7c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4b7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4b7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4b7c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b7c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c4b7c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4b7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4b7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-114">Not supported.</span></span>|
|<span data-ttu-id="c4b7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4b7c-115">Application</span></span>|<span data-ttu-id="c4b7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4b7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b7c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4b7c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4b7c-118">Optional query parameters</span></span>
<span data-ttu-id="c4b7c-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="c4b7c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4b7c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b7c-120">Request headers</span></span>
|<span data-ttu-id="c4b7c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c4b7c-121">Name</span></span>|<span data-ttu-id="c4b7c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4b7c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4b7c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4b7c-123">Authorization</span></span>|<span data-ttu-id="c4b7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4b7c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b7c-126">Request body</span></span>
<span data-ttu-id="c4b7c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4b7c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4b7c-128">Response</span></span>

<span data-ttu-id="c4b7c-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4b7c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4b7c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4b7c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4b7c-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4b7c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b7c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices
```
# <a name="c"></a>[<span data-ttu-id="c4b7c-133">C#</span><span class="sxs-lookup"><span data-stu-id="c4b7c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcdevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4b7c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4b7c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcdevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4b7c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4b7c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcdevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4b7c-136">Java</span><span class="sxs-lookup"><span data-stu-id="c4b7c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcdevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4b7c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4b7c-137">Response</span></span>
><span data-ttu-id="c4b7c-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4b7c-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "00089754-92d2-483c-a073-420723aac8bc_6b97ad6a-be15-4cbe-afbb-4eb74ecb0243",
      "lastUpdated": "2021-07-10T23:05:03.2565097Z",
      "policyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "displayName": "ImageProd - ImageRunner4PROD",
      "managedDeviceId": "f3a8e53b-0a9f-42f1-be73-4fd30d801f62",
      "managedDeviceName": "A0000060000",
      "userPrincipalName": "ImageRunner4PROD@fourthcoffee001.onmicrosoft.com",
      "servicePlanName": "CloudPC_Lite",
      "status": "Provisioned",
      "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
      "tenantDisplayName": "Fourth Coffee Publishing",
      "lastRefreshedDateTime": "2021-07-10T23:05:03.2565097Z",
      "provisioningPolicyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "cloudPcStatus": "Provisioned"
    }
  ]
}
```
