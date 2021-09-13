---
title: Tipo de recurso macOSDeviceFeaturesConfiguration
description: Perfil de configuração de recursos do dispositivo macOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9062bdce77c0dea983d61d9de5a668676c257bbe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091731"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a>Tipo de recurso macOSDeviceFeaturesConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração de recursos do dispositivo macOS.


Herda de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSDeviceFeaturesConfigurations](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-list.md)|Conjunto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Listar propriedades e relações de objetos de [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Obter macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-get.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Ler propriedades e relações de objetos de [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Criar macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-create.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Criar um novo objeto de [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Excluir macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-delete.md)|Nenhum|Excluir [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|
|[Atualizar macOSDeviceFeaturesConfiguration](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-update.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|Atualizar as propriedades de um objeto de [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|airPrintDestinations|[Coleção airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)|Uma matriz de impressoras AirPrint que sempre devem ser mostradas. Esta coleção pode conter um máximo de 500 elementos. Herdado [do appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)|
|autoLaunchItems|[Coleção macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)|Lista de aplicativos, arquivos, pastas e outros itens a iniciar quando o usuário faz login. Esta coleção pode conter um máximo de 500 elementos.|
|adminShowHostInfo|Boleano|Se deve mostrar informações do host do administrador na janela de logon.|
|loginWindowText|Cadeia de Caracteres|Texto personalizado a ser exibido na janela de logon.|
|authorizedUsersListHidden|Boleano|Se será exibida a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.|
|authorizedUsersListHideLocalUsers|Boleano|Se apenas os usuários da rede e do sistema na lista de usuários autorizados na janela de logon.|
|authorizedUsersListHideMobileAccounts|Boleano|Se deve ocultar usuários móveis na lista de usuários autorizados na janela de logon.|
|authorizedUsersListIncludeNetworkUsers|Boleano|Se deve mostrar usuários de rede na lista de usuários autorizados na janela de logon.|
|authorizedUsersListHideAdminUsers|Boleano|Se deve ocultar usuários de administrador na lista de usuários autorizados na janela de logon.|
|authorizedUsersListShowOtherManagedUsers|Boleano|Se deve mostrar outros usuários na lista de usuários autorizados na janela de logon.|
|shutDownDisabled|Boleano|Se deve ocultar o item do botão Desligar na janela de logon.|
|restartDisabled|Boleano|Se deve ocultar o item do botão Reiniciar na janela de logon.|
|sleepDisabled|Boleano|Se deve ocultar o item de menu Ental na janela de logon.|
|consoleAccessDisabled|Boleano|Se o outro usuário ignorará o uso do ' console>> nome de usuário especial.|
|shutDownDisabledWhileLoggedIn|Boleano|Se o item de menu Desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.|
|restartDisabledWhileLoggedIn|Boleano|Se o item de menu Reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.|
|powerOffDisabledWhileLoggedIn|Boleano|Se o item de menu Desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.|
|logOutDisabledWhileLoggedIn|Boleano|Se o item de menu Sair na janela de logon será desabilitado enquanto o usuário estiver conectado.|
|screenLockDisableImmediate|Boleano|Se desabilitar as funções imediatas de bloqueio de tela.|
|associatedDomains|Coleção [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|PRETERIDO: use appAssociatedDomains. Obtém ou define uma lista que mapeia aplicativos para seus domínios associados. A chave deve corresponder à ID do aplicativo e o valor deve ser uma cadeia de caracteres na forma de "service:domain" em que o domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example.com). Esta coleção pode conter um máximo de 500 elementos.|
|appAssociatedDomains|[Coleção macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)|Obtém ou define uma lista que mapeia aplicativos para seus domínios associados. Os identificadores de aplicativo devem ser exclusivos. Esta coleção pode conter um máximo de 500 elementos.|
|singleSignOnExtension|[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)|Obtém ou define um único perfil de extensão de entrada. Preterido: use MacOSSingleSignOnExtension.|
|macOSSingleSignOnExtension|[macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)|Obtém ou define um único perfil de extensão de entrada.|
|contentCachingEnabled|Boleano|Habilita o cache de conteúdo e impede que ele seja desabilitado pelo usuário.|
|contentCachingType|[macOSContentCachingType](../resources/intune-deviceconfig-macoscontentcachingtype.md)|Determina que tipo de conteúdo pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple. Os valores possíveis são: `notConfigured`, `userContentOnly`, `sharedContentOnly`.|
|contentCachingMaxSizeBytes|Int32|O número máximo de bytes de espaço em disco que será usado para o cache de conteúdo. Um valor 0 (padrão) indica espaço em disco ilimitado. |
|contentCachingDataPath|Cadeia de Caracteres|O caminho para o diretório usado para armazenar conteúdo armazenado em cache. O valor deve ser (ou terminar com) /Library/Application Support/Apple/AssetCache/Data|
|contentCachingDisableConnectionSharing|Boleano|Desabilita o compartilhamento de conexões com a Internet.|
|contentCachingForceConnectionSharing|Boleano|Força o compartilhamento de conexão com a Internet. contentCachingDisableConnectionSharing substitui essa configuração.|
|contentCachingClientPolicy|[macOSContentCachingClientPolicy](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|Determina o método no qual os servidores de cache de conteúdo escutarão clientes. Os valores possíveis são: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.|
|contentCachingClientListenRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Uma lista de caches de conteúdo de intervalos IP personalizados será usada para escutar clientes. Esta coleção pode conter um máximo de 500 elementos.|
|contentCachingPeerPolicy|[macOSContentCachingPeerPolicy](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|Determina o método no qual o conteúdo armazena o par de caches com outros caches. Os valores possíveis são: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.|
|contentCachingPeerListenRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Uma lista de caches de conteúdo de intervalos IP personalizados será usada para escutar caches de pares. Esta coleção pode conter um máximo de 500 elementos.|
|contentCachingPeerFilterRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Uma lista de caches de conteúdo de intervalos IP personalizados será usada para consultar conteúdo de caches de pares. Esta coleção pode conter um máximo de 500 elementos.|
|contentCachingParentSelectionPolicy|[macOSContentCachingParentSelectionPolicy](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|Determina o método no qual os servidores de cache de conteúdo selecionarão pais se vários estão presentes. Os possíveis valores são: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.|
|contentCachingParents|String collection|Uma lista de endereços IP que representam caches de conteúdo pai.|
|contentCachingLogClientIdentities|Boleano|Habilita o registro em log de endereços IP e portas de clientes que solicitam conteúdo armazenado em cache.|
|contentCachingPublicRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Uma lista de intervalos IP personalizados que o serviço de cache de conteúdo da Apple deve usar para corresponder clientes a caches de conteúdo. Esta coleção pode conter um máximo de 500 elementos.|
|contentCachingBlockDeletion|Boleano|Impede que os caches de conteúdo puriem conteúdo para liberar espaço em disco para outros aplicativos.|
|contentCachingShowAlerts|Boleano|Exibir alertas de cache de conteúdo como notificações do sistema.|
|contentCachingKeepAwake|Boleano|Impedir que o dispositivo adormeça se o cache de conteúdo estiver habilitado.|
|contentCachingPort|Int32|Define a porta usada para o cache de conteúdo. Se o valor for 0, uma porta disponível aleatória será selecionada. Valores válidos de 0 a 65535|

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
|singleSignOnExtensionPkinitCertificate|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Certificado PKINIT para a autenticação com extensões de login único.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "String",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "String",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "String",
      "domains": [
        "String"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "String",
    "teamIdentifier": "String",
    "domains": [
      "String"
    ],
    "realm": "String",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "String",
        "value": "String"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "String",
    "domains": [
      "String"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "String",
    "credentialBundleIdAccessControlList": [
      "String"
    ],
    "domainRealms": [
      "String"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 1024,
    "passwordExpirationNotificationDays": 1024,
    "userPrincipalName": "String",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 1024,
    "passwordMinimumLength": 1024,
    "passwordMinimumAgeDays": 1024,
    "passwordRequirementsDescription": "String",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "String",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "String"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "String",
  "contentCachingMaxSizeBytes": 1024,
  "contentCachingDataPath": "String",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "String",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingPeerPolicy": "String",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingParentSelectionPolicy": "String",
  "contentCachingParents": [
    "String"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 1024
}
```



