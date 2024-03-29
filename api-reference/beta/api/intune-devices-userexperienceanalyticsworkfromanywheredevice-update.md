---
title: Atualizar userExperienceAnalyticsWorkFromAnywhereDevice
description: Atualize as propriedades de um objeto userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9afde8adaf2baf8e91b57c40ad48af68c077114
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344705"
---
# <a name="update-userexperienceanalyticsworkfromanywheredevice"></a>Atualizar userExperienceAnalyticsWorkFromAnywhereDevice

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da análise de experiência do usuário funciona em qualquer dispositivo.|
|deviceId|Cadeia de caracteres|A experiência do usuário funciona a partir de qualquer ID do dispositivo.|
|deviceName|String|O trabalho do nome do dispositivo em qualquer lugar.|
|serialNumber|String|A experiência do usuário funciona de qualquer lugar do número de série do dispositivo.|
|fabricante|String|A experiência do usuário funciona de qualquer fabricante do dispositivo.|
|modelo|String|A experiência do usuário funciona de qualquer lugar do modelo do dispositivo.|
|propriedade|String|A experiência do usuário funciona de qualquer lugar da propriedade do dispositivo.|
|managedBy|String|A experiência do usuário funciona de qualquer lugar do agente de gerenciamento do dispositivo.|
|autoPilotRegistered|Boolean|A experiência do usuário funciona em qualquer lugar do piloto automático do dispositivo intuneRegistered.|
|autoPilotProfileAssigned|Boolean|A análise da experiência do usuário funciona em qualquer lugar do autopilotProfileAssigned do dispositivo intune.|
|azureAdRegistered|Boolean|A experiência do usuário funciona de qualquer lugar do dispositivo azureAdRegistered.|
|azureAdDeviceId|String|A experiência do usuário funciona em qualquer lugar do Azure Ad device Id.|
|azureAdJoinType|String|A experiência do usuário funciona de qualquer lugar do azure Ad joinType do dispositivo.|
|osDescription|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar da Descrição do sistema operacional do dispositivo.|
|osVersion|String|A experiência do usuário funciona de qualquer lugar da versão do sistema operacional do dispositivo.|
|tenantAttached|Boolean|A experiência do usuário funciona de qualquer locatário do dispositivoAttached.|
|compliancePolicySetToIntune|Booliano|A experiência do usuário funciona de qualquer lugar do dispositivo compliancePolicySetToIntune.|
|otherWorkloadsSetToIntune|Boolean|A experiência do usuário funciona de qualquer outro dispositivoWorkloadsSetToIntune.|
|isCloudManagedGatewayEnabled|Booliano|A experiência do usuário funciona em qualquer lugar que o Gateway de Gerenciamento de Nuvem do dispositivo para o Configuration Manager está habilitado.|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|A experiência do usuário funciona em qualquer lugar do windows upgrade status de qualificação do dispositivo. Os valores possíveis são: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Booliano|A análise da experiência do usuário funciona em qualquer lugar que a verificação de hardware ram do dispositivo falhou para que o dispositivo atualize para a versão mais recente do windows|
|storageCheckFailed|Booliano|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de hardware de armazenamento para que o dispositivo atualize para a versão mais recente do windows.|
|processorCoreCountCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na contagem de núcleos de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|processorSpeedCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de velocidade de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|tpmCheckFailed|Booliano|A experiência do usuário funciona de qualquer dispositivo, falha na verificação de hardware do Módulo de Plataforma Confiável (TPM) para o dispositivo para a versão mais recente da atualização para windows.|
|secureBootCheckFailed|Booliano|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de hardware de inicialização segura para que o dispositivo atualize para a versão mais recente do windows.|
|processorFamilyCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação da família de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|processor64BitCheckFailed|Booliano|A experiência do usuário funciona de qualquer dispositivo, a verificação de arquitetura de hardware de 64 bits do processador falhou para que o dispositivo atualize para a versão mais recente do windows.|
|osCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, falha na verificação do sistema operacional para que o dispositivo atualize para a versão mais recente do windows.|
|workFromAnywhereScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação geral do dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|windowsScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação do windows do dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudManagementScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação de gerenciamento de nuvem de dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudIdentityScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação de identidade na nuvem do dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudProvisioningScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação de provisionamento de nuvem de dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|A experiência do usuário funciona de qualquer lugar por status de saúde do dispositivo. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
Content-type: application/json
Content-length: 1323

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "isCloudManagedGatewayEnabled": true,
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "workFromAnywhereScore": 7.0,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1372

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "isCloudManagedGatewayEnabled": true,
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "workFromAnywhereScore": 7.0,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```




