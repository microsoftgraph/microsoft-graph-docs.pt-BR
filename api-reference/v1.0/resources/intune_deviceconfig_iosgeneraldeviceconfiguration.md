# <a name="iosgeneraldeviceconfiguration-resource-type"></a>Tipo de recurso iosGeneralDeviceConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso iosGeneralDeviceConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosGeneralDeviceConfigurations](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_list.md)|Coleção [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Listar propriedades e relações dos objetos [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Obter iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_get.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Ler propriedades e relações do objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Criar iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_create.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Excluir iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_delete.md)|Nenhum|Excluir um [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|
|[Atualizar iosGeneralDeviceConfiguration](../api/intune_deviceconfig_iosgeneraldeviceconfiguration_update.md)|[iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md)|Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune_deviceconfig_iosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|accountBlockModification|Booleano|Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.|
|activationLockAllowWhenSupervised|Booleano|Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.|
|airDropBlocked|Booleano|Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.|
|airDropForceUnmanagedDropTarget|Booleano|Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).|
|airPlayForcePairingPasswordForOutgoingRequests|Booleano|Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.|
|appleWatchBlockPairing|Booleano|Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appleWatchForceWristDetection|Booleano|Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).|
|appleNewsBlocked|Booleano|Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appsSingleAppModeList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único. Apenas em modo supervisionado. iOS 7.0 e posterior. Esta coleção pode conter um máximo de 500 elementos.|
|appsVisibilityList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior). Essa coleção pode conter um máximo de 10.000 elementos.|
|appsVisibilityListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|Tipo de lista que está na AppsVisibilityList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|appStoreBlockAutomaticDownloads|Booleano|Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|appStoreBlocked|Booleano|Indica se o usuário será ou não impedido de usar a App Store.|
|appStoreBlockInAppPurchases|Booleano|Indica se o usuário será ou não impedido de fazer compras no aplicativo.|
|appStoreBlockUIAppInstallation|Booleano|Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host. Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).|
|appStoreRequirePassword|Booleano|Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.|
|bluetoothBlockModification|Booleano|Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).|
|cameraBlocked|Booleano|Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|cellularBlockDataRoaming|Booleano|Indica se o roaming de dados deve ou não ser bloqueado.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Booleano|Indica se a busca global em segundo plano será ou não bloqueada durante roaming.|
|cellularBlockPerAppDataModification|Booleano|Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.|
|cellularBlockPersonalHotspot|Booleano|Indica se o hotspot pessoal deve ou não ser bloqueado.|
|cellularBlockVoiceRoaming|Booleano|Indica se o roaming de voz deve ou não ser bloqueado.|
|certificatesBlockUntrustedTlsCertificates|Booleano|Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.|
|classroomAppBlockRemoteScreenObservation|Booleano|Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).|
|classroomAppForceUnpromptedScreenObservation|Booleano|Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.|
|compliantAppsList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|Lista que está na AppComplianceList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|configurationProfileBlockChanges|Booleano|Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.|
|definitionLookupBlocked|Booleano|Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|deviceBlockEnableRestrictions|Booleano|Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.|
|deviceBlockEraseContentAndSettings|Booleano|Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.|
|deviceBlockNameModification|Booleano|Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|diagnosticDataBlockSubmission|Booleano|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|diagnosticDataBlockSubmissionModification|Booleano|Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).|
|documentsBlockManagedDocumentsInUnmanagedApps|Booleano|Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.|
|documentsBlockUnmanagedDocumentsInManagedApps|Booleano|Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.|
|emailInDomainSuffixes|Coleção de sequência de caracteres|Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.|
|enterpriseAppBlockTrust|Booleano|Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.|
|enterpriseAppBlockTrustModification|Booleano|Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.|
|faceTimeBlocked|Booleano|Indica se o usuário será ou não impedido de usar o FaceTime.|
|findMyFriendsBlocked|Booleano|Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.|
|gamingBlockGameCenterFriends|Booleano|Indica se o usuário será ou não impedido de ter amigos no Game Center.|
|gamingBlockMultiplayer|Booleano|Indica se o usuário será ou não impedido de usar jogos para vários participantes.|
|gameCenterBlocked|Booleano|Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.|
|hostPairingBlocked|Booleano|indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.|
|iBooksStoreBlocked|Booleano|Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.|
|iBooksStoreBlockErotica|Booleano|Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.|
|iCloudBlockActivityContinuation|Booleano|Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.|
|iCloudBlockBackup|Booleano|Indica se o backup do iCloud deve ou não ser bloqueado.|
|iCloudBlockDocumentSync|Booleano|Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.|
|iCloudBlockManagedAppsSync|Booleano|Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.|
|iCloudBlockPhotoLibrary|Booleano|Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.|
|iCloudBlockPhotoStreamSync|Booleano|Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.|
|iCloudBlockSharedPhotoStream|Booleano|Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.|
|iCloudRequireEncryptedBackup|Booleano|Indica se a criptografia de backups no iCloud será exigida ou não.|
|iTunesBlockExplicitContent|Booleano|Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.|
|iTunesBlockMusicService|Booleano|Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).|
|iTunesBlockRadio|Booleano|Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).|
|keyboardBlockAutoCorrect|Booleano|Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|keyboardBlockDictation|Booleano|Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.|
|keyboardBlockPredictive|Booleano|Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|keyboardBlockShortcuts|Booleano|Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).|
|keyboardBlockSpellCheck|Booleano|Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).|
|kioskModeAllowAssistiveSpeak|Booleano|Indica se a fala assistencial será permitida ou não no modo quiosque.|
|kioskModeAllowAssistiveTouchSettings|Booleano|Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.|
|kioskModeAllowAutoLock|Booleano|Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.|
|kioskModeAllowColorInversionSettings|Booleano|Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.|
|kioskModeAllowRingerSwitch|Booleano|Indica se o uso do botão de toque será permitido ou não no modo quiosque.|
|kioskModeAllowScreenRotation|Booleano|Indica se a rotação de tela será permitida ou não no modo quiosque.|
|kioskModeAllowSleepButton|Booleano|Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.|
|kioskModeAllowTouchscreen|Booleano|Indica se o uso da tela touch será permitido ou não no modo quiosque.|
|kioskModeAllowVoiceOverSettings|Booleano|Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.|
|kioskModeAllowVolumeButtons|Booleano|Indica se o uso dos botões de volume será permitido ou não no modo quiosque.|
|kioskModeAllowZoomSettings|Booleano|Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.|
|kioskModeAppStoreUrl|Cadeia de caracteres|URL na loja de aplicativos do aplicativo para uso no modo de quiosque. Use se KioskModeManagedAppId não for conhecido.|
|kioskModeBuiltInAppId|Sequência de caracteres|ID para aplicativos internos a ser usado para o modo de quiosque. Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidas.|
|kioskModeRequireAssistiveTouch|Booleano|Indica se o toque assistencial deve ou não ser exigido no modo quiosque.|
|kioskModeRequireColorInversion|Booleano|Indica se a inversão de cores deve ou não ser exigida no modo quiosque.|
|kioskModeRequireMonoAudio|Booleano|Indica se o áudio mono deve ou não ser exigido no modo quiosque.|
|kioskModeRequireVoiceOver|Booleano|Indica se o voice over deve ou não ser exigido no modo quiosque.|
|kioskModeRequireZoom|Booleano|Indica se o zoom deve ou não ser exigido no modo quiosque.|
|kioskModeManagedAppId|Cadeia de caracteres|ID de gerenciamento do aplicativo para uso no modo de quiosque. Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.|
|lockScreenBlockControlCenter|Booleano|Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.|
|lockScreenBlockNotificationView|Booleano|Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.|
|lockScreenBlockPassbook|Booleano|Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado|
|lockScreenBlockTodayView|Booleano|Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/intune_deviceconfig_mediacontentratingaustralia.md)|Configurações de classificação de conteúdo de mídia da Austrália|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/intune_deviceconfig_mediacontentratingcanada.md)|Configurações de classificação de conteúdo de mídia do Canadá|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/intune_deviceconfig_mediacontentratingfrance.md)|Configurações de classificação de conteúdo de mídia da França|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/intune_deviceconfig_mediacontentratinggermany.md)|Configurações de classificação de conteúdo de mídia da Alemanha|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/intune_deviceconfig_mediacontentratingireland.md)|Configurações de classificação de conteúdo de mídia da Irlanda|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/intune_deviceconfig_mediacontentratingjapan.md)|Configurações de classificação de conteúdo de mídia do Japão|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/intune_deviceconfig_mediacontentratingnewzealand.md)|Configurações de classificação de conteúdo de mídia da Nova Zelândia|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/intune_deviceconfig_mediacontentratingunitedkingdom.md)|Configurações de classificação de conteúdo de mídia do Reino Unido|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/intune_deviceconfig_mediacontentratingunitedstates.md)|Configurações de classificação de conteúdo de mídia dos Estados Unidos|
|networkUsageRules|Coleção [iosNetworkUsageRule](../resources/intune_deviceconfig_iosnetworkusagerule.md)|Lista de aplicativos gerenciados e regras de rede que se aplicam a eles. Essa coleção pode conter um máximo de 1.000 elementos.|
|mediaContentRatingApps|[ratingAppsType](../resources/intune_deviceconfig_ratingappstype.md)|Configurações de classificação de conteúdo de mídia para aplicativos. Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|messagesBlocked|Booleano|Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.|
|notificationsBlockSettingsModification|Booleano|Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).|
|passcodeBlockFingerprintUnlock|Booleano|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passcodeBlockFingerprintModification|Booleano|Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.|
|passcodeBlockModification|Booleano|Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).|
|passcodeBlockSimple|Booleano|Indica se códigos de acesso simples devem ou não ser bloqueados.|
|passcodeExpirationDays|Int32|Número de dias antes da expiração do código de acesso. Valores válidos de 1 a 65535|
|passcodeMinimumLength|Int32|Comprimento mínimo do código de acesso. Valores válidos de 4 a 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que um código de acesso seja necessário.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passcodeMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter. Valores válidos de 0 a 4|
|passcodePreviousPasscodeBlockCount|Int32|Número de códigos de acesso anteriores para bloquear. Valores válidos de 1 a 24|
|passcodeSignInFailureCountBeforeWipe|Int32|Número permitido de falhas de entrada antes da limpeza do dispositivo. Valores válidos de 4 a 11|
|passcodeRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Booleano|Indica se um código de acesso deve ou não ser exigido.|
|podcastsBlocked|Booleano|Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).|
|safariBlockAutofill|Booleano|Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.|
|safariBlockJavaScript|Booleano|Indica se o JavaScript deve ou não ser bloqueado no Safari.|
|safariBlockPopups|Booleano|Indica se os popups devem ou não ser bloqueados no Safari.|
|safariBlocked|Booleano|Indica se o usuário será ou não impedido de usar o Safari.|
|safariCookieSettings|[webBrowserCookieSettings](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|Configurações de cookie do Safari. Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|Coleção de sequência de caracteres|As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.|
|safariPasswordAutoFillDomains|Coleção de sequência de caracteres|Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui. Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).|
|safariRequireFraudWarning|Booleano|Indica se um aviso de fraude deve ou não ser exigido no Safari.|
|screenCaptureBlocked|Booleano|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|siriBlocked|Booleano|Indica se o usuário será ou não impedido de usar a Siri.|
|siriBlockedWhenLocked|Booleano|Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.|
|siriBlockUserGeneratedContent|Booleano|Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.|
|siriRequireProfanityFilter|Booleano|Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.|
|spotlightBlockInternetResults|Booleano|Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.|
|voiceDialingBlocked|Booleano|Indica se a discagem de voz deve ou não ser bloqueada.|
|wallpaperBlockModification|Booleano|Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).|
|wiFiConnectOnlyToConfiguredNetworks|Booleano|Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração de dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosGeneralDeviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
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
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityListType": "String",
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
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
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
    "String"
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
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeBuiltInAppId": "String",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "String",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "String",
    "tvRating": "String"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "String",
          "publisher": "String",
          "appStoreUrl": "String",
          "appId": "String"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "String",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeSignInFailureCountBeforeWipe": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "String",
  "safariManagedDomains": [
    "String"
  ],
  "safariPasswordAutoFillDomains": [
    "String"
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
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```








