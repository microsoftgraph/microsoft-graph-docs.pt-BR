---
title: Get deviceManagement
description: Ler propriedades e relações do objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c00b60793209904ce184de25f12f1f4ad14fad1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862633"
---
# <a name="get-devicemanagement"></a>Get deviceManagement

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ler propriedades e relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Pré-requisitos

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho) | Permissões (de privilégios máximos a mínimos) |
|:---|:---|
| Delegado (conta corporativa ou de estudante) | |
| &nbsp;&nbsp; **Android para o trabalho** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Auditoria** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp;&nbsp; **Termos da empresa** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Configuração do dispositivo** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **SIM eletrônico** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Registro** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Fencing** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Notificação** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Onboarding** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All |
| &nbsp;&nbsp; **Acesso remoto** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Assistência remota** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Solução de problemas** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Proteção de informações do Windows** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.|
| Aplicativo | Sem suporte. |



## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a>Resposta

Eis um exemplo da resposta. 

Observação: Os objetos de resposta mostrados aqui podem estar truncados para fins de concisão.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

Propriedades apropriadas para o fluxo de trabalho são retornadas.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



