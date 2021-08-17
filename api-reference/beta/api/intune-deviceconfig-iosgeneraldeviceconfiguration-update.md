---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85a90fd74553e06f26a2915b605f7e590b54ece0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262568"
---
# <a name="update-iosgeneraldeviceconfiguration"></a>Atualizar iosGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountBlockModification|Boolean|Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.|
|activationLockAllowWhenSupervised|Boolean|Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.|
|airDropBlocked|Boolean|Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.|
|airDropForceUnmanagedDropTarget|Boolean|Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.|
|appleWatchBlockPairing|Boolean|Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appleWatchForceWristDetection|Boolean|Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).|
|appleNewsBlocked|Boolean|Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appsSingleAppModeList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único. Apenas em modo supervisionado. iOS 7.0 e posterior. Esta coleção pode conter um máximo de 500 elementos.|
|appsVisibilityList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior). Essa coleção pode conter um máximo de 10.000 elementos.|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Tipo de lista que está em AppsVisibilityList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Boolean|Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appStoreBlocked|Boolean|Indica se o usuário será ou não impedido de usar a App Store. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|appStoreBlockInAppPurchases|Boolean|Indica se o usuário será ou não impedido de fazer compras no aplicativo.|
|appStoreBlockUIAppInstallation|Boolean|Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host. Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).|
|appStoreRequirePassword|Boolean|Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.|
|autoFillForceAuthentication|Boolean|Indica se a autenticação do usuário deve ou não forçar o preenchimento automático de senhas e informações de cartão de crédito no Safari e em outros aplicativos em dispositivos supervisionados.|
|bluetoothBlockModification|Boolean|Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).|
|cameraBlocked|Boolean|Indica se o usuário será ou não impedido de acessar a câmera do dispositivo. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|cellularBlockDataRoaming|Boolean|Indica se o roaming de dados deve ou não ser bloqueado.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|Indica se a busca global em segundo plano será ou não bloqueada durante roaming.|
|cellularBlockPerAppDataModification|Boolean|Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.|
|cellularBlockPersonalHotspot|Boolean|Indica se o hotspot pessoal deve ou não ser bloqueado.|
|cellularBlockPlanModification|Boolean|Indica se os usuários podem ou não permitir que os usuários alterem as configurações do plano celular em um dispositivo supervisionado.|
|cellularBlockVoiceRoaming|Boolean|Indica se o roaming de voz deve ou não ser bloqueado.|
|certificatesBlockUntrustedTlsCertificates|Boolean|Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.|
|classroomAppBlockRemoteScreenObservation|Boolean|Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).|
|classroomAppForceUnpromptedScreenObservation|Boolean|Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.|
|classroomForceAutomaticallyJoinClasses|Boolean|Indica se o usuário deve ou não dar permissão automaticamente às solicitações do professor, sem solicitar ao aluno, quando o dispositivo estiver no modo supervisionado.|
|classroomForceUnpromptedAppAndDeviceLock|Boolean|Indica se o professor deve ou não permitir que o professor bloqueie aplicativos ou o dispositivo sem solicitar ao aluno. Apenas em modo supervisionado.|
|compliantAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Lista que está em AppComplianceList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Boolean|Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.|
|definitionLookupBlocked|Boolean|Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|deviceBlockEnableRestrictions|Boolean|Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.|
|deviceBlockEraseContentAndSettings|Boolean|Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.|
|deviceBlockNameModification|Boolean|Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|diagnosticDataBlockSubmission|Boolean|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|diagnosticDataBlockSubmissionModification|Boolean|Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.|
|emailInDomainSuffixes|String collection|Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.|
|enterpriseAppBlockTrust|Boolean|Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.|
|enterpriseAppBlockTrustModification|Boolean|\[Preterido Configurar essa configuração e definir o valor como \] "true" não tem efeito no dispositivo.|
|esimBlockModification|Boolean|Indica se é ou não para permitir a adição ou remoção de planos celulares no eSIM de um dispositivo supervisionado.|
|faceTimeBlocked|Boolean|Indica se o usuário será ou não impedido de usar o FaceTime. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|findMyFriendsBlocked|Boolean|Indica se deve ou não bloquear as alterações para Encontrar Meus Amigos quando o dispositivo estiver no modo supervisionado.|
|gamingBlockGameCenterFriends|Boolean|Indica se o usuário será ou não impedido de ter amigos no Game Center. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|gamingBlockMultiplayer|Boolean|Indica se o usuário será ou não impedido de usar jogos para vários participantes. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|gameCenterBlocked|Boolean|Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.|
|hostPairingBlocked|Boolean|indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.|
|iBooksStoreBlocked|Boolean|Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.|
|iBooksStoreBlockErotica|Boolean|Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.|
|iCloudBlockActivityContinuation|Boolean|Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado no dispositivo iOS para outro dispositivo iOS ou macOS.|
|iCloudBlockBackup|Boolean|Indica se o backup do iCloud deve ou não ser bloqueado. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|iCloudBlockDocumentSync|Boolean|Indica se a sincronização de documentos do iCloud deve ou não ser bloqueado. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|iCloudBlockManagedAppsSync|Boolean|Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.|
|iCloudBlockPhotoLibrary|Boolean|Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.|
|iCloudBlockPhotoStreamSync|Boolean|Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.|
|iCloudBlockSharedPhotoStream|Boolean|Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.|
|iCloudRequireEncryptedBackup|Boolean|Indica se a criptografia de backups no iCloud será exigida ou não.|
|iTunesBlockExplicitContent|Boolean|Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|iTunesBlockMusicService|Boolean|Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).|
|iTunesBlockRadio|Boolean|Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).|
|keyboardBlockAutoCorrect|Boolean|Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|keyboardBlockDictation|Boolean|Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.|
|keyboardBlockPredictive|Boolean|Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|keyboardBlockShortcuts|Boolean|Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|keyboardBlockSpellCheck|Boolean|Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|kioskModeAllowAssistiveSpeak|Boolean|Indica se a fala assistencial será permitida ou não no modo quiosque.|
|kioskModeAllowAssistiveTouchSettings|Boolean|Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.|
|kioskModeAllowAutoLock|Boolean|Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque. A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida. Em vez disso, use KioskModeBlockAutoLock.|
|kioskModeBlockAutoLock|Boolean|Indica se o bloqueio automático do dispositivo deve ou não ser bloqueado no modo quiosque.|
|kioskModeAllowColorInversionSettings|Boolean|Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.|
|kioskModeAllowRingerSwitch|Boolean|Indica se o uso do botão de toque será permitido ou não no modo quiosque. A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida. Use KioskModeBlockRingerSwitch.|
|kioskModeBlockRingerSwitch|Boolean|Indica se o uso do aneler deve ou não ser bloqueado enquanto estiver no modo quiosque.|
|kioskModeAllowScreenRotation|Boolean|Indica se a rotação de tela será permitida ou não no modo quiosque. A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida. Use KioskModeBlockScreenRotation em vez disso.|
|kioskModeBlockScreenRotation|Boolean|Indica se a rotação da tela deve ou não ser bloqueado enquanto estiver no modo quiosque.|
|kioskModeAllowSleepButton|Boolean|Indica se o uso do botão de suspensão será permitido ou não no modo quiosque. A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida. Use KioskModeBlockSleepButton em vez disso.|
|kioskModeBlockSleepButton|Boolean|Indica se o uso do botão de sono deve ou não ser bloqueado enquanto estiver no modo quiosque.|
|kioskModeAllowTouchscreen|Boolean|Indica se o uso da tela touch será permitido ou não no modo quiosque. A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida. Use KioskModeBlockTouchscreen em vez disso.|
|kioskModeBlockTouchscreen|Boolean|Indica se o uso da tela sensível ao toque deve ou não ser bloqueado no modo quiosque.|
|kioskModeEnableVoiceControl|Boolean|Indica se o controle de voz deve ou não ser habilitado no modo quiosque.|
|kioskModeAllowVoiceControlModification|Boolean|Indica se o usuário pode ou não alternar o controle de voz no modo quiosque.|
|kioskModeAllowVoiceOverSettings|Boolean|Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.|
|kioskModeAllowVolumeButtons|Boolean|Indica se o uso dos botões de volume será permitido ou não no modo quiosque. A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida. Use KioskModeBlockVolumeButtons.|
|kioskModeBlockVolumeButtons|Boolean|Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.|
|kioskModeAllowZoomSettings|Boolean|Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.|
|kioskModeAppStoreUrl|String|URL na loja de aplicativos do aplicativo para uso no modo de quiosque. Use se KioskModeManagedAppId não for conhecido.|
|kioskModeBuiltInAppId|Cadeia de caracteres|ID para aplicativos integrados a usar no modo de quiosque. Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não estão definidos.|
|kioskModeRequireAssistiveTouch|Boolean|Indica se o toque assistencial deve ou não ser exigido no modo quiosque.|
|kioskModeRequireColorInversion|Boolean|Indica se a inversão de cores deve ou não ser exigida no modo quiosque.|
|kioskModeRequireMonoAudio|Boolean|Indica se o áudio mono deve ou não ser exigido no modo quiosque.|
|kioskModeRequireVoiceOver|Boolean|Indica se o voice over deve ou não ser exigido no modo quiosque.|
|kioskModeRequireZoom|Boolean|Indica se o zoom deve ou não ser exigido no modo quiosque.|
|kioskModeManagedAppId|String|ID de gerenciamento do aplicativo para uso no modo de quiosque. Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.|
|lockScreenBlockControlCenter|Boolean|Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.|
|lockScreenBlockNotificationView|Boolean|Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.|
|lockScreenBlockPassbook|Boolean|Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado|
|lockScreenBlockTodayView|Boolean|Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|Configurações de classificação de conteúdo de mídia da Austrália|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune-deviceconfig-mediacontentratingcanada.md)|Configurações de classificação de conteúdo de mídia do Canadá|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune-deviceconfig-mediacontentratingfrance.md)|Configurações de classificação de conteúdo de mídia da França|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune-deviceconfig-mediacontentratinggermany.md)|Configurações de classificação de conteúdo de mídia da Alemanha|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune-deviceconfig-mediacontentratingireland.md)|Configurações de classificação de conteúdo de mídia da Irlanda|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune-deviceconfig-mediacontentratingjapan.md)|Configurações de classificação de conteúdo de mídia do Japão|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|Configurações de classificação de conteúdo de mídia da Nova Zelândia|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|Configurações de classificação de conteúdo de mídia do Reino Unido|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|Configurações de classificação de conteúdo de mídia dos Estados Unidos|
|networkUsageRules|Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)|Lista de aplicativos gerenciados e regras de rede que se aplicam a eles. Essa coleção pode conter um máximo de 1.000 elementos.|
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|Configurações de classificação de conteúdo de mídia para Aplicativos. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Boolean|Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.|
|notificationsBlockSettingsModification|Boolean|Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).|
|passcodeBlockFingerprintUnlock|Boolean|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passcodeBlockFingerprintModification|Boolean|Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.|
|passcodeBlockModification|Boolean|Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).|
|passcodeBlockSimple|Boolean|Indica se códigos de acesso simples devem ou não ser bloqueados.|
|passcodeExpirationDays|Int32|Número de dias antes da expiração do código de acesso. Valores válidos de 1 a 65535|
|passcodeMinimumLength|Int32|Comprimento mínimo do código de acesso. Valores válidos de 4 a 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que um código de acesso seja necessário.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passcodeMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter. Valores válidos de 0 a 4|
|passcodePreviousPasscodeBlockCount|Int32|Número de códigos de acesso anteriores para bloquear. Valores válidos de 1 a 24|
|passcodeSignInFailureCountBeforeWipe|Int32|Número permitido de falhas de entrada antes da limpeza do dispositivo. Valores válidos de 2 a 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Boolean|Indica se um código de acesso deve ou não ser exigido.|
|podcastsBlocked|Boolean|Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).|
|proximityBlockSetupToNewDevice|Boolean|Indica se o prompt deve ou não habilitar a instalação de dispositivos próximos com um dispositivo supervisionado.|
|safariBlockAutofill|Boolean|Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|safariBlockJavaScript|Boolean|Indica se o JavaScript deve ou não ser bloqueado no Safari.|
|safariBlockPopups|Boolean|Indica se os popups devem ou não ser bloqueados no Safari.|
|safariBlocked|Boolean|Indica se o usuário será ou não impedido de usar o Safari. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Configurações de cookie do Safari. Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|String collection|As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.|
|safariPasswordAutoFillDomains|String collection|Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui. Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).|
|safariRequireFraudWarning|Boolean|Indica se um aviso de fraude deve ou não ser exigido no Safari.|
|screenCaptureBlocked|Boolean|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|siriBlocked|Boolean|Indica se o usuário será ou não impedido de usar a Siri.|
|siriBlockedWhenLocked|Boolean|Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.|
|siriBlockUserGeneratedContent|Boolean|Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.|
|siriRequireProfanityFilter|Boolean|Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.|
|softwareUpdatesEnforcedDelayInDays|Int32|Define quantos dias uma atualização de software será usada para um dispositivo supervisionado. Valores válidos de 0 a 90|
|softwareUpdatesForceDelayed|Boolean|Indica se o usuário deve ou não atrasar a visibilidade das atualizações de software quando o dispositivo estiver no modo supervisionado.|
|spotlightBlockInternetResults|Boolean|Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.|
|voiceDialingBlocked|Boolean|Indica se a discagem de voz deve ou não ser bloqueada.|
|wallpaperBlockModification|Boolean|Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado. Disponível para dispositivos que executam versões 14.4 e anteriores do iOS e iPadOS. Os dispositivos que executam 14,5+ devem usar a configuração "WiFiConnectToAllowedNetworksOnlyForced.|
|classroomForceRequestPermissionToLeaveClasses|Boolean|Indica se um aluno matriculado em um curso não controlado via Classroom solicitará permissão do professor ao tentar sair do curso (iOS 11.3 e posterior).|
|keychainBlockCloudSync|Boolean|Indica se a sincronização do chaveiro do iCloud está bloqueada ou não. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|pkiBlockOTAUpdates|Boolean|Indica se as atualizações PKI sobre o ar estão ou não bloqueadas. Definir essa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7.0 e posterior).|
|privacyForceLimitAdTracking|Boolean|Indica se o controle de ad é limitado. (iOS 7.0 e posterior).|
|enterpriseBookBlockBackup|Boolean|Indica se o Enterprise de reserva está bloqueado ou não.|
|enterpriseBookBlockMetadataSync|Boolean|Indica se a sincronização de Enterprise e realçamentos do livro está bloqueada.|
|airPrintBlocked|Boolean|Indica se o AirPrint está ou não bloqueado (iOS 11.0 e posterior).|
|airPrintBlockCredentialsStorage|Boolean|Indica se o armazenamento de chaves de nome de usuário e senha para Airprint está bloqueado (iOS 11.0 e posterior).|
|airPrintForceTrustedTLS|Boolean|Indica se certificados confiáveis são necessários para comunicação de impressão TLS (iOS 11.0 e posterior).|
|airPrintBlockiBeaconDiscovery|Boolean|Indica se a descoberta iBeacon ou não de impressoras AirPrint está bloqueada. Isso impede que os sinalizadores AirPrint Bluetooth phishing para tráfego de rede (iOS 11.0 e posterior).|
|filesNetworkDriveAccessBlocked|Boolean|Indica se os dispositivos podem acessar arquivos ou outros recursos em um servidor de rede usando o protocolo SMB (Server Message Block). Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.|
|filesUsbDriveAccessBlocked|Boolean|Indica se os sevices com acesso podem se conectar e abrir arquivos em uma unidade USB. Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.|
|wifiPowerOnForced|Boolean|Indica se o Wi-Fi permanece ou não, mesmo quando o dispositivo está no modo de avião. Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.|
|blockSystemAppRemoval|Boolean|Indica se a remoção ou não de aplicativos do sistema do dispositivo está bloqueada em um dispositivo supervisionado (iOS 11.0 e posterior).|
|vpnBlockCreation|Boolean|Indica se a criação de configurações VPN está ou não bloqueada (iOS 11.0 e posterior).|
|appRemovalBlocked|Boolean|Indica se a remoção de aplicativos é permitida.|
|usbRestrictedModeBlocked|Boolean|Indica se a conexão com acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).|
|passwordBlockAutoFill|Boolean|Indica se o recurso Senhas de Preenchimento Automático é permitido (iOS 12.0 e posterior).|
|passwordBlockProximityRequests|Boolean|Indica se deve ou não bloquear a solicitação de senhas de dispositivos próximos (iOS 12.0 e posterior).|
|passwordBlockAirDropSharing|Boolean|Indica se deve ou não bloquear o compartilhamento de senhas com o recurso de senhas do AirDrop iOS 12.0 e posterior).|
|dateAndTimeForceSetAutomatically|Boolean|Indica se o recurso Data e Hora "Definir Automaticamente" está habilitado e não pode ser desligado pelo usuário (iOS 12.0 e posterior).|
|contactsAllowManagedToUnmanagedWrite|Boolean|Indica se os aplicativos gerenciados podem ou não gravar contatos em contas de contatos não gerenciadas (iOS 12.0 e posteriores).|
|contactsAllowUnmanagedToManagedRead|Boolean|Indica se aplicativos não gerenciados podem ou não ler de contas de contatos gerenciados (iOS 12.0 ou posterior).|
|cellularBlockPersonalHotspotModification|Boolean|Indica se o usuário deve ou não bloquear a modificação da configuração de hotspot pessoal (iOS 12.2 ou posterior).|
|continuousPathKeyboardBlocked|Boolean|Indica se o teclado de caminho contínuo deve ou não ser bloqueado quando o dispositivo é supervisionado (iOS 13 ou posterior).|
|findMyDeviceInFindMyAppBlocked|Boolean|Indica se o dispositivo deve ou não ser bloqueado quando o dispositivo é supervisionado (iOS 13 ou posterior).|
|findMyFriendsInFindMyAppBlocked|Boolean|Indica se deve ou não bloquear Find My Friends quando o dispositivo é supervisionado (iOS 13 ou posterior).|
|iTunesBlocked|Boolean|Indica se o aplicativo iTunes deve ou não ser bloqueado. Requer um dispositivo supervisionado para iOS 13 e posterior.|
|sharedDeviceBlockTemporarySessions|Boolean|Indica se as sessões temporárias de iPads compartilhados (iOS 13.4 ou posteriores) são ou não bloqueados.|
|appClipsBlocked|Boolean|Impede que um usuário adicione clipes de aplicativo e remova todos os Clipes de Aplicativo existentes no dispositivo.|
|applePersonalizedAdsBlocked|Boolean|Limita a publicidade personalizada da Apple quando true. Disponível no iOS 14 e posterior.|
|nfcBlocked|Boolean|Desabilite a NFC para impedir que dispositivos emparelhem com outros dispositivos habilitados para NFC. Disponível para dispositivos iOS/iPadOS que executam 14.2 e posteriores.|
|autoUnlockBlocked|Boolean|Impede que os usuários desbloqueiem seus dispositivos com o Apple Watch. Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.|
|unpairedExternalBootToRecoveryAllowed|Boolean|Permitir que os usuários inicialm dispositivos no modo de recuperação com dispositivos não organizados. Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.|
|onDeviceOnlyDictationForced|Boolean|Desabilita conexões com servidores Siri para que os usuários não possam usar a Siri para ditar o texto. Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.|
|wiFiConnectToAllowedNetworksOnlyForced|Boolean|Exigir que os dispositivos usem Wi-Fi redes configuradas por meio de perfis de configuração. Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.|
|kioskModeAppType|[iosKioskModeAppType](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|Tipo de aplicativo a ser executado no modo quiosque. Os valores possíveis são: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10827

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "wiFiConnectToAllowedNetworksOnlyForced": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10999

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "wiFiConnectToAllowedNetworksOnlyForced": true,
  "kioskModeAppType": "appStoreApp"
}
```




