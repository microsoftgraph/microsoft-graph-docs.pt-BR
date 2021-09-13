---
title: Tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevice
description: O relatório de análise de experiência do usuário Dispositivo para trabalho em qualquer lugar
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae621a500d0b3cef0151ccf2763aa78db182ed67
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046873"
---
# <a name="userexperienceanalyticsworkfromanywheredevice-resource-type"></a>Tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O relatório de análise de experiência do usuário Dispositivo para trabalho em qualquer lugar

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsWorkFromAnywhereDevices](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-list.md)|[Coleção userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Obter userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-get.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Criar userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-create.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Crie um novo [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Excluir userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).|
|[Atualizar userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-update.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da análise de experiência do usuário funciona em qualquer dispositivo.|
|deviceName|String|O trabalho do nome do dispositivo em qualquer lugar.|
|serialNumber|String|A experiência do usuário funciona de qualquer lugar do número de série do dispositivo.|
|fabricante|String|A experiência do usuário funciona de qualquer fabricante do dispositivo.|
|modelo|String|A experiência do usuário funciona de qualquer lugar do modelo do dispositivo.|
|propriedade|Cadeia de Caracteres|A experiência do usuário funciona de qualquer lugar da propriedade do dispositivo.|
|managedBy|Cadeia de Caracteres|A experiência do usuário funciona de qualquer lugar do agente de gerenciamento do dispositivo.|
|autoPilotRegistered|Boleano|A experiência do usuário funciona em qualquer lugar do piloto automático do dispositivo intuneRegistered.|
|autoPilotProfileAssigned|Boleano|A análise da experiência do usuário funciona em qualquer lugar do autopilotProfileAssigned do dispositivo intune.|
|azureAdRegistered|Boleano|A experiência do usuário funciona de qualquer lugar do dispositivo azureAdRegistered.|
|azureAdDeviceId|Cadeia de Caracteres|A experiência do usuário funciona em qualquer lugar do Azure Ad device Id.|
|azureAdJoinType|Cadeia de Caracteres|A experiência do usuário funciona de qualquer lugar do azure Ad joinType do dispositivo.|
|osDescription|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar da Descrição do sistema operacional do dispositivo.|
|osVersion|String|A experiência do usuário funciona de qualquer lugar da versão do sistema operacional do dispositivo.|
|tenantAttached|Boleano|A experiência do usuário funciona de qualquer locatário do dispositivoAttached.|
|compliancePolicySetToIntune|Boleano|A experiência do usuário funciona de qualquer lugar do dispositivo compliancePolicySetToIntune.|
|otherWorkloadsSetToIntune|Boleano|A experiência do usuário funciona de qualquer outro dispositivoWorkloadsSetToIntune.|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|A experiência do usuário funciona em qualquer lugar do windows upgrade status de qualificação do dispositivo. Os valores possíveis são: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Boleano|A análise da experiência do usuário funciona em qualquer lugar que a verificação de hardware ram do dispositivo falhou para que o dispositivo atualize para a versão mais recente do windows|
|storageCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de hardware de armazenamento para que o dispositivo atualize para a versão mais recente do windows.|
|processorCoreCountCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, Falha na contagem de núcleos de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|processorSpeedCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de velocidade de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|tpmCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, falha na verificação de hardware do Módulo de Plataforma Confiável (TPM) para o dispositivo para a versão mais recente da atualização para windows.|
|secureBootCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação de hardware de inicialização segura para que o dispositivo atualize para a versão mais recente do windows.|
|processorFamilyCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, Falha na verificação da família de hardware do processador para que o dispositivo atualize para a versão mais recente do windows.|
|processor64BitCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, a verificação de arquitetura de hardware de 64 bits do processador falhou para que o dispositivo atualize para a versão mais recente do windows.|
|osCheckFailed|Boleano|A experiência do usuário funciona de qualquer dispositivo, falha na verificação do sistema operacional para que o dispositivo atualize para a versão mais recente do windows.|
|windowsScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação do windows do dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudManagementScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação de gerenciamento de nuvem de dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudIdentityScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação de identidade na nuvem do dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudProvisioningScore|Duplo|A experiência do usuário funciona de qualquer lugar por pontuação de provisionamento de nuvem de dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|A experiência do usuário funciona de qualquer lugar por status de saúde do dispositivo. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String",
  "osDescription": "String",
  "osVersion": "String",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "upgradeEligibility": "String",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "windowsScore": "4.2",
  "cloudManagementScore": "4.2",
  "cloudIdentityScore": "4.2",
  "cloudProvisioningScore": "4.2",
  "healthStatus": "String"
}
```



