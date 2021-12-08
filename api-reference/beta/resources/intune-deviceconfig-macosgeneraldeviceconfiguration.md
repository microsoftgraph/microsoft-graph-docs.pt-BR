---
title: Tipo de recurso macOSGeneralDeviceConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e3744b905982e72230f07306c696a45731048b6
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338509"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Tipo de recurso macOSGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso macOSGeneralDeviceConfiguration.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSGeneralDeviceConfigurations](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-list.md)|Coleção [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Lista propriedades e relações dos objetos [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Obter macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-get.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Propriedades de leitura e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Criar macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-create.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Excluir macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-delete.md)|Nenhum|Exclui um [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Atualizar macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-update.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|

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
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|compliantAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Lista que está em CompliantAppsList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|emailInDomainSuffixes|String collection|Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.|
|passwordBlockSimple|Boolean|Bloquear senhas simples.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha.|
|passwordMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter. Valores válidos de 0 a 4|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade necessários antes que uma senha seja necessária.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade necessários antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Boolean|Se uma senha deve ou não ser exigida.|
|passwordMaximumAttemptCount|Int32|O número de tentativas de falha permitidas para inserir a senha na tela de bloqueio do dispositivo. Valores válidos de 2 a 11|
|passwordMinutesUntilFailedLoginReset|Int32|O número de minutos antes de o logon ser redefinido depois que o número máximo de tentativas de logon malsucedida é atingido.|
|keychainBlockCloudSync|Boolean|Indica se a sincronização do chaveiro do iCloud está bloqueada ou não (macOS 10.12 e posterior).|
|safariBlockAutofill|Boolean|Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.|
|cameraBlocked|Boolean|Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|iTunesBlockMusicService|Boolean|Indica se o serviço música deve ou não ser bloqueado e reverter o aplicativo música para o modo clássico.|
|spotlightBlockInternetResults|Boolean|Indica se o Destaque deve ou não ser bloqueado de retornar quaisquer resultados de uma pesquisa na Internet.|
|keyboardBlockDictation|Boolean|Indica se o usuário deve ou não bloquear o uso da entrada de ditado.|
|definitionLookupBlocked|Boolean|Indica se a pesquisa de definição deve ou não ser bloqueado.|
|appleWatchBlockAutoUnlock|Boolean|Indica se os usuários podem ou não bloquear o desbloqueio do Mac com o Apple Watch.|
|iTunesBlockFileSharing|Booliano|Indica se os arquivos serão ou não bloqueados de serem transferidos usando o iTunes.|
|iCloudBlockDocumentSync|Boolean|Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.|
|iCloudBlockMail|Booliano|Indica se o iCloud deve ou não ser bloqueado da sincronização de emails.|
|iCloudBlockAddressBook|Booliano|Indica se o iCloud deve ou não impedir a sincronização de contatos.|
|iCloudBlockCalendar|Boolean|Indica se o iCloud deve ou não bloquear a sincronização de calendários.|
|iCloudBlockReminders|Booliano|Indica se o iCloud deve ou não bloquear a sincronização de lembretes.|
|iCloudBlockBookmarks|Booliano|Indica se o iCloud deve ou não ser bloqueado da sincronização de indicadores.|
|iCloudBlockNotes|Booliano|Indica se o iCloud deve ou não bloquear a sincronização de anotações.|
|airDropBlocked|Boolean|Indica se o AirDrop permitirá ou não.|
|passwordBlockModification|Booliano|Indica se a modificação da senha deve ou não ser possível.|
|passwordBlockFingerprintUnlock|Boolean|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passwordBlockAutoFill|Boolean|Indica se o recurso Senhas de Preenchimento Automático deve ou não ser bloqueado.|
|passwordBlockProximityRequests|Boolean|Indica se deve ou não bloquear a solicitação de senhas de dispositivos próximos.|
|passwordBlockAirDropSharing|Booliano|Indica se deve ou não bloquear o compartilhamento de senhas com o recurso de senhas do AirDrop.|
|softwareUpdatesEnforcedDelayInDays|Int32|Define quantos dias uma atualização de software será usada para um dispositivo supervisionado. Valores válidos de 0 a 90|
|updateDelayPolicy|[macOSSoftwareUpdateDelayPolicy](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|Determina se as atualizações do sistema operacional e/ou do aplicativo são demoradas para macOS. Os valores possíveis são: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`, `unknownFutureValue`, `delayMajorOsUpdateVisibility`.|
|contentCachingBlocked|Boolean|Indica se é ou não para permitir o cache de conteúdo.|
|iCloudBlockPhotoLibrary|Boolean|Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.|
|screenCaptureBlocked|Boolean|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|classroomAppBlockRemoteScreenObservation|Boolean|Indica se a observação de tela remota deve ou não ser permitida pelo aplicativo Classroom. Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.|
|classroomAppForceUnpromptedScreenObservation|Boolean|Indica se o professor de um curso gerenciado no aplicativo Classroom deve ou não dar permissão ao professor para exibir a tela de um aluno sem solicitar. Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.|
|classroomForceAutomaticallyJoinClasses|Booliano|Indica se o aluno deve ou não dar permissão automaticamente às solicitações do professor, sem solicitar ao aluno. Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.|
|classroomForceRequestPermissionToLeaveClasses|Booliano|Indica se um aluno matriculado em um curso não organizado via Sala de Aula será necessário para solicitar permissão do professor ao tentar sair do curso. Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.|
|classroomForceUnpromptedAppAndDeviceLock|Boolean|Indica se o professor deve ou não permitir que o professor bloqueie aplicativos ou o dispositivo sem solicitar ao aluno. Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.|
|iCloudBlockActivityContinuation|Boolean|Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado em um dispositivo MacOS em outro dispositivo iOS ou MacOS (MacOS 10.15 ou posterior).|
|privacyAccessControls|[Coleção macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)|Lista de controles de política de preferência de privacidade. Essa coleção pode conter um máximo de 10.000 elementos.|
|addingGameCenterFriendsBlocked|Boolean|Sim impede que os usuários adicionem amigos ao Game Center. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|gameCenterBlocked|Boolean|Sim desabilita o Game Center e o ícone da Central de Jogos é removido da Tela Inicial. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|multiplayerGamingBlocked|Boolean|TRUE impede jogos multijogador ao usar o Game Center. FALSE permite jogos multijogador ao usar o Game Center. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|wallpaperModificationBlocked|Booliano|TRUE impede que o papel de parede seja alterado. FALSE permite que o papel de parede seja alterado. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|eraseContentAndSettingsBlocked|Boolean|TRUE desabilita a opção de redefinição em dispositivos supervisionados. FALSE habilita a opção de redefinição em dispositivos supervisionados. Disponível para dispositivos que executam versões 12.0 do macOS e posteriores.|
|softwareUpdateMajorOSDeferredInstallDelayInDays|Int32|Especifique o número de dias (1 a 90) para atrasar a visibilidade das principais atualizações de software do sistema operacional. Disponível para dispositivos que executam versões do macOS 11.3 e posteriores. Valores válidos de 0 a 90|
|softwareUpdateMinorOSDeferredInstallDelayInDays|Int32|Especifique o número de dias (1 a 90) para atrasar a visibilidade de atualizações secundárias de software do sistema operacional. Disponível para dispositivos que executam versões do macOS 11.3 e posteriores. Valores válidos de 0 a 90|
|softwareUpdateNonOSDeferredInstallDelayInDays|Int32|Especifique o número de dias (1 a 90) para atrasar a visibilidade de atualizações de software que não são do sistema operacional. Disponível para dispositivos que executam versões do macOS 11.3 e posteriores. Valores válidos de 0 a 90|
|touchIdTimeoutInHours|Int32|Horas máximas após as quais o usuário deve inserir sua senha para desbloquear o dispositivo em vez de usar a ID do Touch. Disponível para dispositivos que executam o macOS 12 e posterior. Valores válidos de 0 a 2147483647|
|iCloudPrivateRelayBlocked|Boolean|O retransmissão privada do iCloud é um serviço iCloud+ que impede que redes e servidores monitorem a atividade de uma pessoa na Internet. Bloqueando o retransmissão privada do iCloud, a Apple não criptografa o tráfego que sai do dispositivo. Disponível para dispositivos que executam o macOS 12 e posterior.|

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
  "@odata.type": "microsoft.graph.macOSGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "emailInDomainSuffixes": [
    "String"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 1024,
  "passwordMinutesUntilFailedLoginReset": 1024,
  "keychainBlockCloudSync": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "updateDelayPolicy": "String",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "String",
      "identifier": "String",
      "identifierType": "String",
      "codeRequirement": "String",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "String",
      "accessibility": "String",
      "addressBook": "String",
      "calendar": "String",
      "reminders": "String",
      "photos": "String",
      "mediaLibrary": "String",
      "fileProviderPresence": "String",
      "systemPolicyAllFiles": "String",
      "systemPolicySystemAdminFiles": "String",
      "systemPolicyDesktopFolder": "String",
      "systemPolicyDocumentsFolder": "String",
      "systemPolicyDownloadsFolder": "String",
      "systemPolicyNetworkVolumes": "String",
      "systemPolicyRemovableVolumes": "String",
      "postEvent": "String",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "String",
          "identifier": "String",
          "identifierType": "String",
          "allowed": true
        }
      ]
    }
  ],
  "addingGameCenterFriendsBlocked": true,
  "gameCenterBlocked": true,
  "multiplayerGamingBlocked": true,
  "wallpaperModificationBlocked": true,
  "eraseContentAndSettingsBlocked": true,
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 1024,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 1024,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 1024,
  "touchIdTimeoutInHours": 1024,
  "iCloudPrivateRelayBlocked": true
}
```




