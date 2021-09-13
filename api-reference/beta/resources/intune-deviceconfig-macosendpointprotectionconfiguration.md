---
title: Tipo de recurso macOSEndpointProtectionConfiguration
description: Perfil de configuração de proteção de ponto de extremidade do MacOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c5ad98d6f208b8e676e335046cc5a66da967de08
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054538"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>Tipo de recurso macOSEndpointProtectionConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração de proteção de ponto de extremidade do MacOS.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSEndpointProtectionConfigurations](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[Coleção macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Listar propriedades e relações dos [objetos macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|
|[Obter macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Leia propriedades e relações do [objeto macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|
|[Criar macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Crie um novo [objeto macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|
|[Excluir macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|Nenhum|Exclui um [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).|
|[Atualizar macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Atualize as propriedades de [um objeto macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|

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
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|Configuração de Sistema e Privacidade que determina de quais locais de download os aplicativos podem ser executados em um dispositivo macOS. Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|gatekeeperBlockOverride|Boleano|Se definido como true, a substituição do usuário para Gatekeeper será desabilitada.|
|firewallEnabled|Boleano|Se o firewall deve ser habilitado ou não.|
|firewallBlockAllIncoming|Boleano|Corresponde à opção "Bloquear todas as conexões de entrada".|
|firewallEnableStealthMode|Boleano|Corresponde a "Habilitar o modo de furtividade".|
|firewallApplications|[Coleção macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)|Lista de aplicativos com configurações de firewall. As configurações de firewall para aplicativos que não estão nesta lista são determinadas pelo usuário. Esta coleção pode conter um máximo de 500 elementos.|
|fileVaultEnabled|Boleano|Se FileVault deve ser habilitado ou não.|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|Obrigatório se FileVault estiver habilitado, determina os tipos da chave de recuperação a ser usada. . Os valores possíveis são: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.|
|fileVaultInstitutionalRecoveryKeyCertificate|Binário|Obrigatório se os tipos de teclas de recuperação selecionados incluirEm InstitucionalRecoveryKey. O arquivo de certificado codificado por DER usado para definir uma chave de recuperação institucional.|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|Cadeia de Caracteres|Nome do arquivo do certificado de chave de recuperação institucional a ser exibido na interface do usuário. (*.der).|
|fileVaultPersonalRecoveryKeyHelpMessage|Cadeia de Caracteres|Obrigatório se os tipos de teclas de recuperação selecionados incluirEm PersonalRecoveryKey. Uma mensagem curta exibida para o usuário que explica como eles podem recuperar sua chave de recuperação pessoal.|
|fileVaultAllowDeferralUntilSignOut|Boleano|Opcional. Se for definido como true, o usuário poderá adiar a habilitação de FileVault até sair.|
|fileVaultNumberOfTimesUserCanIgnore|Int32|Opcional. Ao usar a opção Adiar, esse é o número máximo de vezes que o usuário pode ignorar prompts para habilitar FileVault antes que FileVault seja necessário para o usuário entrar. Se estiver definido como -1, ele sempre solicitará que FileVault seja habilitado até que FileVault seja habilitado, embora permita que o usuário ignore a habilitação de FileVault. Definir isso como 0 desabilitará o recurso.|
|fileVaultDisablePromptAtSignOut|Boleano|Opcional. Ao usar a opção Adiar, se definido como true, o usuário não é solicitado a habilitar FileVault na saída.|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|Opcional. Se os tipos de teclas de recuperação selecionados incluirEm PersonalRecoveryKey, a frequência para girar essa chave, em meses.|
|fileVaultHidePersonalRecoveryKey|Boleano|Opcional. Uma chave de recuperação pessoal oculta não aparece na tela do usuário durante a criptografia FileVault, reduzindo o risco de ela acabar em mãos erradas.|
|advancedThreatProtectionRealTime|[enablement](../resources/intune-shared-enablement.md)|Determina se a proteção em tempo real do Microsoft Defender Advanced Threat Protection será habilitada ou não no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionCloudDelivered|[enablement](../resources/intune-shared-enablement.md)|Determina se a proteção entregue na nuvem deve ou não ser habilitada para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionAutomaticSampleSubmission|[enablement](../resources/intune-shared-enablement.md)|Determina se deve ou não habilitar o envio automático de exemplo de arquivo para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionDiagnosticDataCollection|[enablement](../resources/intune-shared-enablement.md)|Determina se será ou não possível habilitar a coleta de dados de diagnóstico e uso para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionExcludedFolders|String collection|Uma lista de caminhos para pastas a excluir da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|
|advancedThreatProtectionExcludedFiles|String collection|Uma lista de caminhos para arquivos a ser excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|
|advancedThreatProtectionExcludedExtensions|String collection|Uma lista de extensões de arquivo a excluir da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|
|advancedThreatProtectionExcludedProcesses|String collection|Uma lista de nomes de processo a ser excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|

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
  "@odata.type": "microsoft.graph.macOSEndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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
  "gatekeeperAllowedAppSource": "String",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "String",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "String",
  "fileVaultInstitutionalRecoveryKeyCertificate": "binary",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "String",
  "fileVaultPersonalRecoveryKeyHelpMessage": "String",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 1024,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 1024,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "String",
  "advancedThreatProtectionCloudDelivered": "String",
  "advancedThreatProtectionAutomaticSampleSubmission": "String",
  "advancedThreatProtectionDiagnosticDataCollection": "String",
  "advancedThreatProtectionExcludedFolders": [
    "String"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "String"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "String"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "String"
  ]
}
```



