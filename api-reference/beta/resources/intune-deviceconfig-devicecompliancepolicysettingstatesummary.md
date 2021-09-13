---
title: Tipo de recurso deviceCompliancePolicySettingStateSummary
description: Resumo de estado de configuração de política de conformidade do dispositivo por toda a conta.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: faa2aee4a4e8118b3f4a5bc5cb861ac96b6db181
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023574"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>Tipo de recurso deviceCompliancePolicySettingStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo de estado de configuração de política de conformidade do dispositivo por toda a conta.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicySettingStateSummaries](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-list.md)|Conjunto [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Listar propriedades e relações de objetos de [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Obter deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Ler propriedades e relações de objetos de [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Criar deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-create.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Criar um novo objeto de [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Excluir deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-delete.md)|Nenhum|Excluir [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|
|[Atualizar deviceCompliancePolicySettingStateSummary](../api/intune-deviceconfig-devicecompliancepolicysettingstatesummary-update.md)|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)|Atualizar as propriedades de um objeto de [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|configuração|Cadeia de caracteres|O nome da classe de configuração e o nome da propriedade.|
|settingName|Cadeia de caracteres|Nome da configuração.|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Plataforma de configuração. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `androidAOSP`, `all`.|
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



