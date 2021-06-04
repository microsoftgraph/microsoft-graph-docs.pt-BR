---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7fccbc17390e9cd481c2fd06af09ba5681a1e56
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732288"
---
# <a name="get-devicemanagement"></a>Acessar deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo &nbsp; de &nbsp; permissão (por fluxo de &nbsp; trabalho) | Permissões (de privilégios máximos a mínimos) |
|:---|:---|
| Delegado (conta corporativa ou de estudante) | |
| &nbsp;&nbsp;Auditoria | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp;&nbsp;Termos da empresa | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;Configuração do dispositivo | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp;Gerenciamento de dispositivos | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp;Inscrição | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;Notificação | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;Integração | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;RBAC | DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All |
| &nbsp;&nbsp;Assistência remota | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;Gerenciamento de despesas de telecomunicações | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp;Solução de problemas | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
| &nbsp;&nbsp;Windows Proteção de Informações | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
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
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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