---
title: Tipo de recurso windows10GeneralConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows10GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 841a61f636e56e05b0d3b38d6172fa55888595fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369849"
---
# <a name="windows10generalconfiguration-resource-type"></a>Tipo de recurso windows10GeneralConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows10GeneralConfiguration.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10GeneralConfigurations](../api/intune-deviceconfig-windows10generalconfiguration-list.md)|Coleção [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Listar propriedades e relações dos objetos [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Obter windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-get.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Ler propriedades e relações do objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Criar windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-create.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Cria um novo objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Excluir windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-delete.md)|Nenhum|Excluir um [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|
|[Atualizar windows10GeneralConfiguration](../api/intune-deviceconfig-windows10generalconfiguration-update.md)|[windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md)|Atualizar as propriedades de um objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para essa política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para essa política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|taskManagerBlockEndTask|Booliano|Especifique se os usuários que não são administradores podem usar o Gerenciador de tarefas para finalizar tarefas.|
|energySaverOnBatteryThresholdPercentage|Int32|Essa configuração permite especificar o nível de carga da bateria no qual a economia de energia está ativada. Durante a bateria, a economia de energia é ativada automaticamente em (e abaixo) do nível de carga da bateria especificado. Intervalo de entrada válido (0-100). Valores válidos de 0 a 100|
|energySaverPluggedInThresholdPercentage|Int32|Essa configuração permite especificar o nível de carga da bateria no qual a economia de energia está ativada. Enquanto conectado, o economia de energia é automaticamente ativado em (e abaixo) do nível de carga da bateria especificado. Intervalo de entrada válido (0-100). Valores válidos de 0 a 100|
|powerLidCloseActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que o Windows executará quando um usuário fechar a tampa de um computador móvel enquanto estiver na bateria. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerLidCloseActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que o Windows executará quando um usuário fechar a tampa de um computador móvel enquanto estiver conectado. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que o Windows executa quando um usuário pressiona o botão de energia enquanto estiver na bateria. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que o Windows executa quando um usuário pressiona o botão de energia enquanto estiver conectado. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que o Windows executa quando um usuário pressiona o botão dormir enquanto estiver na bateria. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que o Windows executa quando um usuário pressiona o botão dormir enquanto estiver conectado. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerHybridSleepOnBattery|[habilitação](../resources/intune-shared-enablement.md)|Essa configuração permite que você desative a suspensão híbrida enquanto estiver na bateria. Se você definir essa configuração como disable, um Hiberfile não será gerado quando o sistema passar para Sleep (em espera). Se você definir essa configuração para habilitar ou não definir essa configuração de política, os usuários controlarão essa configuração. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|powerHybridSleepPluggedIn|[habilitação](../resources/intune-shared-enablement.md)|Essa configuração permite que você desative a suspensão híbrida enquanto estiver conectado. Se você definir essa configuração como disable, um Hiberfile não será gerado quando o sistema passar para Sleep (em espera). Se você definir essa configuração para habilitar ou não definir essa configuração de política, os usuários controlarão essa configuração. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Agendamento de atualização forçada do Windows 10 para aplicativos.|
|enableAutomaticRedeployment|Booliano|Permitir que usuários com direitos administrativos excluam todos os dados e configurações de usuário usando CTRL + Win + R na tela de bloqueio de dispositivo para que o dispositivo possa ser automaticamente reconfigurado e inscrito novamente no gerenciamento.|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune-deviceconfig-signinassistantoptions.md)|Controla o serviço do assistente de conexão de conta da Microsoft (WLIDSVC) NT. Os valores possíveis são: `notConfigured` e `disabled`.|
|authenticationAllowSecondaryDevice|Booliano|Permite que dispositivos de autenticação secundário funcionem com o Windows.|
|authenticationWebSignIn|[habilitação](../resources/intune-shared-enablement.md)|Indica se o provedor de credenciais da Web será habilitado ou não. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|authenticationPreferredAzureADTenantDomainName|String|Especifica o domínio preferencial entre os domínios disponíveis no locatário do Azure AD.|
|cryptographyAllowFipsAlgorithmPolicy|Booliano|Especifique se deseja permitir ou não a política padrão do FIPS (Federal Information Processing Standard).|
|displayAppListWithGdiDPIScalingTurnedOn|Coleção de cadeias de caracteres|Lista de aplicativos herdados com ajuste de DPI GDI ativado.|
|displayAppListWithGdiDPIScalingTurnedOff|Coleção de cadeias de caracteres|Lista de aplicativos herdados com a expansão de DPI GDI desativada.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Ponto de extremidade para descoberta de impressoras na nuvem.|
|enterpriseCloudPrintOAuthAuthority|String|Ponto de extremidade para aquisição de tokens OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID de um aplicativo cliente autorizado a recuperar tokens OAuth da autoridade OAuth.|
|enterpriseCloudPrintResourceIdentifier|String|URI do recurso OAuth para serviço de impressão, conforme configurado no portal do Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Número máximo de impressoras que devem ser consultadas em um ponto de extremidade de descoberta. Esta é uma configuração somente para dispositivos móveis. Valores válidos de 1 a 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|URI do recurso OAuth para serviço de descoberta de impressoras, conforme configurado no portal do Azure.|
|experienceDoNotSyncBrowserSettings|[browserSyncSetting](../resources/intune-deviceconfig-browsersyncsetting.md)|Permitir ou impedir a sincronização das configurações do navegador Microsoft Edge. Opção para os administradores de ti impedir a sincronização entre dispositivos, mas permitir a substituição do usuário. Os valores possíveis são: `notConfigured`, `blockedWithUserOverride`, `blocked`.|
|messagingBlockSync|Booliano|Indica se o backup e a restauração de mensagens de texto devem ou não ser bloqueados e mensagens em qualquer lugar.|
|messagingBlockMMS|Booliano|Indica se a funcionalidade de envio/recebimento de MMS deve ou não ser bloqueada no dispositivo.|
|messagingBlockRichCommunicationServices|Booliano|Indica se a funcionalidade de envio/recebimento de RCS deve ou não ser bloqueada no dispositivo.|
|printerNames|Coleção de cadeias de caracteres|Provisiona automaticamente impressoras com base em seus nomes (nomes de host de rede).|
|printerDefaultName|String|Nome (nome do host de rede) de uma impressora instalada.|
|printerBlockAddition|Booliano|Impedir a instalação do usuário de impressoras adicionais das configurações de impressoras.|
|searchBlockDiacritics|Booliano|Especifica se a pesquisa pode usar diacríticos.|
|searchDisableAutoLanguageDetection|Booliano|Especifica se a detecção automática de idioma será usada ao indexar conteúdo e propriedades.|
|searchDisableIndexingEncryptedItems|Booliano|Indica se a indexação de itens protegidos por WIP será bloqueada ou não para que eles não apareçam nos resultados de pesquisa da Cortana ou do Explorer.|
|searchEnableRemoteQueries|Boolean|Indica se as consultas remotas do índice deste computador serão bloqueadas ou não.|
|searchDisableUseLocation|Booliano|Especifica se a pesquisa pode usar informações de local.|
|searchDisableLocation|Booliano|Especifica se a pesquisa pode usar informações de local.|
|searchDisableIndexerBackoff|Booliano|Indica se o recurso de retirada de indexador de pesquisa deve ou não ser desativado.|
|searchDisableIndexingRemovableDrive|Booliano|Indica se os usuários poderão ou não adicionar locais de unidades removíveis a bibliotecas e para serem indexados.|
|searchEnableAutomaticIndexSizeManangement|Booliano|Especifica uma quantidade mínima de espaço em disco rígido na mesma unidade como o local do índice antes que a indexação seja interrompida.|
|searchBlockWebResults|Booliano|Indica se a pesquisa da Web deve ou não ser bloqueada.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Booliano|Especifique se deseja permitir a criptografia automática do dispositivo durante o OOBE quando o dispositivo é associado ao AD do Azure (somente desktop).|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Obtém ou define um valor que permite que o dispositivo envie dados de diagnóstico e de telemetria de uso, como Watson. Os valores possíveis são: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Booliano|Obtém ou define um valor para permitir que os administradores de TI impeçam aplicativos e recursos de trabalhar com arquivos no OneDrive.|
|systemTelemetryProxyServer|String|Obtém ou define o nome de domínio totalmente qualificado (FQDN) ou o endereço IP de um servidor proxy para encaminhar as experiências de usuário conectado e solicitações de telemetria.|
|edgeTelemetryForMicrosoft365Analytics|[edgeTelemetryMode](../resources/intune-deviceconfig-edgetelemetrymode.md)|Especifica o tipo de dados de telemetria (nenhum, intranet, Internet, ambos) é enviado para a análise do Microsoft 365. Os valores possíveis são: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune-deviceconfig-inkaccesssetting.md)|Controla o acesso do usuário ao espaço de trabalho de tinta, da área de trabalho e de cima da tela de bloqueio. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|inkWorkspaceAccessState|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Controla o acesso do usuário ao espaço de trabalho de tinta, da área de trabalho e de cima da tela de bloqueio. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|inkWorkspaceBlockSuggestedApps|Booliano|Especifique se deseja mostrar sugestões de aplicativos recomendadas no espaço de trabalho de tinta.|
|smartScreenEnableAppInstallControl|Booliano|Essa propriedade será preterida em julho de 2019 e será substituída pela propriedade SmartScreenAppInstallControl. Permite que os administradores de TI controlem se os usuários poderão instalar aplicativos de lugares que não sejam a Store.|
|smartScreenAppInstallControl|[appInstallControlType](../resources/intune-deviceconfig-appinstallcontroltype.md)|Adicionado no Windows 10, versão 1703. Permite que os administradores de TI controlem se os usuários poderão instalar aplicativos de lugares que não sejam a Store. Os valores possíveis são: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.|
|personalizationDesktopImageUrl|String|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da área de trabalho ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da área de trabalho.|
|personalizationLockScreenImageUrl|String|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da tela de bloqueio ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da tela de bloqueio.|
|bluetoothAllowedServices|String collection|Especifica uma lista de serviços e perfis Bluetooth permitidos em cadeias de caracteres de formato hexadecimal.|
|bluetoothBlockAdvertising|Booliano|Se o usuário será ou não impedido de usar a publicidade do bluetooth.|
|bluetoothBlockPromptedProximalConnections|Booliano|Se os usuários devem ou não ser impedidos de usar o par Swift e outros cenários baseados em proximidade.|
|bluetoothBlockDiscoverableMode|Booliano|Se o usuário será ou não impedido de usar o modo de descoberta de bluetooth.|
|bluetoothBlockPrePairing|Booliano|Se determinados periféricos Bluetooth agrupados serão bloqueados ou não do emparelhamento automático com o dispositivo host.|
|edgeBlockAutofill|Booliano|Indica se o preenchimento automático deve ou não ser bloqueado.|
|edgeBlocked|Booliano|Indica se o usuário será ou não impedido de usar o navegador Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Indica quais cookies bloquear no navegador Edge. Os valores possíveis são: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Booliano|Indica se as ferramentas de desenvolvedor serão bloqueadas ou não no navegador Edge.|
|edgeBlockSendingDoNotTrackHeader|Booliano|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|edgeBlockExtensions|Booliano|Indica se as extensões serão bloqueadas ou não no navegador Edge.|
|edgeBlockInPrivateBrowsing|Booliano|Indica se a navegação InPrivate será bloqueada ou não em redes corporativas no navegador Edge.|
|edgeBlockJavaScript|Booliano|Indica se o usuário será ou não impedido de usar JavaScript.|
|edgeBlockPasswordManager|Boolean|Indica se o gerenciador de senhas será bloqueado ou não.|
|edgeBlockAddressBarDropdown|Booliano|Bloquear a funcionalidade de menu suspenso da barra de endereços no Microsoft Edge. Desabilite essa configuração para minimizar as conexões de rede do Microsoft Edge com serviços Microsoft.|
|edgeBlockCompatibilityList|Booliano|Bloquear lista de compatibilidade da Microsoft no Microsoft Edge. Essa lista da Microsoft ajuda o Edge a exibir corretamente sites com problemas de compatibilidade conhecidos.|
|edgeClearBrowsingDataOnExit|Booliano|Limpar dados de navegação ao sair do Microsoft Edge.|
|edgeAllowStartPagesModification|Booliano|Permitir que os usuários alterem as páginas iniciais no Edge. Use EdgeHomepageUrls para especificar as páginas iniciais que o usuário verá por padrão ao abrir o Edge.|
|edgeDisableFirstRunPage|Booliano|Bloquear a página da Web da Microsoft que é aberta na primeira utilização do Microsoft Edge. Esta política permite que empresas, como aquelas registradas em configurações de emissões zero, bloqueiem esta página.|
|edgeBlockLiveTileDataCollection|Booliano|Bloquear a coleta de informações da Microsoft para criação de bloco dinâmico quando os usuários fixarem um site para iniciar no Microsoft Edge.|
|edgeSyncFavoritesWithInternetExplorer|Booliano|Habilitar a sincronização de favoritos entre o Internet Explorer e o Microsoft Edge. Adições, exclusões, modificações e outras alterações para favoritos são compartilhadas entre navegadores.|
|edgeFavoritesListLocation|String|O local da lista de favoritos a ser provisionada. Pode ser um arquivo local, rede local ou local http.|
|edgeBlockEditFavorites|Booliano|Indica se o usuário será ou não impedido de fazer alterações em favoritos.|
|edgeNewTabPageURL|String|Especifique a página aberta quando novas guias são criadas.|
|edgeHomeButtonConfiguration|[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|Faz com que o botão página inicial oculte, carregue a página inicial padrão, carregue uma nova página de guia ou uma URL personalizada|
|edgeHomeButtonConfigurationEnabled|Booliano|Habilitar a configuração do botão página inicial.|
|edgeOpensWith|[edgeOpenOptions](../resources/intune-deviceconfig-edgeopenoptions.md)|Especifique o tipo de páginas que será aberto no início. Os valores possíveis são: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|edgeBlockSideloadingExtensions|Booliano|Indica se o usuário pode Sideload as extensões.|
|edgeRequiredExtensionPackageFamilyNames|Coleção de cadeias de caracteres|Especifique a lista de nomes de famílias de pacotes de extensões de navegador que são necessários e que não podem ser desativados pelo usuário.|
|edgeBlockPrinting|Booliano|Configure o Edge para permitir ou bloquear a impressão.|
|edgeFavoritesBarVisibility|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Obtém ou define um valor que especifica se a barra de favoritos deve ser configurada para sempre estar visível ou oculta em qualquer página. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|edgeBlockSavingHistory|Booliano|Configure o Edge para permitir que o histórico de navegação seja salvo ou nunca salve o histórico de navegação.|
|edgeBlockFullScreenMode|Booliano|Permitir ou impedir que a borda entre no modo de tela inteira.|
|edgeBlockWebContentOnNewTabPage|Booliano|Configure o para carregar uma página em branco na borda em vez da página padrão nova guia e impedir que os usuários as alterem.|
|edgeBlockTabPreloading|Booliano|Configure se a borda precarregará a página de nova guia na inicialização do Windows.|
|edgeBlockPrelaunch|Booliano|Decida se o Microsoft Edge está inicializado na inicialização do Windows.|
|edgeShowMessageWhenOpeningInternetExplorerSites|[internetExplorerMessageSetting](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|Controla a mensagem exibida por borda antes de mudar para o Internet Explorer. Os valores possíveis são: `notConfigured`, `disabled`, `enabled`, `keepGoing`.|
|edgePreventCertificateErrorOverride|Booliano|Permitir ou impedir que os usuários substituam erros de certificado.|
|edgeKioskModeRestriction|[edgeKioskModeRestrictionType](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|Controla como as configurações do Microsoft Edge são restringidas com base no modo de configuração de quiosque. Os valores possíveis são: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Especifica o tempo, em minutos, da última atividade do usuário antes que o Microsoft Edge quiosque seja redefinido.  Os valores válidos são 0-1440. O padrão é 5. 0 indica nenhuma redefinição. Valores válidos de 0 a 1440|
|cellularBlockDataWhenRoaming|Booliano|Se o usuário será ou não impedido de usar dados da rede celular durante roaming.|
|cellularBlockVpn|Booliano|Se o usuário será ou não impedido de usar VPN na rede celular.|
|cellularBlockVpnWhenRoaming|Boolean|Se o usuário será ou não impedido de usar VPN durante roaming na rede celular.|
|cellularData|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Se o canal de dados da rede celular será ou não permitido. Se não configurada, o canal de dados da rede celular é permitido e o usuário pode desativá-lo. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|defenderBlockEndUserAccess|Booliano|Se o usuário final será ou não impedido de acessar o Defender.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Número de dias antes da exclusão do malware em quarentena. Valores válidos de 0 a 90|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Obtém ou define ações do Defender a serem realizadas em um malware detectado por nível de ameaça.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Dia da semana em que o Defender fará a verificação do sistema. Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderFilesAndFoldersToExclude|Coleção de cadeias de caracteres|Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.|
|defenderFileExtensionsToExclude|Coleção de cadeias de caracteres|Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.|
|defenderScanMaxCpu|Int32|Porcentagem máxima de uso da CPU durante a verificação. Valores válidos de 0 a 100|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Valor de monitoramento da atividade do arquivo. Os valores possíveis são: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Obtém ou define a ação do defender a ser executada em aplicativos potencialmente indesejados (PUA), que inclui software com comportamentos de injeção de anúncio, empacotamento de software, solicitação persistente para pagamento ou assinatura, etc. O defender alerta o usuário quando o PUA está sendo baixado ou tenta se instalar. Adicionado no Windows 10 para área de trabalho. Os valores possíveis são: `deviceDefault`, `block`, `audit`.|
|defenderPotentiallyUnwantedAppActionSetting|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Obtém ou define a ação do defender a ser executada em aplicativos potencialmente indesejados (PUA), que inclui software com comportamentos de injeção de anúncio, empacotamento de software, solicitação persistente para pagamento ou assinatura, etc. O defender alerta o usuário quando o PUA está sendo baixado ou tenta se instalar. Adicionado no Windows 10 para área de trabalho. Os valores possíveis são: `userDefined`, `enable`, `auditMode`.|
|defenderProcessesToExclude|String collection|Processos a serem excluídos das verificações e da proteção em tempo real.|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|A configuração do modo como avisar um usuário do envio de exemplo. Os valores possíveis são: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Booliano|Indica se o monitoramento de comportamento deve ou não ser exigido.|
|defenderRequireCloudProtection|Booliano|Indica se a proteção na nuvem deve ou não ser exigida.|
|defenderRequireNetworkInspectionSystem|Booliano|Indica se o sistema de inspeção de rede deve ou não ser exigido.|
|defenderRequireRealTimeMonitoring|Booliano|Indica se o monitoramento em tempo real deve ou não ser exigido.|
|defenderScanArchiveFiles|Booliano|Indica se os arquivos mortos devem ou não ser verificados.|
|defenderScanDownloads|Booliano|Indica se os downloads devem ou não ser verificados.|
|defenderScheduleScanEnableLowCpuPriority|Booliano|Quando habilitada, a baixa prioridade da CPU será usada durante as verificações agendadas.|
|defenderDisableCatchupQuickScan|Booliano|Quando bloqueado, as verificações de atualização de verificações rápidas agendadas serão desativadas.|
|defenderDisableCatchupFullScan|Booliano|Quando bloqueado, as verificações de atualização para verificações completas agendadas serão desativadas.|
|defenderScanNetworkFiles|Booliano|Indica se os arquivos abertos de uma pasta da rede devem ou não ser verificados.|
|defenderScanIncomingMail|Booliano|Indica se as mensagens de email de entrada devem ou não ser verificadas.|
|defenderScanMappedNetworkDrivesDuringFullScan|Booliano|Indica se as unidades de rede mapeadas devem ou não ser verificadas durante a verificação completa.|
|defenderScanRemovableDrivesDuringFullScan|Booliano|Indica se as unidades removíveis devem ou não ser verificadas durante a verificação completa.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Indica se os scripts carregados no navegador Internet Explorer devem ou não ser verificados.|
|defenderSignatureUpdateIntervalInHours|Int32|O intervalo de atualização da assinatura em horas. Especifique 0 para não verificar. Valores válidos de 0 a 24|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|O tipo de verificação do sistema do Defender. Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledScanTime|TimeOfDay|A hora em que o Defender fará a verificação do sistema.|
|defenderScheduledQuickScanTime|TimeOfDay|O horário de realização da verificação diária rápida.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Especifica o nível de proteção oferecido na nuvem. Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Extensão de tempo limite para verificação de arquivo pela nuvem. Valores válidos de 0 a 50|
|defenderCloudExtendedTimeoutInSeconds|Int32|Extensão de tempo limite para verificação de arquivo pela nuvem. Valores válidos de 0 a 50|
|defenderBlockOnAccessProtection|Booliano|Permite ou proíbe a funcionalidade de proteção de acesso do Windows Defender.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|Verifica se o nível de consentimento do usuário no Windows Defender deve enviar dados. Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|lockScreenAllowTimeoutConfiguration|Booliano|Especifique se deseja mostrar uma definição configurável pelo usuário para controlar o tempo limite da tela enquanto estiver na tela de bloqueio de dispositivos Windows Mobile 10. Se essa política estiver definida como Permitir, o valor definido por lockScreenTimeoutInSeconds será ignorado.|
|lockScreenBlockActionCenterNotifications|Booliano|Indica se as notificações da central de ações na tela de bloqueio serão bloqueadas.|
|lockScreenBlockCortana|Booliano|Indica se o usuário pode ou não interagir com a Cortana usando a fala enquanto o sistema estiver bloqueado.|
|lockScreenBlockToastNotifications|Booliano|Indica se serão permitidas notificações do sistema acima da tela de bloqueio do dispositivo.|
|lockScreenTimeoutInSeconds|Int32|Defina a duração (em segundos) da tela de bloqueio para a tela em desligamento para dispositivos Windows Mobile 10. Os valores compatíveis ficam entre 11 e 1800. Valores válidos de 11 a 1800|
|lockScreenActivateAppsWithVoice|[habilitação](../resources/intune-shared-enablement.md)|Essa configuração de política especifica se os aplicativos do Windows podem ser ativados pela voz enquanto o sistema está bloqueado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|passwordBlockSimple|Booliano|Especifique se PINs ou senhas como "1111" ou "1234" são permitidas. Para computadores do Windows 10, isso também controla o uso de senhas com imagem.|
|passwordExpirationDays|Int32|A expiração da senha em dias. Valores válidos de 0 a 730|
|passwordMinimumLength|Int32|O comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 50|
|passwordRequired|Booliano|Indica se um usuário deverá ou não ter uma senha.|
|passwordRequireWhenResumeFromIdleState|Booliano|Indica se uma senha deve ou não ser exigida ao sair de um estado inativo.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica. Valores válidos de 0 a 999|
|passwordMinimumAgeInDays|Int32|Essa configuração de segurança determina o período de tempo (em dias) que uma senha deve ser usada para que o usuário possa alterá-la. Valores válidos de 0 a 998|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Habilita ou desabilita o uso da ID de publicidade. Adicionado no Windows 10, versão 1607. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Indica se será permitida ou não a aceitação automática da caixa de diálogo de consentimento do usuário com emparelhamento e privacidade ao iniciar aplicativos.|
|privacyDisableLaunchExperience|Booliano|Essa política impede que a experiência de privacidade seja iniciada durante o logon do usuário para usuários novos e atualizados.|
|privacyBlockInputPersonalization|Booliano|Indica se o uso dos serviços de fala baseados na nuvem será bloqueado para os aplicativos Cortana, Ditado ou Store.|
|privacyBlockPublishUserActivities|Booliano|Bloqueia as experiências/descoberta compartilhadas de recursos usados recentemente no alternador de tarefas, etc.|
|privacyBlockActivityFeed|Booliano|Bloqueia o uso de serviços de fala baseados em nuvem para Cortana, ditar ou armazenar aplicativos.|
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
|antiTheftModeBlocked|Booliano|Indica se o usuário será ou não impedido de selecionar a preferência do modo AntiTheft (somente no Windows 10 Mobile).|
|bluetoothBlocked|Booliano|Se o usuário será ou não impedido de usar o bluetooth.|
|cameraBlocked|Booliano|Se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|connectedDevicesServiceBlocked|Boolean|Se serão bloqueados ou não o serviço de dispositivos conectados, que permite a descoberta e conexão de outros dispositivos, mensagens remotas, sessões de aplicativo remoto e outras experiências entre dispositivos.|
|certificatesBlockManualRootCertificateInstallation|Booliano|Se o usuário será ou não impedido de fazer a instalação manual do certificado raiz.|
|copyPasteBlocked|Booliano|Se o usuário será ou não impedido de usar a função copiar/colar.|
|cortanaBlocked|Booliano|Se o usuário será ou não impedido de usar a Cortana.|
|deviceManagementBlockFactoryResetOnMobile|Booliano|Se o usuário será ou não impedido de redefinir o telefone.|
|deviceManagementBlockManualUnenroll|Booliano|Indica se o usuário será ou não impedido de cancelar manualmente o registro no gerenciamento de dispositivo.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|Especifica que nível de filtro de pesquisa segura é necessário. Os valores possíveis são: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Booliano|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|edgeBlockSearchSuggestions|Booliano|Indica se o usuário será ou não impedido de usar as sugestões de pesquisa na barra de endereços.|
|edgeBlockSearchEngineCustomization|Booliano|Indica se o usuário será ou não impedido de adicionar novo mecanismo de pesquisa ou de alterar o mecanismo de pesquisa padrão.|
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
|nfcBlocked|Boolean|Indica se o usuário será ou não impedido de usar a comunicação a curta distância.|
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
|appManagementMSIAllowUserControlOverInstall|Booliano|Essa configuração de política permite que os usuários alterem as opções de instalação que normalmente estão disponíveis somente para administradores do sistema.|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|Booliano|Essa configuração de política instrui o Windows Installer a usar permissões elevadas ao instalar qualquer programa no sistema.|
|dataProtectionBlockDirectMemoryAccess|Booliano|Essa configuração de política permite bloquear o acesso direto à memória (DMA) para todas as portas de downstream PCI que podem ser conectadas a quente até que um usuário faça logon no Windows.|
|appManagementPackageFamilyNamesToLaunchAfterLogOn|Coleção de cadeias de caracteres|Lista de nomes de família de pacotes delimitados por ponto e vírgula de aplicativos do Windows. Os aplicativos do Windows listados devem ser iniciados após o logon.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|privacyAccessControls|coleção [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Indica uma lista de aplicativos com níveis de controle de acesso sobre categorias de dados de privacidade e/ou os níveis de acesso padrão por categoria.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "taskManagerBlockEndTask": true,
  "energySaverOnBatteryThresholdPercentage": 1024,
  "energySaverPluggedInThresholdPercentage": 1024,
  "powerLidCloseActionOnBattery": "String",
  "powerLidCloseActionPluggedIn": "String",
  "powerButtonActionOnBattery": "String",
  "powerButtonActionPluggedIn": "String",
  "powerSleepButtonActionOnBattery": "String",
  "powerSleepButtonActionPluggedIn": "String",
  "powerHybridSleepOnBattery": "String",
  "powerHybridSleepPluggedIn": "String",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "String (timestamp)",
    "recurrence": "String",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "String",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "String",
  "authenticationPreferredAzureADTenantDomainName": "String",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "String"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "String"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": 1024,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "experienceDoNotSyncBrowserSettings": "String",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "String"
  ],
  "printerDefaultName": "String",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "String",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "String",
  "edgeTelemetryForMicrosoft365Analytics": "String",
  "inkWorkspaceAccess": "String",
  "inkWorkspaceAccessState": "String",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "String",
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "String",
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
  "edgeFavoritesListLocation": "String",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "String",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "String",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "String"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "String",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "String",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "String",
  "edgeKioskResetAfterIdleTimeInMinutes": 1024,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "String",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  },
  "defenderSystemScanSchedule": "String",
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderScanMaxCpu": 1024,
  "defenderMonitorFileActivity": "String",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderPotentiallyUnwantedAppActionSetting": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderScanType": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": 1024,
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "String",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 1024,
  "lockScreenActivateAppsWithVoice": "String",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordMinimumAgeInDays": 1024,
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "String",
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
  "startMenuLayoutEdgeAssetsXml": "binary",
  "startMenuLayoutXml": "binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
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
  "windowsSpotlightConfigureOnLockScreen": "String",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "String",
    "exceptions": [
      "String"
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
  "safeSearchFilter": "String",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "String"
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
  "wiFiScanInterval": 1024,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "String",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "String",
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
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "String"
  ]
}
```



