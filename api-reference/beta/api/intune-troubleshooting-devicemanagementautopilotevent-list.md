---
title: Listar deviceManagementAutopilotEvents
description: Listar Propriedades e relações dos objetos deviceManagementAutopilotEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 709fc30929119e42856f92a460944aaf4992d81a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199484"
---
# <a name="list-devicemanagementautopilotevents"></a>Listar deviceManagementAutopilotEvents

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar Propriedades e relações dos objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1501

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
      "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
      "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
      "enrollmentType": "azureADJoinedWithAutopilotProfile",
      "deviceSerialNumber": "Device Serial Number value",
      "managedDeviceName": "Managed Device Name value",
      "userPrincipalName": "User Principal Name value",
      "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
      "enrollmentState": "enrolled",
      "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
      "deploymentState": "success",
      "osVersion": "Os Version value",
      "deploymentDuration": "PT3M21.5549443S",
      "deploymentTotalDuration": "PT1M43.5284261S",
      "devicePreparationDuration": "-PT1M32.1347897S",
      "deviceSetupDuration": "-PT2M57.2190107S",
      "accountSetupDuration": "-PT2M32.0507894S",
      "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
      "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
      "targetedAppCount": 0,
      "targetedPolicyCount": 3,
      "enrollmentFailureDetails": "Enrollment Failure Details value"
    }
  ]
}
```




