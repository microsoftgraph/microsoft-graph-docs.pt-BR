---
title: Criar userExperienceAnalyticsWorkFromAnywhereDevice
description: Crie um novo objeto userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0031a5596d660bab7a10aca9f47d3172a0f4b23
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263258"
---
# <a name="create-userexperienceanalyticsworkfromanywheredevice"></a>Criar userExperienceAnalyticsWorkFromAnywhereDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsWorkFromAnywhereDevice.

A tabela a seguir mostra as propriedades necessárias ao criar o userExperienceAnalyticsWorkFromAnywhereDevice.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da análise de experiência do usuário funciona em qualquer dispositivo.|
|deviceName|String|O trabalho do nome do dispositivo em qualquer lugar.|
|serialNumber|String|A experiência do usuário funciona de qualquer lugar do número de série do dispositivo.|
|fabricante|String|A experiência do usuário funciona de qualquer fabricante do dispositivo.|
|modelo|String|A experiência do usuário funciona de qualquer lugar do modelo do dispositivo.|
|propriedade|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar da propriedade do dispositivo.|
|managedBy|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar do agente de gerenciamento do dispositivo.|
|autoPilotRegistered|Boolean|A experiência do usuário funciona em qualquer lugar do piloto automático do dispositivo intuneRegistered.|
|autoPilotProfileAssigned|Boolean|A análise da experiência do usuário funciona em qualquer lugar do autopilotProfileAssigned do dispositivo intune.|
|azureAdRegistered|Boolean|A experiência do usuário funciona de qualquer lugar do dispositivo azureAdRegistered.|
|azureAdDeviceId|Cadeia de caracteres|A experiência do usuário funciona em qualquer lugar do Azure Ad device Id.|
|azureAdJoinType|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar do azure Ad joinType do dispositivo.|
|osDescription|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar da Descrição do sistema operacional do dispositivo.|
|osVersion|String|A experiência do usuário funciona de qualquer lugar da versão do sistema operacional do dispositivo.|
|tenantAttached|Boolean|A experiência do usuário funciona de qualquer locatário do dispositivoAttached.|
|compliancePolicySetToIntune|Boolean|A experiência do usuário funciona de qualquer lugar do dispositivo compliancePolicySetToIntune.|
|otherWorkloadsSetToIntune|Boolean|A experiência do usuário funciona de qualquer outro dispositivoWorkloadsSetToIntune.|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|A experiência do usuário funciona em qualquer lugar do windows upgrade status de qualificação do dispositivo. Os valores possíveis são: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Boolean|A análise da experiência do usuário funciona em qualquer lugar que a verificação de hardware ram do dispositivo falhou para que o dispositivo atualize para a versão mais recente do windows|
|storageCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de hardware de armazenamento para que o dispositivo atualize para a versão mais recente do windows.|
|processorCoreCountCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na contagem de núcleos de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|processorSpeedCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de velocidade de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|tpmCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, falha na verificação de hardware do Módulo de Plataforma Confiável (TPM) para o dispositivo para a versão mais recente da atualização para windows.|
|secureBootCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de hardware de inicialização segura para que o dispositivo atualize para a versão mais recente do windows.|
|processorFamilyCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação da família de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|processor64BitCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, a verificação de arquitetura de hardware de 64 bits do processador falhou para que o dispositivo atualize para a versão mais recente do windows.|
|osCheckFailed|Boolean|A experiência do usuário funciona de qualquer dispositivo, falha na verificação do sistema operacional para que o dispositivo atualize para a versão mais recente do windows.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
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
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
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
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true
}
```




