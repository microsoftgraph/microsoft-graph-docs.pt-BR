---
title: Tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevice
description: O relatório de análise de experiência do usuário Dispositivo para trabalho em qualquer lugar
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f9f5e5f6bc8ff43a3bac407858c1d41ff06f27d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255575"
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
  "osCheckFailed": true
}
```




