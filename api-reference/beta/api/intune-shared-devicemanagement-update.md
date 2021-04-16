---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80f5fc4065d8db2f0bbb7659f244a14c9ef9331d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867522"
---
# <a name="update-devicemanagement"></a>Atualizar deviceManagement

Namespace: microsoft.graph

> **Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).

## <a name="prerequisites"></a>Pré-requisitos

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Observe que a permissão varia de acordo com o fluxo de trabalho.

| Tipo &nbsp; de &nbsp; permissão (por fluxo de &nbsp; trabalho) | Permissões (de privilégios máximos a mínimos) |
|:---|:---|
| Delegada (conta corporativa ou de estudante) ||
| &nbsp;&nbsp; **Android for Work** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **Auditoria** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Termos da empresa** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Configuração do dispositivo** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Intenção do dispositivo** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **SIM Eletrônico** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Inscrição** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Esgrima** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Notificação** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Integração** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp; &nbsp; **Acesso remoto** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Assistência remota** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Atualização de Software** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Proteção de Informações do Windows** | DeviceManagementApps.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte.|
| Application ||
| &nbsp;&nbsp; **Android for Work** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **Auditoria** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **Termos da empresa** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Configuração do dispositivo** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Intenção do dispositivo** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp; &nbsp; **Gerenciamento de dispositivo** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **SIM Eletrônico** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **Inscrição** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Esgrima** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **Notificação** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Integração** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp; &nbsp; **Acesso remoto** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Assistência remota** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Atualização de Software** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Proteção de Informações do Windows** | DeviceManagementApps.ReadWrite.All |

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
|intuneAccountId|GUID|ID da conta do Intune para determinado locatário|
|legacyPcManangementEnabled|Boolean|A propriedade para habilitar o gerenciamento de computador herdado não-MDM gerenciado para essa conta. Essa propriedade é somente leitura.|
|maximumDepTokens|Int32|Número máximo de tokens DEP permitidos por locatário.|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|Configurações de nível da conta.|
|**Gerenciamento de dispositivo**|
|accountMoveCompletionDateTime|DateTimeOffset|A data & hora em que os dados do locatário foram movidos entre as unidades de escala.|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|Informações de consentimento do administrador.|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|Visão geral da proteção do dispositivo.|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|Regra de limpeza de dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|assinaturas|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|Assinatura do locatário. Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Visão geral do malware para dispositivos windows.|
|**Integração**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

O suporte à propriedade request body varia de acordo com o fluxo de trabalho.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Veja um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:

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

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.

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










