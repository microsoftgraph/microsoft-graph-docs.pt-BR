---
title: Tipo de recurso windowsDeliveryOptimizationConfiguration
description: Windows Configuração de Otimização de Entrega
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d2154971f5691fd07e8ff6690db7a26a4a76d6c8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58815628"
---
# <a name="windowsdeliveryoptimizationconfiguration-resource-type"></a>Tipo de recurso windowsDeliveryOptimizationConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Configuração de Otimização de Entrega


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsDeliveryOptimizationConfigurations](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-list.md)|[Coleção windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Listar propriedades e relações dos [objetos windowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|
|[Obter windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-get.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Leia propriedades e relações do [objeto windowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|
|[Criar windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-create.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Crie um novo [objeto windowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|
|[Excluir windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-delete.md)|Nenhum|Exclui um [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).|
|[Atualizar windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-update.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Atualize as propriedades de um [objeto windowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Especifica o método de download que a otimização de entrega pode usar para gerenciar o consumo de largura de banda de rede para cenários de distribuição de conteúdo grandes. Os valores possíveis são: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|restrictPeerSelectionBy|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|Especifica restringir a seleção de pares por meio da opção selecionada.
A opção 1 (máscara de sub-rede) só se aplica aos modos de Otimização de Entrega LAN (1) e Grupo (2). Os valores possíveis são: `notConfigured` e `subnetMask`.|
|groupIdSource|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|Especifica restringir a seleção de pares a uma fonte especfic.
As opções definidas nesta política aplicam-se apenas ao modo de download do Modo de Otimização de Entrega (2). Se Group (2) não estiver definido como modo de download, essa política será ignorada. Para a opção 3 - ID da opção DHCP, o cliente consultará a ID da Opção DHCP 234 e usará o valor GUID retornado como a ID do Grupo.|
|bandwidthMode|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|Especifica o uso da largura de banda em primeiro plano e em segundo plano usando porcentagens, absolutos ou horas.|
|backgroundDownloadFromHttpDelayInSeconds|Int64|Especifica o número de segundos para atrasar uma fonte HTTP em um download em segundo plano que tem permissão para usar ponto a ponto. Valores válidos de 0 a 4294967295|
|foregroundDownloadFromHttpDelayInSeconds|Int64|Especifica o número de segundos para atrasar uma fonte HTTP em um download em primeiro plano que tem permissão para usar ponto a ponto (0-86400). Valores válidos de 0 a 86400
A especificação 0 define a Otimização de Entrega para gerenciar essa configuração usando o serviço de nuvem. Valores válidos de 0 a 86400|
|minimumRamAllowedToPeerInGigabytes|Int32|Especifica o tamanho mínimo de RAM em GB para usar o par Caching (1-100000). Valores válidos de 1 a 100000|
|minimumDiskSizeAllowedToPeerInGigabytes|Int32|Especifica o tamanho mínimo do disco em GB para usar o par Caching (1-100000). Valores válidos de 1 a 100000
Valores recomendados: 64 GB a 256 GB. Valores válidos de 1 a 100000|
|minimumFileSizeToCacheInMegabytes|Int32|Especifica o tamanho mínimo de arquivo de conteúdo em MB habilitado para usar o par Caching (1-100000). Valores válidos de 1 a 100000
Valores recomendados: 1 MB a 100.000 MB. Valores válidos de 1 a 100000|
|minimumBatteryPercentageAllowedToUpload|Int32|Especifica a porcentagem mínima de bateria para permitir que o dispositivo carregue dados (0-100). Valores válidos de 0 a 100
O valor padrão é 0. O valor 0 (zero) significa "não limitado" e o valor padrão do serviço de nuvem será usado. Valores válidos de 0 a 100|
|modifyCacheLocation|Cadeia de caracteres|Especifica a unidade que a Otimização de Entrega deve usar para seu cache.|
|maximumCacheAgeInDays|Int32|Especifica o tempo máximo em dias em que cada arquivo é mantido no cache de Otimização de Entrega após o download com êxito (0-3650). Valores válidos de 0 a 3650|
|maximumCacheSize|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|Especifica o tamanho máximo de cache que a Otimização de Entrega como porcentagem ou em GB.|
|vpnPeerCaching|[enablement](../resources/intune-shared-enablement.md)|Especifica se o dispositivo tem permissão para participar do Peer Caching enquanto estiver conectado via VPN à rede de domínio. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|cacheServerHostNames|Coleção de cadeias de caracteres|Especifica nomes de host de servidores de cache.|
|cacheServerForegroundDownloadFallbackToHttpDelayInSeconds|Int32|Especifica o número de segundos para atrasar um retorno de servidores de cache para uma fonte HTTP para um download em primeiro plano. Valores válidos de 0 a 2592000.|
|cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds|Int32|Especifica o número de segundos para atrasar um retorno de servidores de cache para uma fonte HTTP para um download em segundo plano. Valores válidos de 0 a 2592000.|

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
  "@odata.type": "microsoft.graph.windowsDeliveryOptimizationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "String",
  "restrictPeerSelectionBy": "String",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 1024,
  "foregroundDownloadFromHttpDelayInSeconds": 1024,
  "minimumRamAllowedToPeerInGigabytes": 1024,
  "minimumDiskSizeAllowedToPeerInGigabytes": 1024,
  "minimumFileSizeToCacheInMegabytes": 1024,
  "minimumBatteryPercentageAllowedToUpload": 1024,
  "modifyCacheLocation": "String",
  "maximumCacheAgeInDays": 1024,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "String",
  "cacheServerHostNames": [
    "String"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 1024,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 1024
}
```



