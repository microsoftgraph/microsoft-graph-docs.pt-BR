---
title: Obter cloudPcOnPremisesConnection
description: Leia as propriedades e os relacionamentos do objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c1d9945b9fb5458ec5e497f8b757d07388d73f8b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158272"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="8285d-103">Obter cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="8285d-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="8285d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8285d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8285d-105">Leia as propriedades e os relacionamentos do objeto [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="8285d-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="8285d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8285d-106">Permissions</span></span>

<span data-ttu-id="8285d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8285d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8285d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8285d-109">Permission type</span></span>| <span data-ttu-id="8285d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8285d-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="8285d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8285d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8285d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8285d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8285d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8285d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8285d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8285d-114">Not supported.</span></span>|
|<span data-ttu-id="8285d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8285d-115">Application</span></span>| <span data-ttu-id="8285d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8285d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8285d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8285d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8285d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8285d-118">Optional query parameters</span></span>

<span data-ttu-id="8285d-119">Esse método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8285d-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="8285d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8285d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8285d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8285d-121">Request headers</span></span>

| <span data-ttu-id="8285d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8285d-122">Name</span></span>          | <span data-ttu-id="8285d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8285d-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8285d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8285d-124">Authorization</span></span> | <span data-ttu-id="8285d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8285d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8285d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8285d-127">Request body</span></span>

<span data-ttu-id="8285d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8285d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8285d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8285d-129">Response</span></span>

<span data-ttu-id="8285d-130">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8285d-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8285d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8285d-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="8285d-132">Exemplo 1: Obter as propriedades padrão de uma conexão local</span><span class="sxs-lookup"><span data-stu-id="8285d-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="8285d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8285d-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8285d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8285d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="8285d-135">C#</span><span class="sxs-lookup"><span data-stu-id="8285d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8285d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8285d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8285d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8285d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8285d-138">Java</span><span class="sxs-lookup"><span data-stu-id="8285d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8285d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8285d-139">Response</span></span>

<span data-ttu-id="8285d-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8285d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="8285d-141">Exemplo 2: Obter as propriedades selecionadas de uma conexão local, incluindo healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="8285d-141">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="8285d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8285d-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8285d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8285d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse
```
# <a name="c"></a>[<span data-ttu-id="8285d-144">C#</span><span class="sxs-lookup"><span data-stu-id="8285d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-withdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8285d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8285d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-withdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8285d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8285d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-withdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8285d-147">Java</span><span class="sxs-lookup"><span data-stu-id="8285d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-withdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8285d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8285d-148">Response</span></span>

<span data-ttu-id="8285d-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8285d-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
