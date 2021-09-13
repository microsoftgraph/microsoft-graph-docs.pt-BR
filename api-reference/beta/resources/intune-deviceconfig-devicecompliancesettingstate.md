---
title: Tipo de recurso deviceComplianceSettingState
description: Estado de configuração de conformidade de um determinado dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c06fe23ed2ec900c97c898e3f0958ef6a731905d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120182"
---
# <a name="devicecompliancesettingstate-resource-type"></a>Tipo de recurso deviceComplianceSettingState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de configuração de conformidade de um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceSettingStates](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|Conjunto [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Listar propriedades e relações de objetos de [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Obter deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Ler propriedades e relações de objetos de [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Criar deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Criar um novo objeto de[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Excluir deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|Nenhum|Excluir [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).|
|[Atualizar deviceComplianceSettingState](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|Atualizar as propriedades de um objeto de [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objeto.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade|
|platformType|[deviceType](../resources/intune-deviceconfig-devicetype.md)|Tipo de plataforma de dispositivo. Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` .|
|configuração|Cadeia de caracteres|O nome da classe de configuração e o nome da propriedade.|
|settingName|Cadeia de caracteres|O nome da configuração sendo relatada|
|deviceId|Cadeia de caracteres|A ID do dispositivo sendo relatada|
|deviceName|Cadeia de caracteres|O nome do dispositivo sendo relatado|
|userId|Cadeia de caracteres|A ID do usuário sendo relatada|
|userEmail|Cadeia de caracteres|O endereço de email do usuário que está sendo relatado|
|userName|Cadeia de caracteres|O nome de usuário que está sendo relatado|
|userPrincipalName|Cadeia de caracteres|O PrincipalName do usuário que está sendo relatado|
|deviceModel|Cadeia de caracteres|O modelo do dispositivo que está sendo relatado|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|O estado de conformidade da configuração. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|DateTime em que o período de cortesia de conformidade do dispositivo termina|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



