---
title: Tipo de recurso deviceCompliancePolicySettingStateSummary
description: Resumo de estado de configuração de política de conformidade do dispositivo por toda a conta.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89cbf2bb8df1ae24917d03c2b4c4535da76be094
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780410"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>Tipo de recurso deviceCompliancePolicySettingStateSummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo de estado de configuração de política de conformidade do dispositivo por toda a conta.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicySettingStateSummaries](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|Conjunto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Listar propriedades e relações de objetos de [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Acessar deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Leia as propriedades e as relações do objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Criar deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Crie um novo objeto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Excluir deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|Nenhum|Excluir [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Atualizar deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Atualizar as propriedades de um objeto de [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|configuração|Cadeia de caracteres|O nome da classe de configuração e o nome da propriedade.|
|settingName|Cadeia de caracteres|Nome da configuração.|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Configuração de plataforma. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|unknownDeviceCount|Int32|Número de dispositivos desconhecidos|
|notApplicableDeviceCount|Int32|Número de dispositivos não aplicáveis|
|compliantDeviceCount|Int32|Número de dispositivos em conformidade|
|remediatedDeviceCount|Int32|Número de dispositivos corrigidos|
|nonCompliantDeviceCount|Int32|Número de dispositivos sem conformidade|
|errorDeviceCount|Int32|Número de dispositivos com erro|
|conflictDeviceCount|Int32|Número de dispositivos em conflito|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceComplianceSettingStates|Conjunto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Ainda não documentado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





