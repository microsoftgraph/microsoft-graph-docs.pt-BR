---
title: Tipo de recurso windows81GeneralConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11903b1186fd334665b62bd203a85fd63ed3c8cb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793572"
---
# <a name="windows81generalconfiguration-resource-type"></a>Tipo de recurso windows81GeneralConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows81GeneralConfiguration.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows81GeneralConfigurations](../api/intune-deviceconfig-windows81generalconfiguration-list.md)|Coleção [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Lista propriedades e relações dos objetos [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Obter windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-get.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Ler propriedades e relações do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Criar windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-create.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[Excluir windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-delete.md)|Nenhum|Excluir um [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|
|[Atualizar windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-update.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.|
|applyOnlyToWindows81|Boolean|Valor que indica se esta política se aplica somente ao Windows 8.1. Essa propriedade é somente leitura.|
|browserBlockAutofill|Boolean|Indica se o preenchimento automático deve ou não ser bloqueado.|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.|
|browserBlockEnterpriseModeAccess|Boolean|Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.|
|browserBlockJavaScript|Boolean|Indica se o usuário será ou não impedido de usar JavaScript.|
|browserBlockPlugins|Boolean|Indica se os plug-ins devem ou não ser bloqueados.|
|browserBlockPopups|Boolean|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|browserBlockSendingDoNotTrackHeader|Boolean|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.|
|browserRequireSmartScreen|Boolean|Indica se o usuário deverá ou não usar o Filtro SmartScreen.|
|browserEnterpriseModeSiteListLocation|String|O local da lista de sites do modo Empresarial. Pode ser um arquivo local, rede local ou local http.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|O nível de segurança da Internet. Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|O nível de segurança da Intranet. Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|browserLoggingReportLocation|String|O local do relatório de registro em log.|
|browserRequireHighSecurityForRestrictedSites|Boolean|Indica se a alta segurança para sites restritos deve ou não ser exigida.|
|browserRequireFirewall|Boolean|Indica se um firewall deve ou não ser exigido.|
|browserRequireFraudWarning|Boolean|Indica se um aviso de fraude deve ou não ser exigido.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|O nível de segurança de sites confiáveis. Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|cellularBlockDataRoaming|Boolean|Indica se o roaming de dados deve ou não ser bloqueado.|
|diagnosticsBlockDataSubmission|Boolean|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|passwordBlockPicturePasswordAndPin|Boolean|Indica se o usuário será ou não impedido de usar senha com imagens ou pin.|
|passwordExpirationDays|Int32|Expiração da senha em dias.|
|passwordMinimumLength|Int32|O comprimento mínimo da senha.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica.|
|storageRequireDeviceEncryption|Boolean|Indica se a criptografia é ou não necessária em um dispositivo móvel.|
|minimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|A classificação de atualização mínima a ser instalada automaticamente. Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.|
|updatesMinimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|A classificação de atualização mínima a ser instalada automaticamente. Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.|
|updatesRequireAutomaticUpdates|Boolean|Indica se as atualizações automáticas devem ou não ser exigidas.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|As configurações de controle da conta do usuário. Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|String|A URL das pastas de trabalho|

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
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "String",
  "updatesMinimumAutoInstallClassification": "String",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



