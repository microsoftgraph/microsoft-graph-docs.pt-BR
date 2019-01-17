---
title: iosUpdateConfiguration resource type
description: A Configuração de Atualização do iOS permite que você configure a janela de tempo na semana para instalar atualizações do iOS
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 3b7abc49e5e4098323b4461612676fdce9bb6aef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982194"
---
# <a name="iosupdateconfiguration-resource-type"></a>iosUpdateConfiguration resource type

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A Configuração de Atualização do iOS permite que você configure a janela de tempo na semana para instalar atualizações do iOS

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosUpdateConfigurations](../api/intune-deviceconfig-iosupdateconfiguration-list.md)|Coleção [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|Lista propriedades e relações dos objetos [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).|
|[Obter iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-get.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|Propriedades de leitura e relações do objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).|
|[Criar iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-create.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|Cria um novo objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).|
|[Excluir iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-delete.md)|Nenhum|Exclui um [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).|
|[Atualizar iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-update.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|Atualiza as propriedades de um objeto [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|isEnabled|Boolean|Configuração estiver habilitada na interface do usuário|
|activeHoursStart|TimeOfDay|Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)|
|activeHoursEnd|TimeOfDay|Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)|
|scheduledInstallDays|coleção [dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Dias na semana para os quais o horário ativo está configurado. Essa coleção pode conter um máximo de 7 elementos.|
|utcTimeOffsetInMinutes|Int32|Deslocamento do horário UTC indicado em minutos|
|enforcedSoftwareUpdateDelayInDays|Int32|Dias antes de atualizações de software estão visíveis para os dispositivos iOS que varia de 0 a 90 inclusive|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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
  "isEnabled": true,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024,
  "enforcedSoftwareUpdateDelayInDays": 1024
}
```





