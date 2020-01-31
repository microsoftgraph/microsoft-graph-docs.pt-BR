---
title: tipo de recurso managedDeviceMobileAppConfigurationState
description: Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3faa3547af9337483f0ded1306e7a64321d345a6
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636012"
---
# <a name="manageddevicemobileappconfigurationstate-resource-type"></a>tipo de recurso managedDeviceMobileAppConfigurationState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationStates](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-list.md)|coleção [managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Listar Propriedades e relações dos objetos [managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|
|[Obter managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-get.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|
|[Criar managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-create.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Criar um novo objeto [managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|
|[Excluir managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-delete.md)|Nenhum|Exclui [managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md).|
|[Atualizar managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-update.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Atualiza as propriedades de um objeto [managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|settingStates|coleção [managedDeviceMobileAppConfigurationSettingState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationSettingState.md)|**TODO: Adicione descrição.**|
|displayName|Cadeia de caracteres|O nome da política dessa policyBase|
|versão|Int32|A versão da política|
|platformType|[policyPlatformType](../resources/intune-shared-policyPlatformType.md)|Tipo de plataforma ao qual a política se aplica. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|state|[complianceStatus](../resources/intune-shared-complianceStatus.md)|O estado de conformidade da política. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|Contagem de quantas configurações uma política contém|
|userId|String|O identificador exclusivo do usuário deve ser GUID|
|userPrincipalName|String|Nome UPN|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024,
  "userId": "String",
  "userPrincipalName": "String"
}
```

