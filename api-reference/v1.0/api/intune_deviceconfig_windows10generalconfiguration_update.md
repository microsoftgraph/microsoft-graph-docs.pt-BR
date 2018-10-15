# <a name="update-windows10generalconfiguration"></a>Atualizar windows10GeneralConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

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
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|Token&gt; de portador obrigatório.&lt;|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|enterpriseCloudPrintDiscoveryEndPoint|Cadeia de caracteres|Ponto de extremidade para descoberta de impressoras na nuvem.|
|enterpriseCloudPrintOAuthAuthority|Cadeia de caracteres|Ponto de extremidade para aquisição de tokens OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|Cadeia de caracteres|GUID de um aplicativo cliente autorizado a recuperar tokens OAuth da autoridade OAuth.|
|enterpriseCloudPrintResourceIdentifier|Cadeia de caracteres|URI do recurso OAuth para serviço de impressão, conforme configurado no portal do Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Número máximo de impressoras que devem ser consultadas em um ponto de extremidade de descoberta. Esta é uma configuração somente para dispositivos móveis. Valores válidos de 1 a 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|Cadeia de caracteres|URI do recurso OAuth para serviço de descoberta de impressoras, conforme configurado no portal do Azure.|
|searchBlockDiacritics|Booleano|Especifica se a pesquisa pode usar diacríticos.|
|searchDisableAutoLanguageDetection|Booleano|Especifica se a detecção automática de idioma será usada ao indexar conteúdo e propriedades.|
|searchDisableIndexingEncryptedItems|Booleano|Indica se a indexação de itens protegidos por WIP será bloqueada ou não para que eles não apareçam nos resultados de pesquisa da Cortana ou do Explorer.|
|searchEnableRemoteQueries|Booleano|Indica se as consultas remotas do índice deste computador serão bloqueadas ou não.|
|searchDisableIndexerBackoff|Booleano|Indica se o recurso de retirada de indexador de pesquisa deve ou não ser desativado.|
|searchDisableIndexingRemovableDrive|Booleano|Indica se os usuários poderão ou não adicionar locais de unidades removíveis a bibliotecas e para serem indexados.|
|searchEnableAutomaticIndexSizeManangement|Booleano|Especifica uma quantidade mínima de espaço em disco rígido na mesma unidade como o local do índice antes que a indexação seja interrompida.|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune_deviceconfig_diagnosticdatasubmissionmode.md)|Obtém ou define um valor, permitindo que o dispositivo envie diagnóstico e dados telemétricos de uso, como Watson. Os valores possíveis são: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Booleano|Obtém ou define um valor para permitir que os administradores de TI impeçam aplicativos e recursos de trabalhar com arquivos no OneDrive.|
|smartScreenEnableAppInstallControl|Booleano|Permite que os administradores de TI controlem se os usuários poderão instalar aplicativos de lugares que não sejam a Store.|
|personalizationDesktopImageUrl|Cadeia de caracteres|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da área de trabalho ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da área de trabalho.|
|personalizationLockScreenImageUrl|Cadeia de caracteres|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da tela de bloqueio ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da tela de bloqueio.|
|bluetoothAllowedServices|Coleção de sequência de caracteres|Especifica uma lista de serviços e perfis Bluetooth permitidos em cadeias de caracteres de formato hexadecimal.|
|bluetoothBlockAdvertising|Booleano|Se o usuário será ou não impedido de usar a publicidade do bluetooth.|
|bluetoothBlockDiscoverableMode|Booleano|Se o usuário será ou não impedido de usar o modo de descoberta de bluetooth.|
|bluetoothBlockPrePairing|Booleano|Se determinados periféricos Bluetooth agrupados serão bloqueados ou não do emparelhamento automático com o dispositivo host.|
|edgeBlockAutofill|Booleano|Indica se o preenchimento automático deve ou não ser bloqueado.|
|edgeBlocked|Booleano|Indica se o usuário será ou não impedido de usar o navegador Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune_deviceconfig_edgecookiepolicy.md)|Indica quais cookies bloquear no navegador Edge. Os valores possíveis são: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Booleano|Indica se as ferramentas de desenvolvedor serão bloqueadas ou não no navegador Edge.|
|edgeBlockSendingDoNotTrackHeader|Booleano|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|edgeBlockExtensions|Booleano|Indica se as extensões serão bloqueadas ou não no navegador Edge.|
|edgeBlockInPrivateBrowsing|Booleano|Indica se a navegação InPrivate será bloqueada ou não em redes corporativas no navegador Edge.|
|edgeBlockJavaScript|Booleano|Indica se o usuário será ou não impedido de usar JavaScript.|
|edgeBlockPasswordManager|Booleano|Indica se o gerenciador de senhas será bloqueado ou não.|
|edgeBlockAddressBarDropdown|Booleano|Bloquear a funcionalidade de menu suspenso da barra de endereços no Microsoft Edge. Desabilite essa configuração para minimizar as conexões de rede do Microsoft Edge com serviços Microsoft.|
|edgeBlockCompatibilityList|Booleano|Bloquear lista de compatibilidade da Microsoft no Microsoft Edge. Essa lista da Microsoft ajuda o Edge a exibir corretamente sites com problemas de compatibilidade conhecidos.|
|edgeClearBrowsingDataOnExit|Booleano|Limpar dados de navegação ao sair do Microsoft Edge.|
|edgeAllowStartPagesModification|Booleano|Permitir que os usuários alterem as páginas iniciais no Edge. Use EdgeHomepageUrls para especificar as páginas iniciais que o usuário verá por padrão ao abrir o Edge.|
|edgeDisableFirstRunPage|Booleano|Bloquear a página da Web da Microsoft que é aberta na primeira utilização do Microsoft Edge. Esta política permite que empresas, como aquelas registradas em configurações de emissões zero, bloqueiem esta página.|
|edgeBlockLiveTileDataCollection|Booleano|Bloquear a coleta de informações da Microsoft para criação de bloco dinâmico quando os usuários fixarem um site para iniciar no Microsoft Edge.|
|edgeSyncFavoritesWithInternetExplorer|Booleano|Habilitar a sincronização de favoritos entre o Internet Explorer e o Microsoft Edge. Adições, exclusões, modificações e outras alterações para favoritos são compartilhadas entre navegadores.|
|cellularBlockDataWhenRoaming|Booleano|Se o usuário será ou não impedido de usar dados da rede celular durante roaming.|
|cellularBlockVpn|Booleano|Se o usuário será ou não impedido de usar VPN na rede celular.|
|cellularBlockVpnWhenRoaming|Booleano|Se o usuário será ou não impedido de usar VPN durante roaming na rede celular.|
|defenderBlockEndUserAccess|Booleano|Se o usuário final será ou não impedido de acessar o Defender.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Número de dias antes da exclusão do malware em quarentena. Valores válidos de 0 a 90|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune_deviceconfig_defenderdetectedmalwareactions.md)|Obtém ou define ações do Defender a serem realizadas em um malware detectado por nível de ameaça.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune_deviceconfig_weeklyschedule.md)|Dia da semana para varredura do sistema pelo Defender. Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|Coleção de sequência de caracteres|Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.|
|defenderFileExtensionsToExclude|Coleção de sequência de caracteres|Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.|
|defenderScanMaxCpu|Int32|Porcentagem máxima de uso da CPU durante a verificação. Valores válidos de 0 a 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune_deviceconfig_defendermonitorfileactivity.md)|Valor para monitorar a atividade do arquivo. Os valores possíveis são: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderProcessesToExclude|Coleção de sequência de caracteres|Processos a serem excluídos das verificações e da proteção em tempo real.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune_deviceconfig_defenderpromptforsamplesubmission.md)|A configuração sobre como solicitar ao usuário o envio da amostra. Os valores possíveis são: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Booleano|Indica se o monitoramento de comportamento deve ou não ser exigido.|
|defenderRequireCloudProtection|Booleano|Indica se a proteção na nuvem deve ou não ser exigida.|
|defenderRequireNetworkInspectionSystem|Booleano|Indica se o sistema de inspeção de rede deve ou não ser exigido.|
|defenderRequireRealTimeMonitoring|Booleano|Indica se o monitoramento em tempo real deve ou não ser exigido.|
|defenderScanArchiveFiles|Booleano|Indica se os arquivos mortos devem ou não ser verificados.|
|defenderScanDownloads|Booleano|Indica se os downloads devem ou não ser verificados.|
|defenderScanNetworkFiles|Booleano|Indica se os arquivos abertos de uma pasta da rede devem ou não ser verificados.|
|defenderScanIncomingMail|Booleano|Indica se as mensagens de email de entrada devem ou não ser verificadas.|
|defenderScanMappedNetworkDrivesDuringFullScan|Booleano|Indica se as unidades de rede mapeadas devem ou não ser verificadas durante a verificação completa.|
|defenderScanRemovableDrivesDuringFullScan|Booleano|Indica se as unidades removíveis devem ou não ser verificadas durante a verificação completa.|
|defenderScanScriptsLoadedInInternetExplorer|Booleano|Indica se os scripts carregados no navegador Internet Explorer devem ou não ser verificados.|
|defenderSignatureUpdateIntervalInHours|Int32|O intervalo de atualização da assinatura em horas. Especifique 0 para não verificar. Valores válidos de 0 a 24|
|defenderScanType|[defenderScanType](../resources/intune_deviceconfig_defenderscantype.md)|O tipo de varredura do sistema do Defender. Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|A hora em que o Defender fará a verificação do sistema.|
|defenderScheduledQuickScanTime|TimeOfDay|O horário de realização da verificação diária rápida.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune_deviceconfig_defendercloudblockleveltype.md)|Especifica o nível de proteção entregue na nuvem. Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|lockScreenAllowTimeoutConfiguration|Booleano|Especifique se deseja mostrar uma definição configurável pelo usuário para controlar o tempo limite da tela enquanto estiver na tela de bloqueio de dispositivos Windows Mobile 10. Se essa política estiver definida como Permitir, o valor definido por lockScreenTimeoutInSeconds será ignorado.|
|lockScreenBlockActionCenterNotifications|Booleano|Indica se as notificações da central de ações na tela de bloqueio serão bloqueadas.|
|lockScreenBlockCortana|Booleano|Indica se o usuário pode ou não interagir com a Cortana usando a fala enquanto o sistema estiver bloqueado.|
|lockScreenBlockToastNotifications|Booleano|Indica se serão permitidas notificações do sistema acima da tela de bloqueio do dispositivo.|
|lockScreenTimeoutInSeconds|Int32|Defina a duração (em segundos) da tela de bloqueio para a tela em desligamento para dispositivos Windows Mobile 10. Os valores compatíveis ficam entre 11 e 1800. Valores válidos de 11 a 1800|
|passwordBlockSimple|Booleano|Especifique se PINs ou senhas como "1111" ou "1234" são permitidas. Para computadores do Windows 10, isso também controla o uso de senhas com imagem.|
|passwordExpirationDays|Int32|A expiração da senha em dias. Valores válidos de 0 a 730|
|passwordMinimumLength|Int32|O comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 50|
|passwordRequired|Booleano|Indica se um usuário deverá ou não ter uma senha.|
|passwordRequireWhenResumeFromIdleState|Booleano|Indica se uma senha deve ou não ser exigida ao sair de um estado inativo.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica. Valores válidos de 0 a 999|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Habilita ou desabilita o uso da ID de publicidade. Adicionado ao Windows 10, versão 1607. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Booleano|Indica se será permitida ou não a aceitação automática da caixa de diálogo de consentimento do usuário com emparelhamento e privacidade ao iniciar aplicativos.|
|privacyBlockInputPersonalization|Booleano|Indica se o uso dos serviços de fala baseados na nuvem será bloqueado para os aplicativos Cortana, Ditado ou Store.|
|startBlockUnpinningAppsFromTaskbar|Booleano|Indica se o usuário será ou não impedido de desafixar aplicativos da barra de tarefas.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune_deviceconfig_windowsstartmenuapplistvisibilitytype.md)|A definição desse valor recolhe a lista de aplicativos, remove a lista de aplicativos totalmente ou desabilita a alternância correspondente no aplicativo de Configurações. Os valores possíveis são: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Booleano|Habilitar essa política impede a exibição da configuração de conta de alteração no bloco de usuário no menu Iniciar.|
|startMenuHideFrequentlyUsedApps|Booleano|Habilitar essa política impede a exibição dos aplicativos mais usados no menu Iniciar e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideHibernate|Booleano|Habilitar essa política impede a exibição da hibernação no botão de energia no menu Iniciar.|
|startMenuHideLock|Booleano|Habilitar essa política impede a exibição do bloqueio no bloco de usuário no menu Iniciar.|
|startMenuHidePowerButton|Booleano|Habilitar essa política impede a exibição do botão de energia no menu Iniciar.|
|startMenuHideRecentJumpLists|Booleano|Habilitar essa política impede a exibição de listas de atalhos recentes no menu Iniciar/barra de tarefas e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideRecentlyAddedApps|Booleano|Habilitar essa política impede a exibição de aplicativos adicionados recentemente no menu Iniciar e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideRestartOptions|Booleano|Habilitar essa política impede a exibição da opção “Reiniciar/Atualizar e Reiniciar” no botão de energia no menu Iniciar.|
|startMenuHideShutDown|Booleano|Habilitar essa política impede a exibição da opção desligar/atualizar e desligar no botão de energia no menu Iniciar.|
|startMenuHideSignOut|Booleano|Habilitar essa política impede a exibição da opção Sair no bloco de usuário no menu Iniciar.|
|startMenuHideSleep|Booleano|Habilitar essa política impede a exibição da suspensão no botão de energia no menu Iniciar.|
|startMenuHideSwitchAccount|Booleano|Habilitar essa política impede a exibição da opção Alternar conta no bloco de usuário no menu Iniciar.|
|startMenuHideUserTile|Booleano|Habilitar essa política impede a exibição do bloco de usuário no menu Iniciar.|
|startMenuLayoutEdgeAssetsXml|Binária|Essa configuração de política permite importar ativos do Edge a serem usados com a política startMenuLayoutXml. O layout inicial pode conter um bloco secundário do aplicativo Microsoft Edge que procura pelo arquivo do ativo local do Edge. Nesse caso, o ativo local do Edge não existiria e faria com que o bloco secundário do Edge aparecesse vazio. Essa política só é aplicada quando a política startMenuLayoutXml é modificada. O valor deve ser uma matriz de bytes codificada em Base64 UTF-8.|
|startMenuLayoutXml|Binária|Permite aos administradores substituir o layout padrão do menu Iniciar e impede que o usuário o altere. O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. O XML deve estar em um formato de matriz de bytes codificada em UTF8.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune_deviceconfig_windowsstartmenumodetype.md)|Permite que os administradores decidam como o menu Iniciar será exibido. Os valores possíveis são: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Documentos no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Downloads no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho FileExplorer no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta HomeGroup no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Música no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Rede no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho PersonalFolder no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Imagens no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Configurações no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune_deviceconfig_visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Vídeos no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Booleano|Indica se o acesso ao aplicativo Configurações deve ou não ser bloqueado.|
|settingsBlockSystemPage|Booleano|Indica se o acesso ao Sistemas deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockDevicesPage|Booleano|Indica se o acesso a Dispositivos deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockNetworkInternetPage|Booleano|Indica se o acesso a Rede e Internet deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockPersonalizationPage|Booleano|Indica se o acesso a Personalização deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockAccountsPage|Booleano|Indica se o acesso a Contas deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockTimeLanguagePage|Booleano|Indica se o acesso a Hora e Idioma deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockEaseOfAccessPage|Booleano|Indica se o acesso à Facilidade de Acesso deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockPrivacyPage|Booleano|Indica se o acesso à Privacidade deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockUpdateSecurityPage|Booleano|Indica se o acesso a Atualização e Segurança deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockAppsPage|Booleano|Indica se o acesso a Aplicativos deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockGamingPage|Booleano|Indica se o acesso a Jogos deve ou não ser bloqueado no aplicativo Configurações.|
|windowsSpotlightBlockConsumerSpecificFeatures|Booleano|Permite que os administradores de TI bloqueiem experiências que normalmente são apenas para consumidores, como Sugestões de início, Notificações de associação, instalação de aplicativo pós-OOBE e redirecionamento de blocos.|
|windowsSpotlightBlocked|Booleano|Permite que os administradores de TI desativem todos os recursos do Destaque do Windows|
|windowsSpotlightBlockOnActionCenter|Booleano|Bloquear sugestões da Microsoft mostradas após cada instalação limpa do sistema operacional, após upgrades ou de modo contínuo para apresentar aos usuários as novidades ou alterações|
|windowsSpotlightBlockTailoredExperiences|Booleano|Bloquear conteúdo personalizado no Destaque do Windows com base no uso do dispositivo pelo usuário.|
|windowsSpotlightBlockThirdPartyNotifications|Booleano|Bloquear conteúdo de terceiros fornecido por meio do Destaque do Windows|
|windowsSpotlightBlockWelcomeExperience|Booleano|Bloquear a experiência de boas-vindas do Destaque do Windows|
|windowsSpotlightBlockWindowsTips|Booleano|Permite que os administradores de TI desativem os popups de Dicas do Windows.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune_deviceconfig_windowsspotlightenablementsettings.md)|Especifica o tipo de Destaque Os valores possíveis são: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Booleano|Se definida, as configurações de proxy serão aplicadas a todos os processos e contas no dispositivo. Caso contrário, serão aplicadas à conta de usuário registrada no MDM.|
|networkProxyDisableAutoDetect|Booleano|Desabilitar a detecção automática de configurações. Se habilitada, o sistema tentará encontrar o caminho para um script de configuração automática de proxy (PAC).|
|networkProxyAutomaticConfigurationUrl|Cadeia de caracteres|Endereço para o script de configuração automática de proxy (PAC) desejado.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune_deviceconfig_windows10networkproxyserver.md)|Especifica configurações manuais de servidor proxy.|
|accountsBlockAddingNonMicrosoftAccountEmail|Booleano|Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.|
|antiTheftModeBlocked|Booleano|Indica se o usuário será ou não impedido de selecionar a preferência do modo AntiTheft (somente no Windows 10 Mobile).|
|bluetoothBlocked|Booleano|Se o usuário será ou não impedido de usar o bluetooth.|
|cameraBlocked|Booleano|Se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|connectedDevicesServiceBlocked|Booleano|Se serão bloqueados ou não o serviço de dispositivos conectados, que permite a descoberta e conexão de outros dispositivos, mensagens remotas, sessões de aplicativo remoto e outras experiências entre dispositivos.|
|certificatesBlockManualRootCertificateInstallation|Booleano|Se o usuário será ou não impedido de fazer a instalação manual do certificado raiz.|
|copyPasteBlocked|Booleano|Se o usuário será ou não impedido de usar a função copiar/colar.|
|cortanaBlocked|Booleano|Se o usuário será ou não impedido de usar a Cortana.|
|deviceManagementBlockFactoryResetOnMobile|Booleano|Se o usuário será ou não impedido de redefinir o telefone.|
|deviceManagementBlockManualUnenroll|Booleano|Indica se o usuário será ou não impedido de cancelar manualmente o registro no gerenciamento de dispositivo.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune_deviceconfig_safesearchfiltertype.md)|Especifica qual nível de filtro de pesquisa segura é necessário. Os valores possíveis são: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Booleano|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|edgeBlockSearchSuggestions|Booleano|Indica se o usuário será ou não impedido de usar as sugestões de pesquisa na barra de endereços.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Booleano|Indica se o usuário será ou não impedido de enviar tráfego da Intranet para o Internet Explorer a partir do Edge.|
|edgeRequireSmartScreen|Booleano|Indica se o usuário deverá ou não usar o Filtro SmartScreen.|
|edgeEnterpriseModeSiteListLocation|Cadeia de caracteres|Indica o local da lista de sites do modo Empresarial. Pode ser um arquivo local, rede local ou local http.|
|edgeFirstRunUrl|Cadeia de caracteres|A primeira URL a ser executada quando o navegador Edge é aberto pela primeira vez.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)|Permite aos administradores de TI definir um mecanismo de pesquisa padrão para dispositivos controlados por MDM. Os usuários podem substituí-lo e alterar o mecanismo de pesquisa padrão fornecido, caso a política AllowSearchEngineCustomization não esteja definida.|
|edgeHomepageUrls|Coleção de sequência de caracteres|A lista de URLs de home pages mostradas em dispositivos registrados no MDM no navegador Edge.|
|edgeBlockAccessToAboutFlags|Booleano|Indica se será impedido ou não o acesso a sinalizadores Sobre no navegador Edge.|
|smartScreenBlockPromptOverride|Booleano|Indica se os usuários poderão ou não substituir avisos do Filtro SmartScreen sobre sites potencialmente maliciosos.|
|smartScreenBlockPromptOverrideForFiles|Booleano|Indica se os usuários poderão ou não substituir os avisos do Filtro SmartScreen sobre sites baixados não verificados.|
|webRtcBlockLocalhostIpAddress|Booleano|Indica se o endereço IP do localhost do usuário será ou não exibido durante chamadas telefônicas usando o WebRTC|
|internetSharingBlocked|Booleano|Indica se o usuário será ou não impedido de usar o compartilhamento de Internet.|
|settingsBlockAddProvisioningPackage|Booleano|Indica se o usuário será ou não impedido de instalar pacotes de provisionamento.|
|settingsBlockRemoveProvisioningPackage|Booleano|Indica se o agente de configuração de tempo de execução será ou não impedido de remover pacotes de provisionamento.|
|settingsBlockChangeSystemTime|Booleano|Indica se o usuário será ou não impedido de alterar configurações de data e hora.|
|settingsBlockEditDeviceName|Booleano|Indica se o usuário será ou não impedido de editar o nome do dispositivo.|
|settingsBlockChangeRegion|Booleano|Indica se o usuário será ou não impedido de alterar as configurações de região.|
|settingsBlockChangeLanguage|Booleano|Indica se o usuário será ou não impedido de alterar as configurações de idioma.|
|settingsBlockChangePowerSleep|Booleano|Indica se o usuário será ou não impedido de alterar as configurações de energia e suspensão.|
|locationServicesBlocked|Booleano|Indica se o usuário será ou não bloqueado dos serviços de localização.|
|microsoftAccountBlocked|Booleano|Indica se uma conta da Microsoft será ou não bloqueada.|
|microsoftAccountBlockSettingsSync|Booleano|Indica se a sincronização de configurações da conta da Microsoft será ou não bloqueada.|
|nfcBlocked|Booleano|Indica se o usuário será ou não impedido de usar a comunicação a curta distância.|
|resetProtectionModeBlocked|Booleano|Indica se o usuário será ou não bloqueado do modo de proteção contra restauração de fábrica.|
|screenCaptureBlocked|Booleano|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|storageBlockRemovableStorage|Booleano|Indica se o usuário será ou não impedido de usar o armazenamento removível.|
|storageRequireMobileDeviceEncryption|Booleano|Indica se a criptografia é ou não necessária em um dispositivo móvel.|
|usbBlocked|Booleano|Indica se o usuário será ou não bloqueado da conexão USB.|
|voiceRecordingBlocked|Booleano|Indica se o usuário será ou não bloqueado da gravação de voz.|
|wiFiBlockAutomaticConnectHotspots|Booleano|Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada. Não terá impacto se o Wi-Fi estiver bloqueado.|
|wiFiBlocked|Booleano|Indica se o usuário será ou não impedido de usar o Wi-Fi.|
|wiFiBlockManualConfiguration|Booleano|Indica se o usuário será ou não impedido de usar a configuração manual do Wi-Fi.|
|wiFiScanInterval|Int32|Especificar com que frequência os dispositivos procuram redes Wi-Fi. Os valores compatíveis ficam entre 1 e 500, em que 100 = padrão e 500 = frequência baixa. Valores válidos de 1 a 500|
|wirelessDisplayBlockProjectionToThisDevice|Booleano|Indica se outros dispositivos poderão ou não descobrir este PC para fins de projeção.|
|wirelessDisplayBlockUserInputFromReceiver|Booleano|Indica se a entrada do usuário pelo receptor de vídeo sem fio será permitida ou não.|
|wirelessDisplayRequirePinForPairing|Booleano|Indica se será exigido um PIN para que novos dispositivo iniciem o emparelhamento.|
|windowsStoreBlocked|Booleano|Indica se o usuário será ou não impedido de usar a Windows Store.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Indica se os aplicativos dos pacotes AppX assinados com um certificado confiável podem fazer sideload. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Booleano|Indica se a atualização automática de aplicativos pela Windows Store será bloqueada ou não.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Indica se a permissão de desbloquear os desenvolvedores será feita ou não. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Booleano|Indica se vários usuários do mesmo aplicativo serão ou não impedidos de compartilhar dados.|
|appsBlockWindowsStoreOriginatedApps|Booleano|Indica se será desabilitada ou não a inicialização de todos os aplicativos da Windows Store pré-instalados ou baixados.|
|windowsStoreEnablePrivateStoreOnly|Booleano|Indica se o Repositório particular será ativado ou não.|
|storageRestrictAppDataToSystemVolume|Booleano|Indica se os dados do aplicativo ficarão restritos à unidade do sistema.|
|storageRestrictAppInstallToSystemVolume|Booleano|Indica se a instalação de aplicativos ficará restrita à unidade do sistema.|
|gameDvrBlocked|Booleano|Indica se DVR e difusão serão bloqueados ou não.|
|experienceBlockDeviceDiscovery|Booleano|Indica se a experiência de descoberta de dispositivos será ativada ou não.|
|experienceBlockErrorDialogWhenNoSIM|Booleano|Indica se a caixa de diálogo de erro poderá ou não ser exibida se nenhum cartão SIM for detectado.|
|experienceBlockTaskSwitcher|Booleano|Indica se a alternância de tarefas será ativada ou não no dispositivo.|
|logonBlockFastUserSwitching|Booleano|Desabilita a capacidade para alternar rapidamente entre os usuários conectados simultaneamente sem fazer logoff.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9699

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9875

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "smartScreenEnableAppInstallControl": true,
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyBlockInputPersonalization": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true
}
```








