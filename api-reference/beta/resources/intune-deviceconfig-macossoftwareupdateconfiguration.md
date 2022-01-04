---
title: Tipo de recurso macOSSoftwareUpdateConfiguration
description: Configuração de Atualização de Software MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 642e33528c7beb29e4d7a4c65b281dc470e06a6e
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711960"
---
# <a name="macossoftwareupdateconfiguration-resource-type"></a>Tipo de recurso macOSSoftwareUpdateConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de Atualização de Software MacOS


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSSoftwareUpdateConfigurations](../api/intune-deviceconfig-macossoftwareupdateconfiguration-list.md)|[Coleção macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Listar propriedades e relações dos [objetos macOSSoftwareUpdateConfiguration.](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|
|[Obter macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-get.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Leia propriedades e relações do [objeto macOSSoftwareUpdateConfiguration.](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|
|[Criar macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-create.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Crie um novo [objeto macOSSoftwareUpdateConfiguration.](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|
|[Excluir macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-delete.md)|Nenhum|Exclui um [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md).|
|[Atualizar macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-update.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|Atualize as propriedades de [um objeto macOSSoftwareUpdateConfiguration.](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|criticalUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Atualize o comportamento para atualizações críticas. Os possíveis valores são: `notConfigured`, `default`, `downloadOnly`, `installASAP`, `notifyOnly`, `installLater`.|
|configDataUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Atualizar comportamento para atualizações de arquivo de dados de configuração. Os possíveis valores são: `notConfigured`, `default`, `downloadOnly`, `installASAP`, `notifyOnly`, `installLater`.|
|firmwareUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Comportamento de atualização para atualizações de firmware. Os possíveis valores são: `notConfigured`, `default`, `downloadOnly`, `installASAP`, `notifyOnly`, `installLater`.|
|allOtherUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|Atualize o comportamento de todas as outras atualizações. Os possíveis valores são: `notConfigured`, `default`, `downloadOnly`, `installASAP`, `notifyOnly`, `installLater`.|
|updateScheduleType|[macOSSoftwareUpdateScheduleType](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|Atualizar tipo de agendamento. Os valores possíveis são: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.|
|customUpdateTimeWindows|[Coleção customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md)|Janelas de tempo personalizadas quando as atualizações serão permitidas ou bloqueadas. Essa coleção pode conter no máximo 20 elementos.|
|updateTimeWindowUtcOffsetInMinutes|Int32|Minutos indicando deslocamento UTC para cada janela de tempo de atualização|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação de configuração do dispositivo pelo usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "criticalUpdateBehavior": "String",
  "configDataUpdateBehavior": "String",
  "firmwareUpdateBehavior": "String",
  "allOtherUpdateBehavior": "String",
  "updateScheduleType": "String",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "String",
      "endDay": "String",
      "startTime": "String (time of day)",
      "endTime": "String (time of day)"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 1024
}
```




