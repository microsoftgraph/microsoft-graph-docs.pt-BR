---
title: Tipo de recurso advancedThreatProtectionOnboardingDeviceSettingState
description: Estado de integração do ATP para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17e71bb9551c1dcc413ab4101c9ede980b0e1fac
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669830"
---
# <a name="advancedthreatprotectiononboardingdevicesettingstate-resource-type"></a>Tipo de recurso advancedThreatProtectionOnboardingDeviceSettingState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de integração do ATP para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar advancedThreatProtectionOnboardingDeviceSettingStates](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-list.md)|[coleção advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Listar propriedades e relações dos [objetos advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .|
|[Obter advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-get.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Ler propriedades e relações do [objeto advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .|
|[Criar advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-create.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Crie um novo [objeto advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .|
|[Excluir advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-delete.md)|Nenhum|Exclui um [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).|
|[Atualizar advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-update.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Atualize as propriedades de [um objeto advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade|
|platformType|[Devicetype](../resources/intune-deviceconfig-devicetype.md)|Tipo de plataforma de dispositivo. Os valores possíveis são: , , , , , , , `winCE`, `iPod``cloudPC``palm``macMDM``blackberry``unix``linux``iSocConsumer``unknown``windows10x``androidnGMS``iPad``chromeOS``androidEnterprise``androidForWork``surfaceHub``holoLens``android``iPhone``winEmbedded`. `windowsPhone``mac``nokia``winMO6``windowsRT``desktop`|
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
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
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




