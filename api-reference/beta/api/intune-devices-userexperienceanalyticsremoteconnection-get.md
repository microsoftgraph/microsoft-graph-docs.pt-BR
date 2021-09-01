---
title: Obter userExperienceAnalyticsRemoteConnection
description: Leia propriedades e relações do objeto userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd80b3ac077b086e2cb49af8824cf6aac5b3ac27
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58798592"
---
# <a name="get-userexperienceanalyticsremoteconnection"></a>Obter userExperienceAnalyticsRemoteConnection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia propriedades e relações do [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/{userExperienceAnalyticsRemoteConnectionId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
    "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "model": "Model value",
    "virtualNetwork": "Virtual Network value",
    "manufacturer": "Manufacturer value",
    "deviceCount": 11,
    "cloudPcRoundTripTime": 6.666666666666667,
    "cloudPcSignInTime": 5.666666666666667,
    "remoteSignInTime": 5.333333333333333,
    "coreBootTime": 4.0,
    "coreSignInTime": 4.666666666666667,
    "cloudPcFailurePercentage": 8.0,
    "userPrincipalName": "User Principal Name value"
  }
}
```



