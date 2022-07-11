---
title: Tipo de recurso macOSEndpointProtectionConfiguration
description: Perfil de configuração de proteção de ponto de extremidade do MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 213a4173104e159330cce48a8fffefd107b8546c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666981"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>Tipo de recurso macOSEndpointProtectionConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração de proteção de ponto de extremidade do MacOS.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSEndpointProtectionConfigurations](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[Coleção macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Listar propriedades e relações dos objetos [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Obter macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Ler propriedades e relações do objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Criar macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Crie um novo [objeto macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|
|[Excluir macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|Nenhum|Exclui um [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).|
|[Atualizar macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|Atualize as propriedades de um [objeto macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|Configuração de sistema e privacidade que determina de quais locais de download os aplicativos podem ser executados em um dispositivo macOS. Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.|
|gatekeeperBlockOverride|Boolean|Se definido como true, a substituição do usuário para o Gatekeeper será desabilitada.|
|firewallEnabled|Boolean|Se o firewall deve ser habilitado ou não.|
|firewallBlockAllIncoming|Boolean|Corresponde à opção "Bloquear todas as conexões de entrada".|
|firewallEnableStealthMode|Boolean|Corresponde a "Habilitar modo furtivo".|
|firewallApplications|[Coleção macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)|Lista de aplicativos com configurações de firewall. As configurações de firewall para aplicativos que não estão nesta lista são determinadas pelo usuário. Esta coleção pode conter um máximo de 500 elementos.|
|fileVaultEnabled|Boolean|Se o FileVault deve ser habilitado ou não.|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|Necessário se o FileVault estiver habilitado, determina os tipos de chave de recuperação a serem usadas. . Os valores possíveis são: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.|
|fileVaultInstitutionalRecoveryKeyCertificate|Binária|Obrigatório se os tipos de chave de recuperação selecionados incluíem InstitutionalRecoveryKey. O arquivo de certificado codificado por DER usado para definir uma chave de recuperação institucional.|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|Cadeia de caracteres|Nome do arquivo do certificado de chave de recuperação institucional a ser exibido na interface do usuário. (*.der).|
|fileVaultPersonalRecoveryKeyHelpMessage|Cadeia de caracteres|Obrigatório se os tipos de chave de recuperação selecionados incluíem PersonalRecoveryKey. Uma breve mensagem exibida para o usuário que explica como ele pode recuperar sua chave de recuperação pessoal.|
|fileVaultAllowDeferralUntilSignOut|Booleano|Opcional. Se definido como true, o usuário pode adiar a habilitação do FileVault até sair.|
|fileVaultNumberOfTimesUserCanIgnore|Int32|Opcional. Ao usar a opção Defer, esse é o número máximo de vezes que o usuário pode ignorar os prompts para habilitar o FileVault antes que o FileVault seja necessário para o usuário entrar. Se definido como -1, ele sempre solicitará a habilitação do FileVault até que o FileVault esteja habilitado, embora permita que o usuário ignore a habilitação do FileVault. Definir isso como 0 desabilitará o recurso.|
|fileVaultDisablePromptAtSignOut|Booleano|Opcional. Ao usar a opção Defer, se definida como true, o usuário não será solicitado a habilitar o FileVault na saída.|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|Opcional. Se os tipos de chave de recuperação selecionados incluem PersonalRecoveryKey, a frequência para girar essa chave, em meses.|
|fileVaultHidePersonalRecoveryKey|Booleano|Opcional. Uma chave de recuperação pessoal oculta não aparece na tela do usuário durante a criptografia fileVault, reduzindo o risco de ela terminar em mãos erradas.|
|advancedThreatProtectionRealTime|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Determina se a proteção em tempo real da Proteção Avançada contra Ameaças do Microsoft Defender deve ou não ser habilitada no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionCloudDelivered|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Determina se a proteção fornecida na nuvem deve ou não ser habilitada para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionAutomaticSampleSubmission|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Determina se deve ou não habilitar o envio automático de exemplo de arquivo para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionDiagnosticDataCollection|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Determina se a coleta de dados de diagnóstico e uso deve ou não ser habilitada para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|advancedThreatProtectionExcludedFolders|String collection|Uma lista de caminhos para pastas a serem excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|
|advancedThreatProtectionExcludedFiles|Coleção String|Uma lista de caminhos para arquivos a serem excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|
|advancedThreatProtectionExcludedExtensions|String collection|Uma lista de extensões de arquivo a serem excluídas da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|
|advancedThreatProtectionExcludedProcesses|Coleção String|Uma lista de nomes de processo a serem excluídos da verificação de antivírus para a Proteção Avançada contra Ameaças do Microsoft Defender no macOS.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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




