---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d8465ee45a2a6c23dedc4fe049ef1f73bb25218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924689"
---
# <a name="update-devicemanagement"></a>Atualizar deviceManagement

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Pré-requisitos

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Observe que a permissão varia de acordo com o fluxo de trabalho.

| Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho) | Permissões (de privilégios máximos a mínimos) |
|:---|:---|
| Delegado (conta corporativa ou de estudante) ||
| &nbsp;&nbsp; **Android para o trabalho** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp;&nbsp; **Auditoria** | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; **Termos da empresa** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Configuração do dispositivo** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **SIM eletrônico** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Registro** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Fencing** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Notificação** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Onboarding** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; **Acesso remoto** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Assistência remota** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **a solução de problemas** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Proteção de informações do Windows** | DeviceManagementApps.ReadWrite.All |
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
|id|Cadeia de caracteres|Identificador exclusivo do dispositivo.|
|**Configuração do dispositivo**|
|intuneAccountId|GUID|ID da conta Intune para dado locatário|
|legacyPcManangementEnabled|Booliano|A propriedade habilitem Non-MDM gerenciados herdado gerenciamento de PC para essa conta. Esta propriedade é somente leitura.|
|maximumDepTokens|Int32|Número máximo de tokens DEP permitido por locatário.|
|configurações|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivos**|
|accountMoveCompletionDateTime|DateTimeOffset|A data hora & ao mover os dados de inquilinos entre scaleunits.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informações de consentimento do administrador.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Visão geral de proteção do dispositivo.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regra de limpeza do dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|assinaturas|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Assinatura de locatário. Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Visão geral de malware para dispositivos do windows.|
|**Inclusão**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

Suporte de propriedade de corpo de solicitação varia de acordo com o fluxo de trabalho.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Aqui está um exemplo de uma solicitação seguindo o fluxo de trabalho de gerenciamento de dispositivo:

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

Veja a seguir um exemplo da resposta. 

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Propriedades retornadas variam de acordo com o fluxo de trabalho e contexto.

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



