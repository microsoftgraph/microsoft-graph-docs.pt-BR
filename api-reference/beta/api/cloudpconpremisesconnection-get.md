---
title: Obter cloudPcOnPremisesConnection
description: Leia as propriedades e as relações do objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 24c5be1f4e05a91b52821b24ab76885f63124c2c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378208"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="c9e63-103">Obter cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c9e63-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="c9e63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9e63-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9e63-105">Leia as propriedades e as relações do objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="c9e63-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9e63-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c9e63-106">Permissions</span></span>

<span data-ttu-id="c9e63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9e63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9e63-109">Permission type</span></span>| <span data-ttu-id="c9e63-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9e63-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="c9e63-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9e63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9e63-112">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="c9e63-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="c9e63-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9e63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9e63-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9e63-114">Not supported.</span></span>|
|<span data-ttu-id="c9e63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9e63-115">Application</span></span>| <span data-ttu-id="c9e63-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9e63-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9e63-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9e63-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9e63-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c9e63-118">Optional query parameters</span></span>

<span data-ttu-id="c9e63-119">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c9e63-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="c9e63-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c9e63-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9e63-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e63-121">Request headers</span></span>

| <span data-ttu-id="c9e63-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c9e63-122">Name</span></span>          | <span data-ttu-id="c9e63-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9e63-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c9e63-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9e63-124">Authorization</span></span> | <span data-ttu-id="c9e63-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9e63-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9e63-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e63-127">Request body</span></span>

<span data-ttu-id="c9e63-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9e63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e63-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9e63-129">Response</span></span>

<span data-ttu-id="c9e63-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9e63-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9e63-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9e63-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="c9e63-132">Exemplo 1: obter as propriedades padrão de uma conexão local</span><span class="sxs-lookup"><span data-stu-id="c9e63-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="c9e63-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e63-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

#### <a name="response"></a><span data-ttu-id="c9e63-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9e63-134">Response</span></span>

<span data-ttu-id="c9e63-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9e63-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "healthCheckStatus": "running",
    "inUse": false
  }
}
```

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="c9e63-136">Exemplo 2: obter as propriedades selecionadas de uma conexão local, incluindo healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="c9e63-136">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="c9e63-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9e63-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,subscriptionId,subscriptionName,adDomainName,adDomainUsername,organizationalUnit,virtualNetworkId,subnetId,healthCheckStatus,healthCheckStatusDetails,inUse
```

#### <a name="response"></a><span data-ttu-id="c9e63-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9e63-138">Response</span></span>

<span data-ttu-id="c9e63-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9e63-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
