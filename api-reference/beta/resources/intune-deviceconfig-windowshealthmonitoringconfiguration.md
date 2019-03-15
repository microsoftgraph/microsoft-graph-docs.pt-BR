---
title: tipo de recurso windowsHealthMonitoringConfiguration
description: Configuração de monitoramento de integridade do dispositivo Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bd9b1e16a33a68048f347fba100d290a7d9d849
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631450"
---
# <a name="windowshealthmonitoringconfiguration-resource-type"></a>tipo de recurso windowsHealthMonitoringConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de monitoramento de integridade do dispositivo Windows


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsHealthMonitoringConfigurations](../api/intune-deviceconfig-windowshealthmonitoringconfiguration-list.md)|coleção [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)|Listar Propriedades e relações dos objetos [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .|
|[Obter windowsHealthMonitoringConfiguration](../api/intune-deviceconfig-windowshealthmonitoringconfiguration-get.md)|[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)|Leia as propriedades e as relações do objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .|
|[Criar windowsHealthMonitoringConfiguration](../api/intune-deviceconfig-windowshealthmonitoringconfiguration-create.md)|[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)|Criar um novo objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .|
|[Excluir windowsHealthMonitoringConfiguration](../api/intune-deviceconfig-windowshealthmonitoringconfiguration-delete.md)|Nenhum|Exclui [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).|
|[Atualizar windowsHealthMonitoringConfiguration](../api/intune-deviceconfig-windowshealthmonitoringconfiguration-update.md)|[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)|Atualiza as propriedades de um objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|allowDeviceHealthMonitoring|[habilitação](../resources/intune-shared-enablement.md)|Habilita o monitoramento de integridade do dispositivo no dispositivo. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|configDeviceHealthMonitoringScope|[windowsHealthMonitoringScope](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|Especifica conjunto de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado. Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHealthMonitoringConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "allowDeviceHealthMonitoring": "String",
  "configDeviceHealthMonitoringScope": "String"
}
```




