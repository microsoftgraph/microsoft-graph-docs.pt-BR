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
# <a name="get-cloudpconpremisesconnection"></a>Obter cloudPcOnPremisesConnection

Namespace: microsoft.graph

Leia as propriedades e as relações do objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão| Permissões (de privilégios máximos a mínimos) |
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC. ReadWrite. All, CloudPC. Read. All|
|Delegado (conta pessoal da Microsoft) | Sem suporte.|
|Aplicativo| Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a>Exemplo 1: obter as propriedades padrão de uma conexão local

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

#### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a>Exemplo 2: obter as propriedades selecionadas de uma conexão local, incluindo healthCheckStatusDetails

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,subscriptionId,subscriptionName,adDomainName,adDomainUsername,organizationalUnit,virtualNetworkId,subnetId,healthCheckStatus,healthCheckStatusDetails,inUse
```

#### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
