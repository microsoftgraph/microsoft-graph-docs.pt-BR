---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f265c4e8665d607b1bed87e7c61949131877fa99
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732291"
---
# <a name="update-devicemanagement"></a>Atualizar deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo &nbsp; de &nbsp; permissão (por fluxo de &nbsp; trabalho) | Permissões (de privilégios máximos a mínimos) |
|:---|:---|
| Delegado (conta corporativa ou de estudante) |
| &nbsp;&nbsp;Auditoria | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp;Termos da empresa | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;Registro corporativo | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp;&nbsp;Configuração do dispositivo | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;Gerenciamento de dispositivos | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;Proteção de ponto de extremidade | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;Notificação | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;Integração | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;Controle de acesso baseado em função | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp;Assistência remota | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;Gerenciamento de despesas de telecomunicações | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;Solução de problemas | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;Windows Proteção de Informações | DeviceManagementApps.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.|
| Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo|
|**Configuração do dispositivo**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivo**|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Integração**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

O suporte à propriedade request body varia de acordo com o fluxo de trabalho.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```









