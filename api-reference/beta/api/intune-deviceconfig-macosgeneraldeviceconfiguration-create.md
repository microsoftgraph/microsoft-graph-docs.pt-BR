---
title: Criar macOSGeneralDeviceConfiguration
description: Cria um novo objeto macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa5afab21f38da8ce2a18c75ab295e439bf9a4e2
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711932"
---
# <a name="create-macosgeneraldeviceconfiguration"></a>Criar macOSGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto macOSGeneralDeviceConfiguration.

A tabela a seguir mostra as propriedades obrigatórias ao criar macOSGeneralDeviceConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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
|keychainBlockCloudSync|Booliano|Indica se a sincronização do chaveiro do iCloud está bloqueada ou não (macOS 10.12 e posterior).|
|safariBlockAutofill|Boolean|Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.|
|cameraBlocked|Boolean|Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|iTunesBlockMusicService|Boolean|Indica se o serviço música deve ou não ser bloqueado e reverter o aplicativo música para o modo clássico.|
|spotlightBlockInternetResults|Boolean|Indica se o Destaque deve ou não ser bloqueado de retornar quaisquer resultados de uma pesquisa na Internet.|
|keyboardBlockDictation|Boolean|Indica se o usuário deve ou não bloquear o uso da entrada de ditado.|
|definitionLookupBlocked|Boolean|Indica se a pesquisa de definição deve ou não ser bloqueado.|
|appleWatchBlockAutoUnlock|Booliano|Indica se os usuários podem ou não bloquear o desbloqueio do Mac com o Apple Watch.|
|iTunesBlockFileSharing|Boolean|Indica se os arquivos serão ou não bloqueados de serem transferidos usando o iTunes.|
|iCloudBlockDocumentSync|Boolean|Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.|
|iCloudBlockMail|Booliano|Indica se o iCloud deve ou não ser bloqueado da sincronização de emails.|
|iCloudBlockAddressBook|Booliano|Indica se o iCloud deve ou não impedir a sincronização de contatos.|
|iCloudBlockCalendar|Booliano|Indica se o iCloud deve ou não bloquear a sincronização de calendários.|
|iCloudBlockReminders|Booliano|Indica se o iCloud deve ou não bloquear a sincronização de lembretes.|
|iCloudBlockBookmarks|Booliano|Indica se o iCloud deve ou não ser bloqueado da sincronização de indicadores.|
|iCloudBlockNotes|Booliano|Indica se o iCloud deve ou não bloquear a sincronização de anotações.|
|airDropBlocked|Boolean|Indica se o AirDrop permitirá ou não.|
|passwordBlockModification|Booliano|Indica se a modificação da senha deve ou não ser possível.|
|passwordBlockFingerprintUnlock|Boolean|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passwordBlockAutoFill|Booliano|Indica se o recurso Senhas de Preenchimento Automático deve ou não ser bloqueado.|
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
|classroomForceUnpromptedAppAndDeviceLock|Booliano|Indica se o professor deve ou não permitir que o professor bloqueie aplicativos ou o dispositivo sem solicitar ao aluno. Requer o registro MDM por meio do Apple School Manager ou do Apple Business Manager.|
|iCloudBlockActivityContinuation|Boolean|Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado em um dispositivo MacOS em outro dispositivo iOS ou MacOS (MacOS 10.15 ou posterior).|
|privacyAccessControls|[Coleção macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)|Lista de controles de política de preferência de privacidade. Essa coleção pode conter um máximo de 10.000 elementos.|
|addingGameCenterFriendsBlocked|Booliano|Sim impede que os usuários adicionem amigos ao Game Center. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|gameCenterBlocked|Boolean|Sim desabilita o Game Center e o ícone da Central de Jogos é removido da Tela Inicial. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|multiplayerGamingBlocked|Booliano|TRUE impede jogos multijogador ao usar o Game Center. FALSE permite jogos multijogador ao usar o Game Center. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|wallpaperModificationBlocked|Boolean|TRUE impede que o papel de parede seja alterado. FALSE permite que o papel de parede seja alterado. Disponível para dispositivos que executam versões do macOS 10.13 e posteriores.|
|eraseContentAndSettingsBlocked|Booliano|TRUE desabilita a opção de redefinição em dispositivos supervisionados. FALSE habilita a opção de redefinição em dispositivos supervisionados. Disponível para dispositivos que executam versões 12.0 do macOS e posteriores.|
|softwareUpdateMajorOSDeferredInstallDelayInDays|Int32|Especifique o número de dias (1 a 90) para atrasar a visibilidade das principais atualizações de software do sistema operacional. Disponível para dispositivos que executam versões do macOS 11.3 e posteriores. Valores válidos de 0 a 90|
|softwareUpdateMinorOSDeferredInstallDelayInDays|Int32|Especifique o número de dias (1 a 90) para atrasar a visibilidade de atualizações secundárias de software do sistema operacional. Disponível para dispositivos que executam versões do macOS 11.3 e posteriores. Valores válidos de 0 a 90|
|softwareUpdateNonOSDeferredInstallDelayInDays|Int32|Especifique o número de dias (1 a 90) para atrasar a visibilidade de atualizações de software que não são do sistema operacional. Disponível para dispositivos que executam versões do macOS 11.3 e posteriores. Valores válidos de 0 a 90|
|touchIdTimeoutInHours|Int32|Horas máximas após as quais o usuário deve inserir sua senha para desbloquear o dispositivo em vez de usar a ID do Touch. Disponível para dispositivos que executam o macOS 12 e posterior. Valores válidos de 0 a 2147483647|
|iCloudPrivateRelayBlocked|Boolean|O retransmissão privada do iCloud é um serviço iCloud+ que impede que redes e servidores monitorem a atividade de uma pessoa na Internet. Bloqueando o retransmissão privada do iCloud, a Apple não criptografa o tráfego que sai do dispositivo. Disponível para dispositivos que executam o macOS 12 e posterior.|
|iCloudDesktopAndDocumentsBlocked|Boolean|Quando TRUE, a sincronização da área de trabalho na nuvem e documentos é bloqueada. Quando FALSE, a sincronização da área de trabalho de nuvem e documentos são permitidas. Disponível para dispositivos que executam o macOS 10.12.4 e posteriores.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5014

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
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
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
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
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 13,
  "touchIdTimeoutInHours": 5,
  "iCloudPrivateRelayBlocked": true,
  "iCloudDesktopAndDocumentsBlocked": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5186

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
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
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
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
  "softwareUpdateMajorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateMinorOSDeferredInstallDelayInDays": 15,
  "softwareUpdateNonOSDeferredInstallDelayInDays": 13,
  "touchIdTimeoutInHours": 5,
  "iCloudPrivateRelayBlocked": true,
  "iCloudDesktopAndDocumentsBlocked": true
}
```




