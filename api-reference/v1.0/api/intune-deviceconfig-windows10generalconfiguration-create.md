---
title: Criar windows10GeneralConfiguration
description: Cria um novo objeto windows10GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12074071692cb7e44b5615feb329eb68f51b0cdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020189"
---
# <a name="create-windows10generalconfiguration"></a>Criar windows10GeneralConfiguration

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).

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
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windows10GeneralConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windows10GeneralConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|enterpriseCloudPrintDiscoveryEndPoint|String|Ponto de extremidade para descoberta de impressoras na nuvem.|
|enterpriseCloudPrintOAuthAuthority|String|Ponto de extremidade para aquisição de tokens OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID de um aplicativo cliente autorizado a recuperar tokens OAuth da autoridade OAuth.|
|enterpriseCloudPrintResourceIdentifier|String|URI do recurso OAuth para serviço de impressão, conforme configurado no portal do Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Número máximo de impressoras que devem ser consultadas em um ponto de extremidade de descoberta. Esta é uma configuração somente para dispositivos móveis. Valores válidos de 1 a 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|URI do recurso OAuth para serviço de descoberta de impressoras, conforme configurado no portal do Azure.|
|searchBlockDiacritics|Booliano|Especifica se a pesquisa pode usar diacríticos.|
|searchDisableAutoLanguageDetection|Booliano|Especifica se a detecção automática de idioma será usada ao indexar conteúdo e propriedades.|
|searchDisableIndexingEncryptedItems|Booliano|Indica se a indexação de itens protegidos por WIP será bloqueada ou não para que eles não apareçam nos resultados de pesquisa da Cortana ou do Explorer.|
|searchEnableRemoteQueries|Booliano|Indica se as consultas remotas do índice deste computador serão bloqueadas ou não.|
|searchDisableIndexerBackoff|Booliano|Indica se o recurso de retirada de indexador de pesquisa deve ou não ser desativado.|
|searchDisableIndexingRemovableDrive|Booliano|Indica se os usuários poderão ou não adicionar locais de unidades removíveis a bibliotecas e para serem indexados.|
|searchEnableAutomaticIndexSizeManangement|Booliano|Especifica uma quantidade mínima de espaço em disco rígido na mesma unidade como o local do índice antes que a indexação seja interrompida.|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Obtém ou define um valor que permite que o dispositivo envie dados de diagnóstico e de telemetria de uso, como Watson. Os valores possíveis são: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Booliano|Obtém ou define um valor para permitir que os administradores de TI impeçam aplicativos e recursos de trabalhar com arquivos no OneDrive.|
|smartScreenEnableAppInstallControl|Booliano|Permite que os administradores de TI controlem se os usuários poderão instalar aplicativos de lugares que não sejam a Store.|
|personalizationDesktopImageUrl|String|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da área de trabalho ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da área de trabalho.|
|personalizationLockScreenImageUrl|String|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da tela de bloqueio ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da tela de bloqueio.|
|bluetoothAllowedServices|String collection|Especifica uma lista de serviços e perfis Bluetooth permitidos em cadeias de caracteres de formato hexadecimal.|
|bluetoothBlockAdvertising|Booliano|Se o usuário será ou não impedido de usar a publicidade do bluetooth.|
|bluetoothBlockDiscoverableMode|Booliano|Se o usuário será ou não impedido de usar o modo de descoberta de bluetooth.|
|bluetoothBlockPrePairing|Booliano|Se determinados periféricos Bluetooth agrupados serão bloqueados ou não do emparelhamento automático com o dispositivo host.|
|edgeBlockAutofill|Boolean|Indica se o preenchimento automático deve ou não ser bloqueado.|
|edgeBlocked|Booliano|Indica se o usuário será ou não impedido de usar o navegador Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Indica quais cookies bloquear no navegador Edge. Os valores possíveis são: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Booliano|Indica se as ferramentas de desenvolvedor serão bloqueadas ou não no navegador Edge.|
|edgeBlockSendingDoNotTrackHeader|Booliano|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|edgeBlockExtensions|Booliano|Indica se as extensões serão bloqueadas ou não no navegador Edge.|
|edgeBlockInPrivateBrowsing|Booliano|Indica se a navegação InPrivate será bloqueada ou não em redes corporativas no navegador Edge.|
|edgeBlockJavaScript|Booliano|Indica se o usuário será ou não impedido de usar JavaScript.|
|edgeBlockPasswordManager|Booliano|Indica se o gerenciador de senhas será bloqueado ou não.|
|edgeBlockAddressBarDropdown|Booliano|Bloquear a funcionalidade de menu suspenso da barra de endereços no Microsoft Edge. Desabilite essa configuração para minimizar as conexões de rede do Microsoft Edge com serviços Microsoft.|
|edgeBlockCompatibilityList|Booliano|Bloquear lista de compatibilidade da Microsoft no Microsoft Edge. Essa lista da Microsoft ajuda o Edge a exibir corretamente sites com problemas de compatibilidade conhecidos.|
|edgeClearBrowsingDataOnExit|Booliano|Limpar dados de navegação ao sair do Microsoft Edge.|
|edgeAllowStartPagesModification|Booliano|Permitir que os usuários alterem as páginas iniciais no Edge. Use EdgeHomepageUrls para especificar as páginas iniciais que o usuário verá por padrão ao abrir o Edge.|
|edgeDisableFirstRunPage|Booliano|Bloquear a página da Web da Microsoft que é aberta na primeira utilização do Microsoft Edge. Esta política permite que empresas, como aquelas registradas em configurações de emissões zero, bloqueiem esta página.|
|edgeBlockLiveTileDataCollection|Booliano|Bloquear a coleta de informações da Microsoft para criação de bloco dinâmico quando os usuários fixarem um site para iniciar no Microsoft Edge.|
|edgeSyncFavoritesWithInternetExplorer|Booliano|Habilitar a sincronização de favoritos entre o Internet Explorer e o Microsoft Edge. Adições, exclusões, modificações e outras alterações para favoritos são compartilhadas entre navegadores.|
|cellularBlockDataWhenRoaming|Booliano|Se o usuário será ou não impedido de usar dados da rede celular durante roaming.|
|cellularBlockVpn|Booliano|Se o usuário será ou não impedido de usar VPN na rede celular.|
|cellularBlockVpnWhenRoaming|Booliano|Se o usuário será ou não impedido de usar VPN durante roaming na rede celular.|
|defenderBlockEndUserAccess|Booliano|Se o usuário final será ou não impedido de acessar o Defender.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Número de dias antes da exclusão do malware em quarentena. Valores válidos de 0 a 90|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Obtém ou define ações do Defender a serem realizadas em um malware detectado por nível de ameaça.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Dia da semana em que o Defender fará a verificação do sistema. Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|defenderFilesAndFoldersToExclude|Coleção de cadeias de caracteres|Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.|
|defenderFileExtensionsToExclude|Coleção de cadeias de caracteres|Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.|
|defenderScanMaxCpu|Int32|Porcentagem máxima de uso da CPU durante a verificação. Valores válidos de 0 a 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Valor de monitoramento da atividade do arquivo. Os valores possíveis são: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderProcessesToExclude|String collection|Processos a serem excluídos das verificações e da proteção em tempo real.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|A configuração do modo como avisar um usuário do envio de exemplo. Os valores possíveis são: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean|Indica se o monitoramento de comportamento deve ou não ser exigido.|
|defenderRequireCloudProtection|Booliano|Indica se a proteção na nuvem deve ou não ser exigida.|
|defenderRequireNetworkInspectionSystem|Booliano|Indica se o sistema de inspeção de rede deve ou não ser exigido.|
|defenderRequireRealTimeMonitoring|Booliano|Indica se o monitoramento em tempo real deve ou não ser exigido.|
|defenderScanArchiveFiles|Booliano|Indica se os arquivos mortos devem ou não ser verificados.|
|defenderScanDownloads|Booliano|Indica se os downloads devem ou não ser verificados.|
|defenderScanNetworkFiles|Booliano|Indica se os arquivos abertos de uma pasta da rede devem ou não ser verificados.|
|defenderScanIncomingMail|Booliano|Indica se as mensagens de email de entrada devem ou não ser verificadas.|
|defenderScanMappedNetworkDrivesDuringFullScan|Booliano|Indica se as unidades de rede mapeadas devem ou não ser verificadas durante a verificação completa.|
|defenderScanRemovableDrivesDuringFullScan|Booliano|Indica se as unidades removíveis devem ou não ser verificadas durante a verificação completa.|
|defenderScanScriptsLoadedInInternetExplorer|Booliano|Indica se os scripts carregados no navegador Internet Explorer devem ou não ser verificados.|
|defenderSignatureUpdateIntervalInHours|Int32|O intervalo de atualização da assinatura em horas. Especifique 0 para não verificar. Valores válidos de 0 a 24|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|O tipo de verificação do sistema do Defender. Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|A hora em que o Defender fará a verificação do sistema.|
|defenderScheduledQuickScanTime|TimeOfDay|O horário de realização da verificação diária rápida.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Especifica o nível de proteção oferecido na nuvem. Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|lockScreenAllowTimeoutConfiguration|Booliano|Especifique se deseja mostrar uma definição configurável pelo usuário para controlar o tempo limite da tela enquanto estiver na tela de bloqueio de dispositivos Windows Mobile 10. Se essa política estiver definida como Permitir, o valor definido por lockScreenTimeoutInSeconds será ignorado.|
|lockScreenBlockActionCenterNotifications|Booliano|Indica se as notificações da central de ações na tela de bloqueio serão bloqueadas.|
|lockScreenBlockCortana|Booliano|Indica se o usuário pode ou não interagir com a Cortana usando a fala enquanto o sistema estiver bloqueado.|
|lockScreenBlockToastNotifications|Booliano|Indica se serão permitidas notificações do sistema acima da tela de bloqueio do dispositivo.|
|lockScreenTimeoutInSeconds|Int32|Defina a duração (em segundos) da tela de bloqueio para a tela em desligamento para dispositivos Windows Mobile 10. Os valores compatíveis ficam entre 11 e 1800. Valores válidos de 11 a 1800|
|passwordBlockSimple|Booliano|Especifique se PINs ou senhas como "1111" ou "1234" são permitidas. Para computadores do Windows 10, isso também controla o uso de senhas com imagem.|
|passwordExpirationDays|Int32|A expiração da senha em dias. Valores válidos de 0 a 730|
|passwordMinimumLength|Int32|O comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 50|
|passwordRequired|Booliano|Indica se um usuário deverá ou não ter uma senha.|
|passwordRequireWhenResumeFromIdleState|Boolean|Indica se uma senha deve ou não ser exigida ao sair de um estado inativo.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica. Valores válidos de 0 a 999|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Habilita ou desabilita o uso da ID de publicidade. Adicionado no Windows 10, versão 1607. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Booliano|Indica se será permitida ou não a aceitação automática da caixa de diálogo de consentimento do usuário com emparelhamento e privacidade ao iniciar aplicativos.|
|privacyBlockInputPersonalization|Booliano|Indica se o uso dos serviços de fala baseados na nuvem será bloqueado para os aplicativos Cortana, Ditado ou Store.|
|startBlockUnpinningAppsFromTaskbar|Booliano|Indica se o usuário será ou não impedido de desafixar aplicativos da barra de tarefas.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|A definição desse valor recolhe a lista de aplicativos, remove a lista de aplicativos totalmente ou desabilita a alternância correspondente no aplicativo Configurações. Os valores possíveis são: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Booliano|Habilitar essa política impede a exibição da configuração de conta de alteração no bloco de usuário no menu Iniciar.|
|startMenuHideFrequentlyUsedApps|Booliano|Habilitar essa política impede a exibição dos aplicativos mais usados no menu Iniciar e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideHibernate|Booliano|Habilitar essa política impede a exibição da hibernação no botão de energia no menu Iniciar.|
|startMenuHideLock|Booliano|Habilitar essa política impede a exibição do bloqueio no bloco de usuário no menu Iniciar.|
|startMenuHidePowerButton|Booliano|Habilitar essa política impede a exibição do botão de energia no menu Iniciar.|
|startMenuHideRecentJumpLists|Booliano|Habilitar essa política impede a exibição de listas de atalhos recentes no menu Iniciar/barra de tarefas e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideRecentlyAddedApps|Booliano|Habilitar essa política impede a exibição de aplicativos adicionados recentemente no menu Iniciar e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideRestartOptions|Booliano|Habilitar essa política impede a exibição da opção “Reiniciar/Atualizar e Reiniciar” no botão de energia no menu Iniciar.|
|startMenuHideShutDown|Booliano|Habilitar essa política impede a exibição da opção desligar/atualizar e desligar no botão de energia no menu Iniciar.|
|startMenuHideSignOut|Booliano|Habilitar essa política impede a exibição da opção Sair no bloco de usuário no menu Iniciar.|
|startMenuHideSleep|Booliano|Habilitar essa política impede a exibição da suspensão no botão de energia no menu Iniciar.|
|startMenuHideSwitchAccount|Booliano|Habilitar essa política impede a exibição da opção Alternar conta no bloco de usuário no menu Iniciar.|
|startMenuHideUserTile|Boolean|Habilitar essa política impede a exibição do bloco de usuário no menu Iniciar.|
|startMenuLayoutEdgeAssetsXml|Binária|Essa configuração de política permite importar ativos do Edge a serem usados com a política startMenuLayoutXml. O layout inicial pode conter um bloco secundário do aplicativo Microsoft Edge que procura pelo arquivo do ativo local do Edge. Nesse caso, o ativo local do Edge não existiria e faria com que o bloco secundário do Edge aparecesse vazio. Essa política só é aplicada quando a política startMenuLayoutXml é modificada. O valor deve ser uma matriz de bytes codificada em Base64 UTF-8.|
|startMenuLayoutXml|Binária|Permite aos administradores substituir o layout padrão do menu Iniciar e impede que o usuário o altere. O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. O XML deve estar em um formato de matriz de bytes codificada em UTF8.|
|startMenuMode|[windowsStartMenuModeType](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|Permite aos administradores decidir como o menu Iniciar é exibido. Os valores possíveis são: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Documentos no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Downloads no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho do Explorador de Arquivos no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta HomeGroup no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Música no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Rede no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Pessoal no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Imagens no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Configurações no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Impõe a visibilidade (Mostrar/Ocultar) do atalho da pasta Vídeos no menu Iniciar. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|settingsBlockSettingsApp|Booliano|Indica se o acesso ao aplicativo Configurações deve ou não ser bloqueado.|
|settingsBlockSystemPage|Booliano|Indica se o acesso ao Sistemas deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockDevicesPage|Booliano|Indica se o acesso a Dispositivos deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockNetworkInternetPage|Booliano|Indica se o acesso a Rede e Internet deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockPersonalizationPage|Booliano|Indica se o acesso a Personalização deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockAccountsPage|Booliano|Indica se o acesso a Contas deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockTimeLanguagePage|Booliano|Indica se o acesso a Hora e idioma deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockEaseOfAccessPage|Booliano|Indica se o acesso à Facilidade de Acesso deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockPrivacyPage|Booliano|Indica se o acesso à Privacidade deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockUpdateSecurityPage|Booliano|Indica se o acesso a Atualização e Segurança deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockAppsPage|Booliano|Indica se o acesso a Aplicativos deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockGamingPage|Booliano|Indica se o acesso a Jogos deve ou não ser bloqueado no aplicativo Configurações.|
|windowsSpotlightBlockConsumerSpecificFeatures|Booliano|Permite que os administradores de TI bloqueiem experiências que normalmente são apenas para consumidores, como Sugestões de início, Notificações de associação, instalação de aplicativo pós-OOBE e redirecionamento de blocos.|
|windowsSpotlightBlocked|Booliano|Permite que os administradores de TI desativem todos os recursos do Destaque do Windows|
|windowsSpotlightBlockOnActionCenter|Booliano|Bloquear sugestões da Microsoft mostradas após cada instalação limpa do sistema operacional, após upgrades ou de modo contínuo para apresentar aos usuários as novidades ou alterações|
|windowsSpotlightBlockTailoredExperiences|Booliano|Bloquear conteúdo personalizado no Destaque do Windows com base no uso do dispositivo pelo usuário.|
|windowsSpotlightBlockThirdPartyNotifications|Booliano|Bloquear conteúdo de terceiros fornecido por meio do Destaque do Windows|
|windowsSpotlightBlockWelcomeExperience|Booliano|Bloquear a experiência de boas-vindas do Destaque do Windows|
|windowsSpotlightBlockWindowsTips|Booliano|Permite que os administradores de TI desativem os popups de Dicas do Windows.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Especifica o tipo de destaque. Os valores possíveis são: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Booliano|Se definida, as configurações de proxy serão aplicadas a todos os processos e contas no dispositivo. Caso contrário, serão aplicadas à conta de usuário registrada no MDM.|
|networkProxyDisableAutoDetect|Booliano|Desabilitar a detecção automática de configurações. Se habilitada, o sistema tentará encontrar o caminho para um script de configuração automática de proxy (PAC).|
|networkProxyAutomaticConfigurationUrl|String|Endereço para o script de configuração automática de proxy (PAC) desejado.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|Especifica configurações manuais de servidor proxy.|
|accountsBlockAddingNonMicrosoftAccountEmail|Booliano|Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.|
|antiTheftModeBlocked|Boolean|Indica se o usuário será ou não impedido de selecionar a preferência do modo AntiTheft (somente no Windows 10 Mobile).|
|bluetoothBlocked|Boolean|Se o usuário será ou não impedido de usar o bluetooth.|
|cameraBlocked|Booliano|Se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|connectedDevicesServiceBlocked|Booliano|Se serão bloqueados ou não o serviço de dispositivos conectados, que permite a descoberta e conexão de outros dispositivos, mensagens remotas, sessões de aplicativo remoto e outras experiências entre dispositivos.|
|certificatesBlockManualRootCertificateInstallation|Booliano|Se o usuário será ou não impedido de fazer a instalação manual do certificado raiz.|
|copyPasteBlocked|Booliano|Se o usuário será ou não impedido de usar a função copiar/colar.|
|cortanaBlocked|Booliano|Se o usuário será ou não impedido de usar a Cortana.|
|deviceManagementBlockFactoryResetOnMobile|Booliano|Se o usuário será ou não impedido de redefinir o telefone.|
|deviceManagementBlockManualUnenroll|Booliano|Indica se o usuário será ou não impedido de cancelar manualmente o registro no gerenciamento de dispositivo.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|Especifica que nível de filtro de pesquisa segura é necessário. Os valores possíveis são: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Booliano|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|edgeBlockSearchSuggestions|Booliano|Indica se o usuário será ou não impedido de usar as sugestões de pesquisa na barra de endereços.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Booliano|Indica se o tráfego de intranet deve ou não ser alternado da borda para o Internet Explorer. Observação: o nome dessa propriedade é inesperado; a propriedade é obsoleta, use EdgeSendIntranetTrafficToInternetExplorer em vez disso.|
|edgeSendIntranetTrafficToInternetExplorer|Booliano|Indica se o tráfego de intranet deve ou não ser alternado da borda para o Internet Explorer.|
|edgeRequireSmartScreen|Booliano|Indica se o usuário deverá ou não usar o Filtro SmartScreen.|
|edgeEnterpriseModeSiteListLocation|String|Indica o local da lista de sites do modo Empresarial. Pode ser um arquivo local, rede local ou local http.|
|edgeFirstRunUrl|String|A primeira URL a ser executada quando o navegador Edge é aberto pela primeira vez.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|Permite aos administradores de TI definir um mecanismo de pesquisa padrão para dispositivos controlados por MDM. Os usuários podem substituí-lo e alterar o mecanismo de pesquisa padrão fornecido, caso a política AllowSearchEngineCustomization não esteja definida.|
|edgeHomepageUrls|String collection|A lista de URLs de home pages mostradas em dispositivos registrados no MDM no navegador Edge.|
|edgeBlockAccessToAboutFlags|Booliano|Indica se será impedido ou não o acesso a sinalizadores Sobre no navegador Edge.|
|smartScreenBlockPromptOverride|Booliano|Indica se os usuários poderão ou não substituir avisos do Filtro SmartScreen sobre sites potencialmente maliciosos.|
|smartScreenBlockPromptOverrideForFiles|Booliano|Indica se os usuários poderão ou não substituir os avisos do Filtro SmartScreen sobre sites baixados não verificados.|
|webRtcBlockLocalhostIpAddress|Booliano|Indica se o endereço IP do localhost do usuário será ou não exibido durante chamadas telefônicas usando o WebRTC|
|internetSharingBlocked|Booliano|Indica se o usuário será ou não impedido de usar o compartilhamento de Internet.|
|settingsBlockAddProvisioningPackage|Booliano|Indica se o usuário será ou não impedido de instalar pacotes de provisionamento.|
|settingsBlockRemoveProvisioningPackage|Booliano|Indica se o agente de configuração de tempo de execução será ou não impedido de remover pacotes de provisionamento.|
|settingsBlockChangeSystemTime|Booliano|Indica se o usuário será ou não impedido de alterar configurações de data e hora.|
|settingsBlockEditDeviceName|Booliano|Indica se o usuário será ou não impedido de editar o nome do dispositivo.|
|settingsBlockChangeRegion|Booliano|Indica se o usuário será ou não impedido de alterar as configurações de região.|
|settingsBlockChangeLanguage|Booliano|Indica se o usuário será ou não impedido de alterar as configurações de idioma.|
|settingsBlockChangePowerSleep|Booliano|Indica se o usuário será ou não impedido de alterar as configurações de energia e suspensão.|
|locationServicesBlocked|Booliano|Indica se o usuário será ou não bloqueado dos serviços de localização.|
|microsoftAccountBlocked|Booliano|Indica se uma conta da Microsoft será ou não bloqueada.|
|microsoftAccountBlockSettingsSync|Boolean|Indica se a sincronização de configurações da conta da Microsoft será ou não bloqueada.|
|nfcBlocked|Booliano|Indica se o usuário será ou não impedido de usar a comunicação a curta distância.|
|resetProtectionModeBlocked|Booliano|Indica se o usuário será ou não bloqueado do modo de proteção contra restauração de fábrica.|
|screenCaptureBlocked|Booliano|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|storageBlockRemovableStorage|Booliano|Indica se o usuário será ou não impedido de usar o armazenamento removível.|
|storageRequireMobileDeviceEncryption|Booliano|Indica se a criptografia é ou não necessária em um dispositivo móvel.|
|usbBlocked|Booliano|Indica se o usuário será ou não bloqueado da conexão USB.|
|voiceRecordingBlocked|Booliano|Indica se o usuário será ou não bloqueado da gravação de voz.|
|wiFiBlockAutomaticConnectHotspots|Booliano|Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada. Não terá impacto se o Wi-Fi estiver bloqueado.|
|wiFiBlocked|Booliano|Indica se o usuário será ou não impedido de usar o Wi-Fi.|
|wiFiBlockManualConfiguration|Booliano|Indica se o usuário será ou não impedido de usar a configuração manual do Wi-Fi.|
|wiFiScanInterval|Int32|Especificar com que frequência os dispositivos procuram redes Wi-Fi. Os valores compatíveis ficam entre 1 e 500, em que 100 = padrão e 500 = frequência baixa. Valores válidos de 1 a 500|
|wirelessDisplayBlockProjectionToThisDevice|Booliano|Indica se outros dispositivos poderão ou não descobrir este PC para fins de projeção.|
|wirelessDisplayBlockUserInputFromReceiver|Booliano|Indica se a entrada do usuário pelo receptor de vídeo sem fio será permitida ou não.|
|wirelessDisplayRequirePinForPairing|Booliano|Indica se será exigido um PIN para que novos dispositivo iniciem o emparelhamento.|
|windowsStoreBlocked|Booliano|Indica se o usuário será ou não impedido de usar a Windows Store.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indica se aplicativos de pacotes AppX assinados com um certificado confiável podem ser transferidos por sideload. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Booliano|Indica se a atualização automática de aplicativos pela Windows Store será bloqueada ou não.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indica se o desbloqueio do desenvolver será permitido ou não. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Booliano|Indica se vários usuários do mesmo aplicativo serão ou não impedidos de compartilhar dados.|
|appsBlockWindowsStoreOriginatedApps|Booliano|Indica se será desabilitada ou não a inicialização de todos os aplicativos da Windows Store pré-instalados ou baixados.|
|windowsStoreEnablePrivateStoreOnly|Booliano|Indica se o Repositório particular será ativado ou não.|
|storageRestrictAppDataToSystemVolume|Booliano|Indica se os dados do aplicativo ficarão restritos à unidade do sistema.|
|storageRestrictAppInstallToSystemVolume|Booliano|Indica se a instalação de aplicativos ficará restrita à unidade do sistema.|
|gameDvrBlocked|Booliano|Indica se DVR e difusão serão bloqueados ou não.|
|experienceBlockDeviceDiscovery|Booliano|Indica se a experiência de descoberta de dispositivos será ativada ou não.|
|experienceBlockErrorDialogWhenNoSIM|Booliano|Indica se a caixa de diálogo de erro poderá ou não ser exibida se nenhum cartão SIM for detectado.|
|experienceBlockTaskSwitcher|Booliano|Indica se a alternância de tarefas será ativada ou não no dispositivo.|
|logonBlockFastUserSwitching|Boolean|Desabilita a capacidade para alternar rapidamente entre os usuários conectados simultaneamente sem fazer logoff.|
|Propriedadetenantlockdownrequirenetworkduringoutofboxexperience|Booliano|Se o dispositivo é necessário para se conectar à rede.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9822

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "edgeSendIntranetTrafficToInternetExplorer": true,
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
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9994

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
  "edgeSendIntranetTrafficToInternetExplorer": true,
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
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true
}
```



