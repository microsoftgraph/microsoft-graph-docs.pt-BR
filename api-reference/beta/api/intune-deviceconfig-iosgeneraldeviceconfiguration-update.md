---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
ms.openlocfilehash: 651915670976792e923ba34d8d560521742bbd44
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033444"
---
# <a name="update-iosgeneraldeviceconfiguration"></a>Atualizar iosGeneralDeviceConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountBlockModification|Booliano|Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.|
|activationLockAllowWhenSupervised|Booliano|Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.|
|airDropBlocked|Booliano|Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.|
|airDropForceUnmanagedDropTarget|Booliano|Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).|
|airPlayForcePairingPasswordForOutgoingRequests|Booliano|Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.|
|appleWatchBlockPairing|Booliano|Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appleWatchForceWristDetection|Booliano|Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).|
|appleNewsBlocked|Booliano|Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appsSingleAppModeList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único. Apenas em modo supervisionado. iOS 7.0 e posterior. Esta coleção pode conter um máximo de 500 elementos.|
|appsVisibilityList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior). Essa coleção pode conter um máximo de 10.000 elementos.|
|appsVisibilityListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Tipo de lista que está em AppsVisibilityList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Booliano|Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appStoreBlocked|Booliano|Indica se o usuário será ou não impedido de usar a App Store.|
|appStoreBlockInAppPurchases|Booliano|Indica se o usuário será ou não impedido de fazer compras no aplicativo.|
|appStoreBlockUIAppInstallation|Booliano|Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host. Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).|
|appStoreRequirePassword|Booliano|Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.|
|bluetoothBlockModification|Booliano|Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).|
|cameraBlocked|Booliano|Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|cellularBlockDataRoaming|Booliano|Indica se o roaming de dados deve ou não ser bloqueado.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Booliano|Indica se a busca global em segundo plano será ou não bloqueada durante roaming.|
|cellularBlockPerAppDataModification|Booliano|Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.|
|cellularBlockPersonalHotspot|Booliano|Indica se o hotspot pessoal deve ou não ser bloqueado.|
|cellularBlockVoiceRoaming|Booliano|Indica se o roaming de voz deve ou não ser bloqueado.|
|certificatesBlockUntrustedTlsCertificates|Booliano|Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.|
|classroomAppBlockRemoteScreenObservation|Booliano|Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).|
|classroomAppForceUnpromptedScreenObservation|Booliano|Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.|
|compliantAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Lista que está em AppComplianceList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Booliano|Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.|
|definitionLookupBlocked|Booliano|Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|deviceBlockEnableRestrictions|Booliano|Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.|
|deviceBlockEraseContentAndSettings|Booliano|Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.|
|deviceBlockNameModification|Booliano|Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|diagnosticDataBlockSubmission|Booliano|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|diagnosticDataBlockSubmissionModification|Booliano|Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).|
|documentsBlockManagedDocumentsInUnmanagedApps|Booliano|Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.|
|documentsBlockUnmanagedDocumentsInManagedApps|Booliano|Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.|
|emailInDomainSuffixes|String collection|Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.|
|enterpriseAppBlockTrust|Booliano|Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.|
|enterpriseAppBlockTrustModification|Booliano|Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.|
|faceTimeBlocked|Booliano|Indica se o usuário será ou não impedido de usar o FaceTime.|
|findMyFriendsBlocked|Booliano|Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.|
|gamingBlockGameCenterFriends|Booliano|Indica se o usuário será ou não impedido de ter amigos no Game Center.|
|gamingBlockMultiplayer|Booliano|Indica se o usuário será ou não impedido de usar jogos para vários participantes.|
|gameCenterBlocked|Booliano|Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.|
|hostPairingBlocked|Booliano|indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.|
|iBooksStoreBlocked|Booliano|Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.|
|iBooksStoreBlockErotica|Booliano|Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.|
|iCloudBlockActivityContinuation|Booliano|Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.|
|iCloudBlockBackup|Booliano|Indica se o backup do iCloud deve ou não ser bloqueado.|
|iCloudBlockDocumentSync|Booliano|Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.|
|iCloudBlockManagedAppsSync|Booliano|Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.|
|iCloudBlockPhotoLibrary|Booliano|Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.|
|iCloudBlockPhotoStreamSync|Booliano|Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.|
|iCloudBlockSharedPhotoStream|Booliano|Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.|
|iCloudRequireEncryptedBackup|Booliano|Indica se a criptografia de backups no iCloud será exigida ou não.|
|iTunesBlockExplicitContent|Booliano|Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.|
|iTunesBlockMusicService|Booliano|Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).|
|iTunesBlockRadio|Booliano|Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).|
|keyboardBlockAutoCorrect|Booliano|Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|keyboardBlockDictation|Booliano|Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.|
|keyboardBlockPredictive|Booliano|Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|keyboardBlockShortcuts|Booliano|Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|keyboardBlockSpellCheck|Booliano|Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|kioskModeAllowAssistiveSpeak|Booliano|Indica se a fala assistencial será permitida ou não no modo quiosque.|
|kioskModeAllowAssistiveTouchSettings|Booliano|Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.|
|kioskModeAllowAutoLock|Booliano|Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.|
|kioskModeAllowColorInversionSettings|Booliano|Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.|
|kioskModeAllowRingerSwitch|Booliano|Indica se o uso do botão de toque será permitido ou não no modo quiosque.|
|kioskModeAllowScreenRotation|Booliano|Indica se a rotação de tela será permitida ou não no modo quiosque.|
|kioskModeAllowSleepButton|Booliano|Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.|
|kioskModeAllowTouchscreen|Booliano|Indica se o uso da tela touch será permitido ou não no modo quiosque.|
|kioskModeAllowVoiceOverSettings|Booliano|Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.|
|kioskModeAllowVolumeButtons|Booliano|Indica se o uso dos botões de volume será permitido ou não no modo quiosque.|
|kioskModeBlockVolumeButtons|Booliano|Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.|
|kioskModeAllowZoomSettings|Booliano|Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.|
|kioskModeAppStoreUrl|String|URL na loja de aplicativos do aplicativo para uso no modo de quiosque. Use se KioskModeManagedAppId não for conhecido.|
|kioskModeBuiltInAppId|String|ID para aplicativos internos a ser usado para o modo de quiosque. Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidas.|
|kioskModeRequireAssistiveTouch|Booliano|Indica se o toque assistencial deve ou não ser exigido no modo quiosque.|
|kioskModeRequireColorInversion|Booliano|Indica se a inversão de cores deve ou não ser exigida no modo quiosque.|
|kioskModeRequireMonoAudio|Booliano|Indica se o áudio mono deve ou não ser exigido no modo quiosque.|
|kioskModeRequireVoiceOver|Booliano|Indica se o voice over deve ou não ser exigido no modo quiosque.|
|kioskModeRequireZoom|Booliano|Indica se o zoom deve ou não ser exigido no modo quiosque.|
|kioskModeManagedAppId|String|ID de gerenciamento do aplicativo para uso no modo de quiosque. Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.|
|lockScreenBlockControlCenter|Booliano|Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.|
|lockScreenBlockNotificationView|Booliano|Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.|
|lockScreenBlockPassbook|Booliano|Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado|
|lockScreenBlockTodayView|Booliano|Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.|
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
|mediaContentRatingApps|[ratingAppsType](../resources/intune-deviceconfig-ratingappstype.md)|As configurações de classificação para aplicativos de conteúdo de mídia. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Booliano|Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.|
|notificationsBlockSettingsModification|Booliano|Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).|
|passcodeBlockFingerprintUnlock|Booliano|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passcodeBlockFingerprintModification|Booliano|Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.|
|passcodeBlockModification|Booliano|Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).|
|passcodeBlockSimple|Booliano|Indica se códigos de acesso simples devem ou não ser bloqueados.|
|passcodeExpirationDays|Int32|Número de dias antes da expiração do código de acesso. Valores válidos de 1 a 65535|
|passcodeMinimumLength|Int32|Comprimento mínimo do código de acesso. Valores válidos de 4 a 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que um código de acesso seja necessário.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passcodeMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter. Valores válidos de 0 a 4|
|passcodePreviousPasscodeBlockCount|Int32|Número de códigos de acesso anteriores para bloquear. Valores válidos de 1 a 24|
|passcodeSignInFailureCountBeforeWipe|Int32|Número permitido de falhas de entrada antes da limpeza do dispositivo. Valores válidos de 4 a 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Booliano|Indica se um código de acesso deve ou não ser exigido.|
|podcastsBlocked|Booliano|Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).|
|safariBlockAutofill|Booliano|Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.|
|safariBlockJavaScript|Booliano|Indica se o JavaScript deve ou não ser bloqueado no Safari.|
|safariBlockPopups|Booliano|Indica se os popups devem ou não ser bloqueados no Safari.|
|safariBlocked|Booliano|Indica se o usuário será ou não impedido de usar o Safari.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Configurações de cookie do Safari. Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|String collection|As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.|
|safariPasswordAutoFillDomains|String collection|Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui. Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).|
|safariRequireFraudWarning|Booliano|Indica se um aviso de fraude deve ou não ser exigido no Safari.|
|screenCaptureBlocked|Booliano|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|siriBlocked|Booliano|Indica se o usuário será ou não impedido de usar a Siri.|
|siriBlockedWhenLocked|Booliano|Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.|
|siriBlockUserGeneratedContent|Booliano|Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.|
|siriRequireProfanityFilter|Booliano|Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.|
|spotlightBlockInternetResults|Booliano|Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.|
|voiceDialingBlocked|Booliano|Indica se a discagem de voz deve ou não ser bloqueada.|
|wallpaperBlockModification|Booliano|Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).|
|wiFiConnectOnlyToConfiguredNetworks|Booliano|Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.|
|classroomForceRequestPermissionToLeaveClasses|Booliano|Indica se um estudante inscrito em um curso não gerenciado por meio da sala de aula solicitará permissão do professor ao tentar deixar o curso (iOS 11.3 e posterior).|
|keychainBlockCloudSync|Booliano|Indica se ou não a sincronização do conjunto de chaves iCloud está bloqueada.|
|pkiBlockOTAUpdates|Booliano|Indica se ou não atualizações PKI via satélite são bloqueadas. Definindo essa restrição para false, não desabilite verificações CRL e OCSP (iOS 7.0 e posterior).|
|privacyForceLimitAdTracking|Booliano|Indica se o anúncio acompanhamento é limitado. (iOS 7.0 e posterior).|
|enterpriseBookBlockBackup|Booliano|Indica se ou não a empresa livro backup seja bloqueado.|
|enterpriseBookBlockMetadataSync|Booliano|Indica se ou não Enterprise catálogo notas e destaques sync está bloqueado.|
|airPrintBlocked|Booliano|Indica se é ou não AirPrint bloqueados (iOS 11.0 e posteriores).|
|airPrintBlockCredentialsStorage|Booliano|Indica se ou não o armazenamento do conjunto de chaves do usuário e senha para Airprint é bloqueado (iOS 11.0 e posteriores).|
|airPrintForceTrustedTLS|Booliano|Indica se os certificados confiáveis são necessários para a comunicação de impressão de TLS (iOS 11.0 e posteriores).|
|airPrintBlockiBeaconDiscovery|Booliano|Indica se ou não iBeacon descoberta de impressoras AirPrint está bloqueada. Isso impede que os avisos de AirPrint Bluetooth artificiais contra phishing para tráfego de rede (iOS 11.0 e posteriores).|
|blockSystemAppRemoval|Booliano|Indica se ou não a remoção de aplicativos do sistema do dispositivo seja bloqueada em um dispositivo supervisionado (iOS 11.0 e posteriores).|
|vpnBlockCreation|Booliano|Indica se é ou não a criação de configurações de VPN bloqueados (iOS 11.0 e posteriores).|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8428

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
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
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8604

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
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
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true
}
```





