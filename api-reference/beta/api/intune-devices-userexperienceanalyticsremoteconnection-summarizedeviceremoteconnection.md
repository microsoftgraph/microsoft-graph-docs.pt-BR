---
title: função summarizeDeviceRemoteConnection
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23053d4e61ad3f60fc2a4a7d8090d5c692d2f0eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445698"
---
# <a name="summarizedeviceremoteconnection-function"></a>função summarizeDeviceRemoteConnection

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|summarizeBy|[userExperienceAnalyticsSummarizedBy](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|Ainda não documentado|



## <a name="response"></a>Resposta
Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection(summarizeBy='parameterValue')
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
      "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "virtualNetwork": "Virtual Network value",
      "deviceCount": 11,
      "cloudPcRoundTripTime": 6.666666666666667,
      "cloudPcSignInTime": 5.666666666666667,
      "remoteSignInTime": 5.333333333333333,
      "coreBootTime": 4.0,
      "coreSignInTime": 4.666666666666667,
      "cloudPcFailurePercentage": 8.0
    }
  ]
}
```




