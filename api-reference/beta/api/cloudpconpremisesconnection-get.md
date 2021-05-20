---
title: Obter cloudPcOnPremisesConnection
description: Leia as propriedades e as relações do objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 291e6e17494bf8dcfc467b8d3c594f27d6b2e710
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546837"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="1f882-103">Obter cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="1f882-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="1f882-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f882-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f882-105">Leia as propriedades e as relações do [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="1f882-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="1f882-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f882-106">Permissions</span></span>

<span data-ttu-id="1f882-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f882-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f882-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f882-109">Permission type</span></span>| <span data-ttu-id="1f882-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f882-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="1f882-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f882-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f882-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f882-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="1f882-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f882-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f882-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f882-114">Not supported.</span></span>|
|<span data-ttu-id="1f882-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f882-115">Application</span></span>|<span data-ttu-id="1f882-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f882-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f882-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f882-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f882-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f882-118">Optional query parameters</span></span>

<span data-ttu-id="1f882-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f882-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="1f882-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f882-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f882-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-121">Request headers</span></span>

| <span data-ttu-id="1f882-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1f882-122">Name</span></span>          | <span data-ttu-id="1f882-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f882-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1f882-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f882-124">Authorization</span></span> | <span data-ttu-id="1f882-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f882-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f882-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-127">Request body</span></span>

<span data-ttu-id="1f882-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f882-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f882-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f882-129">Response</span></span>

<span data-ttu-id="1f882-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f882-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f882-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1f882-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="1f882-132">Exemplo 1: Obter as propriedades padrão de uma conexão local</span><span class="sxs-lookup"><span data-stu-id="1f882-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="1f882-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f882-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f882-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="1f882-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f882-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f882-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f882-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f882-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f882-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f882-138">Java</span><span class="sxs-lookup"><span data-stu-id="1f882-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f882-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f882-139">Response</span></span>

<span data-ttu-id="1f882-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f882-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
    "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdccffff",
    "displayName": "Display Name value",
    "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
    "subscriptionName": "Subscription Name value",
    "adDomainName": "Active Directory Domain Name value",
    "adDomainUsername": "Active Directory Domain User Name value",
    "organizationalUnit": "Organization Unit value",
    "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
    "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
    "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
    "healthCheckStatus": "running"
  }
}
```

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="1f882-141">Exemplo 2: Obter as propriedades selecionadas de uma conexão local, incluindo healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="1f882-141">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="1f882-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f882-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1f882-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f882-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse
```
# <a name="c"></a>[<span data-ttu-id="1f882-144">C#</span><span class="sxs-lookup"><span data-stu-id="1f882-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-withdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f882-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f882-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-withdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f882-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f882-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-withdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f882-147">Java</span><span class="sxs-lookup"><span data-stu-id="1f882-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-withdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f882-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f882-148">Response</span></span>

<span data-ttu-id="1f882-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f882-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
    "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdccffff",
    "displayName": "Display Name value",
    "healthCheckStatus": "failed",
    "healthCheckStatusDetails": {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
      "startDateTime": "2020-11-03T12:43:14Z",
      "endDateTime": "2020-11-03T12:43:32Z",
      "healthChecks": [
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "failed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:14Z",
          "endDateTime": "2020-11-03T12:43:15Z",
          "errorType": "dnsCheckFqdnNotFound",
          "recommendedAction": "We did not find the provided domain name; please re-enter",
          "additionalDdetails": null
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "passed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:15Z",
          "endDateTime": "2020-11-03T12:43:26Z",
          "errorType": null,
          "recommendedAction": null,
          "additionalDetails": null
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "failed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:27Z",
          "endDateTime": "2020-11-03T12:43:32Z",
          "errorType": "endpointConnectivityCheckUrlNotWhitelisted",
          "recommendedAction": "Recommended Action value",
          "additionaldDetails": "Additional Details value"
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "passed",
          "displayName": "Display Name value",
          "startDateTime": null,
          "endDateTime": null,
          "errorType": null,
          "recommendedAction": null,
          "additionaldDetails": null
        }
      ]
    },
    "inUse": false
  }
}
```
