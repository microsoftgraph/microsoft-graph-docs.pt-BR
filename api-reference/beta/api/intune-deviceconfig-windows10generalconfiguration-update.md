---
title: Atualizar windows10GeneralConfiguration
description: Atualizar as propriedades de um objeto windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4511017aa539a2405b59b622858878e60e6ff9a3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788342"
---
# <a name="update-windows10generalconfiguration"></a>Atualizar windows10GeneralConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

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
No corpo da solicitação, forneça uma representação JSON do objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|taskManagerBlockEndTask|Boleano|Especifique se os não administradores podem usar o Gerenciador de Tarefas para finalizar tarefas.|
|energySaverOnBatteryThresholdPercentage|Int32|Essa configuração permite especificar o nível de carga da bateria no qual o Economia de Energia está ligado. Durante a bateria, o Economia de Energia é ativado automaticamente em (e abaixo) do nível de carga da bateria especificado. Intervalo de entrada válido (0-100). Valores válidos de 0 a 100|
|energySaverPluggedInThresholdPercentage|Int32|Essa configuração permite especificar o nível de carga da bateria no qual o Economia de Energia está ligado. Quando conectado, o Economia de Energia é ativado automaticamente em (e abaixo) do nível de carga da bateria especificado. Intervalo de entrada válido (0-100). Valores válidos de 0 a 100|
|powerLidCloseActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação Windows tomada quando um usuário fecha a tampa de um computador móvel durante a bateria. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerLidCloseActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação Windows tomada quando um usuário fecha a tampa de um computador móvel enquanto está conectado. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação Windows tomada quando um usuário pressiona o botão Ligar durante a bateria. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação Windows tomada quando um usuário pressiona o botão Ligar enquanto estiver conectado. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionOnBattery|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação que Windows tomada quando um usuário pressiona o botão Sleep durante a bateria. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionPluggedIn|[powerActionType](../resources/intune-deviceconfig-poweractiontype.md)|Essa configuração especifica a ação Windows tomada quando um usuário pressiona o botão Sleep enquanto está conectado. Os valores possíveis são: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerHybridSleepOnBattery|[enablement](../resources/intune-shared-enablement.md)|Essa configuração permite desativar o sono híbrido durante a bateria. Se você definir essa configuração como desabilitada, um hiberfile não será gerado quando o sistema faz a transição para o sleep (Stand By). Se você definir essa configuração para habilitar ou não configurar essa configuração de política, os usuários controlarão essa configuração. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|powerHybridSleepPluggedIn|[enablement](../resources/intune-shared-enablement.md)|Essa configuração permite desativar o sono híbrido enquanto estiver conectado. Se você definir essa configuração como desabilitada, um hiberfile não será gerado quando o sistema faz a transição para o sleep (Stand By). Se você definir essa configuração para habilitar ou não configurar essa configuração de política, os usuários controlarão essa configuração. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|Windows 10 forçar o agendamento de atualização para Aplicativos.|
|enableAutomaticRedeployment|Boleano|Permitir que os usuários com direitos administrativos excluam todos os dados e configurações do usuário usando CTRL + Win + R na tela de bloqueio do dispositivo para que o dispositivo possa ser automaticamente reconfigurado e re-inscrito no gerenciamento.|
|microsoftAccountSignInAssistantSettings|[signInAssistantOptions](../resources/intune-deviceconfig-signinassistantoptions.md)|Controla o serviço NT Sign-In assistente de conta da Microsoft (wlidsvc). Os valores possíveis são: `notConfigured` e `disabled`.|
|authenticationAllowSecondaryDevice|Boleano|Permite que dispositivos de autenticação secundários funcionem com Windows.|
|authenticationWebSignIn|[enablement](../resources/intune-shared-enablement.md)|Indica se o Provedor de Credenciais da Web será habilitado ou não. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|authenticationPreferredAzureADTenantDomainName|Cadeia de caracteres|Especifica o domínio preferencial entre os domínios disponíveis no locatário do Azure AD.|
|cryptographyAllowFipsAlgorithmPolicy|Boleano|Especifique se é permitido ou não a política FIPS (Federal Information Processing Standard).|
|displayAppListWithGdiDPIScalingTurnedOn|Coleção de cadeias de caracteres|Lista de aplicativos herdado que têm o Dimensionamento de DPI GDI ligado.|
|displayAppListWithGdiDPIScalingTurnedOff|Coleção de cadeias de caracteres|Lista de aplicativos herdado que têm o Dimensionamento de DPI GDI desligado.|
|enterpriseCloudPrintDiscoveryEndPoint|String|Ponto de extremidade para descoberta de impressoras na nuvem.|
|enterpriseCloudPrintOAuthAuthority|String|Ponto de extremidade para aquisição de tokens OAuth.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID de um aplicativo cliente autorizado a recuperar tokens OAuth da autoridade OAuth.|
|enterpriseCloudPrintResourceIdentifier|String|URI do recurso OAuth para serviço de impressão, conforme configurado no portal do Azure.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Número máximo de impressoras que devem ser consultadas em um ponto de extremidade de descoberta. Esta é uma configuração somente para dispositivos móveis. Valores válidos de 1 a 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|URI do recurso OAuth para serviço de descoberta de impressoras, conforme configurado no portal do Azure.|
|experienceDoNotSyncBrowserSettings|[browserSyncSetting](../resources/intune-deviceconfig-browsersyncsetting.md)|Permitir ou impedir a sincronização de configurações Microsoft Edge Navegador. Opção para os administradores de IT impedirem a sincronização entre dispositivos, mas permitir a substituição do usuário. Os valores possíveis são: `notConfigured`, `blockedWithUserOverride`, `blocked`.|
|messagingBlockSync|Boleano|Indica se a mensagem de texto deve ou não ser restaurada e restaurada em todos os lugares.|
|messagingBlockMMS|Boleano|Indica se a funcionalidade de envio/recebimento MMS deve ou não ser bloqueado no dispositivo.|
|messagingBlockRichCommunicationServices|Boleano|Indica se a funcionalidade RCS enviar/receber no dispositivo.|
|printerNames|Coleção de cadeias de caracteres|Provisionar impressoras automaticamente com base em seus nomes (nomes de host de rede).|
|printerDefaultName|Cadeia de caracteres|Nome (nome do host de rede) de uma impressora instalada.|
|printerBlockAddition|Boleano|Impedir a instalação do usuário de impressoras adicionais de configurações de impressoras.|
|searchBlockDiacritics|Boolean|Especifica se a pesquisa pode usar diacríticos.|
|searchDisableAutoLanguageDetection|Boolean|Especifica se a detecção automática de idioma será usada ao indexar conteúdo e propriedades.|
|searchDisableIndexingEncryptedItems|Boolean|Indica se a indexação de itens protegidos por WIP será bloqueada ou não para que eles não apareçam nos resultados de pesquisa da Cortana ou do Explorer.|
|searchEnableRemoteQueries|Boolean|Indica se as consultas remotas do índice deste computador serão bloqueadas ou não.|
|searchDisableUseLocation|Boleano|Especifica se a pesquisa pode usar informações de local.|
|searchDisableLocation|Boleano|Especifica se a pesquisa pode usar informações de local.|
|searchDisableIndexerBackoff|Boolean|Indica se o recurso de retirada de indexador de pesquisa deve ou não ser desativado.|
|searchDisableIndexingRemovableDrive|Boolean|Indica se os usuários poderão ou não adicionar locais de unidades removíveis a bibliotecas e para serem indexados.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Especifica uma quantidade mínima de espaço em disco rígido na mesma unidade como o local do índice antes que a indexação seja interrompida.|
|searchBlockWebResults|Boleano|Indica se a pesquisa da Web deve ou não ser bloqueado.|
|findMyFiles|[enablement](../resources/intune-shared-enablement.md)|Controla se o usuário pode configurar a pesquisa para o modo Encontrar Meus Arquivos, que pesquisa arquivos em discos rígidos secundários e também fora do perfil de usuário. Find My Files não permite que os usuários pesquisem arquivos ou locais aos quais eles não têm acesso. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Boleano|Especifique se é necessário permitir a criptografia automática de dispositivo durante o OOBE quando o dispositivo estiver ingressado no Azure AD (somente área de trabalho).|
|diagnosticsDataSubmissionMode|[diagnosticDataSubmissionMode](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|Obtém ou define um valor que permite que o dispositivo envie dados de diagnóstico e de telemetria de uso, como Watson. Os valores possíveis são: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|oneDriveDisableFileSync|Boolean|Obtém ou define um valor para permitir que os administradores de TI impeçam aplicativos e recursos de trabalhar com arquivos no OneDrive.|
|systemTelemetryProxyServer|Cadeia de caracteres|Obtém ou define o FQDN (nome de domínio totalmente qualificado) ou endereço IP de um servidor proxy para encaminhar as experiências do usuário conectado e solicitações de Telemetria.|
|edgeTelemetryForMicrosoft365Analytics|[edgeTelemetryMode](../resources/intune-deviceconfig-edgetelemetrymode.md)|Especifica que tipo de dados de telemetria (nenhum, intranet, internet, ambos) são enviados para Microsoft 365 Analytics. Os valores possíveis são: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.|
|inkWorkspaceAccess|[inkAccessSetting](../resources/intune-deviceconfig-inkaccesssetting.md)|Controla o acesso do usuário ao espaço de trabalho de tinta, da área de trabalho e de cima da tela de bloqueio. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|inkWorkspaceAccessState|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Controla o acesso do usuário ao espaço de trabalho de tinta, da área de trabalho e de cima da tela de bloqueio. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|inkWorkspaceBlockSuggestedApps|Boleano|Especifique se deve mostrar sugestões de aplicativo recomendadas no espaço de trabalho de tinta.|
|smartScreenEnableAppInstallControl|Boolean|Essa propriedade será preterida em julho de 2019 e será substituída pela propriedade SmartScreenAppInstallControl. Permite que os administradores de TI controlem se os usuários poderão instalar aplicativos de lugares que não sejam a Store.|
|smartScreenAppInstallControl|[appInstallControlType](../resources/intune-deviceconfig-appinstallcontroltype.md)|Adicionado na Windows 10, versão 1703. Permite que os administradores de TI controlem se os usuários poderão instalar aplicativos de lugares que não sejam a Store. Os valores possíveis são: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.|
|personalizationDesktopImageUrl|String|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da área de trabalho ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da área de trabalho.|
|personalizationLockScreenImageUrl|String|Uma URL http ou https para uma imagem jpg, jpeg ou png que precisa ser baixada e usada como a imagem da tela de bloqueio ou uma URL de arquivo para uma imagem local no sistema de arquivos que precisa ser usada como a imagem da tela de bloqueio.|
|bluetoothAllowedServices|String collection|Especifica uma lista de serviços e perfis Bluetooth permitidos em cadeias de caracteres de formato hexadecimal.|
|bluetoothBlockAdvertising|Boolean|Se o usuário será ou não impedido de usar a publicidade do bluetooth.|
|bluetoothBlockPromptedProximalConnections|Boleano|Se os usuários usarão o Swift Pair ou não e outros cenários baseados em proximidade.|
|bluetoothBlockDiscoverableMode|Boolean|Se o usuário será ou não impedido de usar o modo de descoberta de bluetooth.|
|bluetoothBlockPrePairing|Boolean|Se determinados periféricos Bluetooth agrupados serão bloqueados ou não do emparelhamento automático com o dispositivo host.|
|edgeBlockAutofill|Boolean|Indica se o preenchimento automático deve ou não ser bloqueado.|
|edgeBlocked|Boolean|Indica se o usuário será ou não impedido de usar o navegador Edge.|
|edgeCookiePolicy|[edgeCookiePolicy](../resources/intune-deviceconfig-edgecookiepolicy.md)|Indica quais cookies bloquear no navegador Edge. Os valores possíveis são: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeBlockDeveloperTools|Boolean|Indica se as ferramentas de desenvolvedor serão bloqueadas ou não no navegador Edge.|
|edgeBlockSendingDoNotTrackHeader|Boolean|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|edgeBlockExtensions|Boolean|Indica se as extensões serão bloqueadas ou não no navegador Edge.|
|edgeBlockInPrivateBrowsing|Boolean|Indica se a navegação InPrivate será bloqueada ou não em redes corporativas no navegador Edge.|
|edgeBlockJavaScript|Boolean|Indica se o usuário será ou não impedido de usar JavaScript.|
|edgeBlockPasswordManager|Boolean|Indica se o gerenciador de senhas será bloqueado ou não.|
|edgeBlockAddressBarDropdown|Boolean|Bloquear a funcionalidade de menu suspenso da barra de endereços no Microsoft Edge. Desabilite essa configuração para minimizar as conexões de rede do Microsoft Edge com serviços Microsoft.|
|edgeBlockCompatibilityList|Boolean|Bloquear lista de compatibilidade da Microsoft no Microsoft Edge. Essa lista da Microsoft ajuda o Edge a exibir corretamente sites com problemas de compatibilidade conhecidos.|
|edgeClearBrowsingDataOnExit|Boolean|Limpar dados de navegação ao sair do Microsoft Edge.|
|edgeAllowStartPagesModification|Boolean|Permitir que os usuários alterem as páginas iniciais no Edge. Use EdgeHomepageUrls para especificar as páginas iniciais que o usuário verá por padrão ao abrir o Edge.|
|edgeDisableFirstRunPage|Boolean|Bloquear a página da Web da Microsoft que é aberta na primeira utilização do Microsoft Edge. Esta política permite que empresas, como aquelas registradas em configurações de emissões zero, bloqueiem esta página.|
|edgeBlockLiveTileDataCollection|Boolean|Bloquear a coleta de informações da Microsoft para criação de bloco dinâmico quando os usuários fixarem um site para iniciar no Microsoft Edge.|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Habilitar a sincronização de favoritos entre o Internet Explorer e o Microsoft Edge. Adições, exclusões, modificações e outras alterações para favoritos são compartilhadas entre navegadores.|
|edgeFavoritesListLocation|Cadeia de caracteres|O local da lista de favoritos a ser provisionamento. Pode ser um arquivo local, rede local ou local http.|
|edgeBlockEditFavorites|Boleano|Indica se o usuário deve ou não bloquear as alterações feitas em Favoritos.|
|edgeNewTabPageURL|Cadeia de caracteres|Especifique a página aberta quando novas guias são criadas.|
|edgeHomeButtonConfiguration|[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|Faz com que o botão Página Inicial seja ocultado, carregue a página Inicial padrão, carregue uma página nova guia ou uma URL personalizada|
|edgeHomeButtonConfigurationEnabled|Boleano|Habilita a configuração do botão Página Inicial.|
|edgeOpensWith|[edgeOpenOptions](../resources/intune-deviceconfig-edgeopenoptions.md)|Especifique que tipo de páginas estão abertas no início. Os valores possíveis são: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|edgeBlockSideloadingExtensions|Boleano|Indica se o usuário pode fazer sideload de extensões.|
|edgeRequiredExtensionPackageFamilyNames|Coleção de cadeias de caracteres|Especifique a lista de nomes de família de pacotes de extensões do navegador que são necessárias e não podem ser desligadas pelo usuário.|
|edgeBlockPrinting|Booliano|Configure Edge para permitir ou bloquear a impressão.|
|edgeFavoritesBarVisibility|[visibilitySetting](../resources/intune-deviceconfig-visibilitysetting.md)|Obter ou definir um valor que especifica se a barra de favoritos deve ser sempre visível ou oculta em qualquer página. Os valores possíveis são: `notConfigured`, `hide`, `show`.|
|edgeBlockSavingHistory|Boleano|Configure o Edge para permitir que o histórico de navegação seja salvo ou nunca salve o histórico de navegação.|
|edgeBlockFullScreenMode|Booliano|Permitir ou impedir que Edge entre no modo de tela inteira.|
|edgeBlockWebContentOnNewTabPage|Boleano|Configure para carregar uma página em branco no Edge em vez da página de guia Nova padrão e impedir que os usuários a mudem.|
|edgeBlockTabPreloading|Boleano|Configure se o Edge pré-carregará a nova página de tabulação na Windows inicialização.|
|edgeBlockPrelaunch|Boleano|Decida se Microsoft Edge pré-inicialização na Windows inicialização.|
|edgeShowMessageWhenOpeningInternetExplorerSites|[internetExplorerMessageSetting](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|Controla a mensagem exibida pelo Edge antes de alternar para o Internet Explorer. Os valores possíveis são: `notConfigured`, `disabled`, `enabled`, `keepGoing`.|
|edgePreventCertificateErrorOverride|Boleano|Permitir ou impedir que os usuários anulam erros de certificado.|
|edgeKioskModeRestriction|[edgeKioskModeRestrictionType](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|Controla como as Microsoft Edge são restritas com base no modo configurar quiosque. Os valores possíveis são: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Especifica o tempo em minutos da última atividade do usuário antes Microsoft Edge de quiosque.  Os valores válidos são 0-1440. O padrão é 5. 0 indica nenhuma redefinição. Valores válidos de 0 a 1440|
|cellularBlockDataWhenRoaming|Boolean|Se o usuário será ou não impedido de usar dados da rede celular durante roaming.|
|cellularBlockVpn|Boolean|Se o usuário será ou não impedido de usar VPN na rede celular.|
|cellularBlockVpnWhenRoaming|Boolean|Se o usuário será ou não impedido de usar VPN durante roaming na rede celular.|
|cellularData|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Se o canal de dados celular deve ou não ser possível no dispositivo. Se não estiver configurado, o canal de dados celular será permitido e o usuário poderá desativar. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|defenderRequireRealTimeMonitoring|Boolean|Indica se o monitoramento em tempo real deve ou não ser exigido.|
|defenderRequireBehaviorMonitoring|Boolean|Indica se o monitoramento de comportamento deve ou não ser exigido.|
|defenderRequireNetworkInspectionSystem|Boolean|Indica se o sistema de inspeção de rede deve ou não ser exigido.|
|defenderScanDownloads|Boolean|Indica se os downloads devem ou não ser verificados.|
|defenderScheduleScanEnableLowCpuPriority|Boleano|Quando habilitada, a baixa prioridade da CPU será usada durante verificações agendadas.|
|defenderDisableCatchupQuickScan|Boleano|Quando bloqueado, as verificações de recuperação de verificações rápidas agendadas serão desligadas.|
|defenderDisableCatchupFullScan|Boleano|Quando bloqueado, as verificações de catch-up para verificações completas agendadas serão desligadas.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Indica se os scripts carregados no navegador Internet Explorer devem ou não ser verificados.|
|defenderBlockEndUserAccess|Boolean|Se o usuário final será ou não impedido de acessar o Defender.|
|defenderSignatureUpdateIntervalInHours|Int32|O intervalo de atualização da assinatura em horas. Especifique 0 para não verificar. Valores válidos de 0 a 24|
|defenderMonitorFileActivity|[defenderMonitorFileActivity](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|Valor de monitoramento da atividade do arquivo. Os valores possíveis são: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Número de dias antes da exclusão do malware em quarentena. Valores válidos de 0 a 90|
|defenderScanMaxCpu|Int32|Porcentagem máxima de uso da CPU durante a verificação. Valores válidos de 0 a 100|
|defenderScanArchiveFiles|Boolean|Indica se os arquivos mortos devem ou não ser verificados.|
|defenderScanIncomingMail|Boolean|Indica se as mensagens de email de entrada devem ou não ser verificadas.|
|defenderScanRemovableDrivesDuringFullScan|Boolean|Indica se as unidades removíveis devem ou não ser verificadas durante a verificação completa.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|Indica se as unidades de rede mapeadas devem ou não ser verificadas durante a verificação completa.|
|defenderScanNetworkFiles|Boolean|Indica se os arquivos abertos de uma pasta da rede devem ou não ser verificados.|
|defenderRequireCloudProtection|Boolean|Indica se a proteção na nuvem deve ou não ser exigida.|
|defenderCloudBlockLevel|[defenderCloudBlockLevelType](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Especifica o nível de proteção oferecido na nuvem. Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Extensão de tempo de tempo para verificação de arquivos pela nuvem. Valores válidos de 0 a 50|
|defenderCloudExtendedTimeoutInSeconds|Int32|Extensão de tempo de tempo para verificação de arquivos pela nuvem. Valores válidos de 0 a 50|
|defenderPromptForSampleSubmission|[defenderPromptForSampleSubmission](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|A configuração do modo como avisar um usuário do envio de exemplo. Os valores possíveis são: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderScheduledQuickScanTime|TimeOfDay|O horário de realização da verificação diária rápida.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|O tipo de verificação do sistema do Defender. Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.|
|defenderSystemScanSchedule|[weeklySchedule](../resources/intune-deviceconfig-weeklyschedule.md)|Dia da semana em que o Defender fará a verificação do sistema. Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|A hora em que o Defender fará a verificação do sistema.|
|defenderPotentiallyUnwantedAppAction|[defenderPotentiallyUnwantedAppAction](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|Obtém ou define a ação do Defender a ser tomada no PuA (Aplicativo Potencialmente Indesejado), que inclui software com comportamentos de injeção de ad, agregação de software, solicitação persistente para pagamento ou assinatura, etc. O Defender alerta o usuário quando o PUA está sendo baixado ou tenta se instalar. Adicionado em Windows 10 para área de trabalho. Os valores possíveis são: `deviceDefault`, `block`, `audit`.|
|defenderPotentiallyUnwantedAppActionSetting|[defenderProtectionType](../resources/intune-deviceconfig-defenderprotectiontype.md)|Obtém ou define a ação do Defender a ser tomada no PuA (Aplicativo Potencialmente Indesejado), que inclui software com comportamentos de injeção de ad, agregação de software, solicitação persistente para pagamento ou assinatura, etc. O Defender alerta o usuário quando o PUA está sendo baixado ou tenta se instalar. Adicionado em Windows 10 para área de trabalho. Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|Verifica se o nível de consentimento do usuário Windows Defender enviar dados. Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderBlockOnAccessProtection|Boleano|Permite ou não permite Windows Defender funcionalidade na Proteção do Access.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Obtém ou define ações do Defender a serem realizadas em um malware detectado por nível de ameaça.|
|defenderFileExtensionsToExclude|String collection|Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.|
|defenderFilesAndFoldersToExclude|String collection|Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.|
|defenderProcessesToExclude|String collection|Processos a serem excluídos das verificações e da proteção em tempo real.|
|lockScreenAllowTimeoutConfiguration|Boolean|Especifique se deseja mostrar uma definição configurável pelo usuário para controlar o tempo limite da tela enquanto estiver na tela de bloqueio de dispositivos Windows Mobile 10. Se essa política estiver definida como Permitir, o valor definido por lockScreenTimeoutInSeconds será ignorado.|
|lockScreenBlockActionCenterNotifications|Boolean|Indica se as notificações da central de ações na tela de bloqueio serão bloqueadas.|
|lockScreenBlockCortana|Boolean|Indica se o usuário pode ou não interagir com a Cortana usando a fala enquanto o sistema estiver bloqueado.|
|lockScreenBlockToastNotifications|Boolean|Indica se serão permitidas notificações do sistema acima da tela de bloqueio do dispositivo.|
|lockScreenTimeoutInSeconds|Int32|Defina a duração (em segundos) da tela de bloqueio para a tela em desligamento para dispositivos Windows Mobile 10. Os valores compatíveis ficam entre 11 e 1800. Valores válidos de 11 a 1800|
|lockScreenActivateAppsWithVoice|[enablement](../resources/intune-shared-enablement.md)|Essa configuração de política especifica se Windows aplicativos podem ser ativados por voz enquanto o sistema está bloqueado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|passwordBlockSimple|Boolean|Especifique se PINs ou senhas como "1111" ou "1234" são permitidas. Para computadores do Windows 10, isso também controla o uso de senhas com imagem.|
|passwordExpirationDays|Int32|A expiração da senha em dias. Valores válidos de 0 a 730|
|passwordMinimumLength|Int32|O comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 50|
|passwordRequired|Boolean|Indica se um usuário deverá ou não ter uma senha.|
|passwordRequireWhenResumeFromIdleState|Boolean|Indica se uma senha deve ou não ser exigida ao sair de um estado inativo.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica. Valores válidos de 0 a 999|
|passwordMinimumAgeInDays|Int32|Essa configuração de segurança determina o período de tempo (em dias) que uma senha deve ser usada para que o usuário possa alterá-la. Valores válidos de 0 a 998|
|privacyAdvertisingId|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Habilita ou desabilita o uso da ID de publicidade. Adicionado no Windows 10, versão 1607. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Indica se será permitida ou não a aceitação automática da caixa de diálogo de consentimento do usuário com emparelhamento e privacidade ao iniciar aplicativos.|
|privacyDisableLaunchExperience|Boleano|Essa política impede que a experiência de privacidade seja lançada durante o logon do usuário para usuários novos e atualizados.|
|privacyBlockInputPersonalization|Boolean|Indica se o uso dos serviços de fala baseados na nuvem será bloqueado para os aplicativos Cortana, Ditado ou Store.|
|privacyBlockPublishUserActivities|Boleano|Bloqueia as experiências compartilhadas/descoberta de recursos usados recentemente no alternador de tarefas etc.|
|privacyBlockActivityFeed|Boleano|Bloqueia o uso de serviços de fala baseados em nuvem para aplicativos Cortana, Ditado ou Store.|
|activateAppsWithVoice|[enablement](../resources/intune-shared-enablement.md)|Especifica se Windows aplicativos podem ser ativados por voz. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|startBlockUnpinningAppsFromTaskbar|Boolean|Indica se o usuário será ou não impedido de desafixar aplicativos da barra de tarefas.|
|startMenuAppListVisibility|[windowsStartMenuAppListVisibilityType](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|A definição desse valor recolhe a lista de aplicativos, remove a lista de aplicativos totalmente ou desabilita a alternância correspondente no aplicativo Configurações. Os valores possíveis são: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolean|Habilitar essa política impede a exibição da configuração de conta de alteração no bloco de usuário no menu Iniciar.|
|startMenuHideFrequentlyUsedApps|Boolean|Habilitar essa política impede a exibição dos aplicativos mais usados no menu Iniciar e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideHibernate|Boolean|Habilitar essa política impede a exibição da hibernação no botão de energia no menu Iniciar.|
|startMenuHideLock|Boolean|Habilitar essa política impede a exibição do bloqueio no bloco de usuário no menu Iniciar.|
|startMenuHidePowerButton|Boolean|Habilitar essa política impede a exibição do botão de energia no menu Iniciar.|
|startMenuHideRecentJumpLists|Boolean|Habilitar essa política impede a exibição de listas de atalhos recentes no menu Iniciar/barra de tarefas e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideRecentlyAddedApps|Boolean|Habilitar essa política impede a exibição de aplicativos adicionados recentemente no menu Iniciar e desabilita a alternância correspondente no aplicativo Configurações.|
|startMenuHideRestartOptions|Boolean|Habilitar essa política impede a exibição da opção “Reiniciar/Atualizar e Reiniciar” no botão de energia no menu Iniciar.|
|startMenuHideShutDown|Boolean|Habilitar essa política impede a exibição da opção desligar/atualizar e desligar no botão de energia no menu Iniciar.|
|startMenuHideSignOut|Boolean|Habilitar essa política impede a exibição da opção Sair no bloco de usuário no menu Iniciar.|
|startMenuHideSleep|Boolean|Habilitar essa política impede a exibição da suspensão no botão de energia no menu Iniciar.|
|startMenuHideSwitchAccount|Boolean|Habilitar essa política impede a exibição da opção Alternar conta no bloco de usuário no menu Iniciar.|
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
|settingsBlockSettingsApp|Boolean|Indica se o acesso ao aplicativo Configurações deve ou não ser bloqueado.|
|settingsBlockSystemPage|Boolean|Indica se o acesso ao Sistemas deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockDevicesPage|Boolean|Indica se o acesso a Dispositivos deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockNetworkInternetPage|Boolean|Indica se o acesso a Rede e Internet deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockPersonalizationPage|Boolean|Indica se o acesso a Personalização deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockAccountsPage|Boolean|Indica se o acesso a Contas deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockTimeLanguagePage|Boolean|Indica se o acesso a Hora e idioma deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockEaseOfAccessPage|Boolean|Indica se o acesso à Facilidade de Acesso deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockPrivacyPage|Boolean|Indica se o acesso à Privacidade deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockUpdateSecurityPage|Boolean|Indica se o acesso a Atualização e Segurança deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockAppsPage|Boolean|Indica se o acesso a Aplicativos deve ou não ser bloqueado no aplicativo Configurações.|
|settingsBlockGamingPage|Boolean|Indica se o acesso a Jogos deve ou não ser bloqueado no aplicativo Configurações.|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|Permite que os administradores de TI bloqueiem experiências que normalmente são apenas para consumidores, como Sugestões de início, Notificações de associação, instalação de aplicativo pós-OOBE e redirecionamento de blocos.|
|windowsSpotlightBlocked|Boolean|Permite que os administradores de TI desativem todos os recursos do Destaque do Windows|
|windowsSpotlightBlockOnActionCenter|Boolean|Bloquear sugestões da Microsoft mostradas após cada instalação limpa do sistema operacional, após upgrades ou de modo contínuo para apresentar aos usuários as novidades ou alterações|
|windowsSpotlightBlockTailoredExperiences|Boolean|Bloquear conteúdo personalizado no Destaque do Windows com base no uso do dispositivo pelo usuário.|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|Bloquear conteúdo de terceiros fornecido por meio do Destaque do Windows|
|windowsSpotlightBlockWelcomeExperience|Boolean|Bloquear a experiência de boas-vindas do Destaque do Windows|
|windowsSpotlightBlockWindowsTips|Boolean|Permite que os administradores de TI desativem os popups de Dicas do Windows.|
|windowsSpotlightConfigureOnLockScreen|[windowsSpotlightEnablementSettings](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|Especifica o tipo de Destaque. Os valores possíveis são: `notConfigured`, `disabled`, `enabled`.|
|networkProxyApplySettingsDeviceWide|Boolean|Se definida, as configurações de proxy serão aplicadas a todos os processos e contas no dispositivo. Caso contrário, serão aplicadas à conta de usuário registrada no MDM.|
|networkProxyDisableAutoDetect|Boolean|Desabilitar a detecção automática de configurações. Se habilitada, o sistema tentará encontrar o caminho para um script de configuração automática de proxy (PAC).|
|networkProxyAutomaticConfigurationUrl|String|Endereço para o script de configuração automática de proxy (PAC) desejado.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/intune-deviceconfig-windows10networkproxyserver.md)|Especifica configurações manuais de servidor proxy.|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.|
|antiTheftModeBlocked|Boolean|Indica se o usuário será ou não impedido de selecionar a preferência do modo AntiTheft (somente no Windows 10 Mobile).|
|bluetoothBlocked|Boolean|Se o usuário será ou não impedido de usar o bluetooth.|
|cameraBlocked|Boolean|Se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|connectedDevicesServiceBlocked|Boolean|Se serão bloqueados ou não o serviço de dispositivos conectados, que permite a descoberta e conexão de outros dispositivos, mensagens remotas, sessões de aplicativo remoto e outras experiências entre dispositivos.|
|certificatesBlockManualRootCertificateInstallation|Boolean|Se o usuário será ou não impedido de fazer a instalação manual do certificado raiz.|
|copyPasteBlocked|Boolean|Se o usuário será ou não impedido de usar a função copiar/colar.|
|cortanaBlocked|Boolean|Se o usuário será ou não impedido de usar a Cortana.|
|deviceManagementBlockFactoryResetOnMobile|Boolean|Se o usuário será ou não impedido de redefinir o telefone.|
|deviceManagementBlockManualUnenroll|Boolean|Indica se o usuário será ou não impedido de cancelar manualmente o registro no gerenciamento de dispositivo.|
|safeSearchFilter|[safeSearchFilterType](../resources/intune-deviceconfig-safesearchfiltertype.md)|Especifica que nível de filtro de pesquisa segura é necessário. Os valores possíveis são: `userDefined`, `strict`, `moderate`.|
|edgeBlockPopups|Boolean|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|edgeBlockSearchSuggestions|Boolean|Indica se o usuário deve ou não bloquear o uso das sugestões de pesquisa na barra de endereços.|
|edgeBlockSearchEngineCustomization|Boleano|Indica se o usuário deve ou não bloquear a adição do novo mecanismo de pesquisa ou a alteração do mecanismo de pesquisa padrão.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|Indica se o tráfego da intranet deve ou não ser alternado do Edge para o Internet Explorer. Observação: o nome dessa propriedade é enganoso; a propriedade é obsoleta, use EdgeSendIntranetTrafficToInternetExplorer.|
|edgeSendIntranetTrafficToInternetExplorer|Boleano|Indica se o tráfego da intranet deve ou não ser alternado do Edge para o Internet Explorer.|
|edgeRequireSmartScreen|Boolean|Indica se o usuário deverá ou não usar o Filtro SmartScreen.|
|edgeEnterpriseModeSiteListLocation|String|Indica o local da lista de sites do modo Empresarial. Pode ser um arquivo local, rede local ou local http.|
|edgeFirstRunUrl|String|A primeira URL a ser executada quando o navegador Edge é aberto pela primeira vez.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)|Permite aos administradores de TI definir um mecanismo de pesquisa padrão para dispositivos controlados por MDM. Os usuários podem substituí-lo e alterar o mecanismo de pesquisa padrão fornecido, caso a política AllowSearchEngineCustomization não esteja definida.|
|edgeHomepageUrls|String collection|A lista de URLs de home pages mostradas em dispositivos registrados no MDM no navegador Edge.|
|edgeBlockAccessToAboutFlags|Boolean|Indica se será impedido ou não o acesso a sinalizadores Sobre no navegador Edge.|
|smartScreenBlockPromptOverride|Boolean|Indica se os usuários poderão ou não substituir avisos do Filtro SmartScreen sobre sites potencialmente maliciosos.|
|smartScreenBlockPromptOverrideForFiles|Boolean|Indica se os usuários poderão ou não substituir os avisos do Filtro SmartScreen sobre sites baixados não verificados.|
|webRtcBlockLocalhostIpAddress|Boolean|Indica se o endereço IP do localhost do usuário será ou não exibido durante chamadas telefônicas usando o WebRTC|
|internetSharingBlocked|Boolean|Indica se o usuário será ou não impedido de usar o compartilhamento de Internet.|
|settingsBlockAddProvisioningPackage|Boolean|Indica se o usuário será ou não impedido de instalar pacotes de provisionamento.|
|settingsBlockRemoveProvisioningPackage|Boolean|Indica se o agente de configuração de tempo de execução será ou não impedido de remover pacotes de provisionamento.|
|settingsBlockChangeSystemTime|Boolean|Indica se o usuário será ou não impedido de alterar configurações de data e hora.|
|settingsBlockEditDeviceName|Boolean|Indica se o usuário será ou não impedido de editar o nome do dispositivo.|
|settingsBlockChangeRegion|Boolean|Indica se o usuário será ou não impedido de alterar as configurações de região.|
|settingsBlockChangeLanguage|Boolean|Indica se o usuário será ou não impedido de alterar as configurações de idioma.|
|settingsBlockChangePowerSleep|Boolean|Indica se o usuário será ou não impedido de alterar as configurações de energia e suspensão.|
|locationServicesBlocked|Boolean|Indica se o usuário será ou não bloqueado dos serviços de localização.|
|microsoftAccountBlocked|Boolean|Indica se uma conta da Microsoft será ou não bloqueada.|
|microsoftAccountBlockSettingsSync|Boolean|Indica se a sincronização de configurações da conta da Microsoft será ou não bloqueada.|
|nfcBlocked|Boolean|Indica se o usuário será ou não impedido de usar a comunicação a curta distância.|
|resetProtectionModeBlocked|Boolean|Indica se o usuário será ou não bloqueado do modo de proteção contra restauração de fábrica.|
|screenCaptureBlocked|Boolean|Indica se o usuário será ou não impedido de fazer capturas de tela.|
|storageBlockRemovableStorage|Boolean|Indica se o usuário será ou não impedido de usar o armazenamento removível.|
|storageRequireMobileDeviceEncryption|Boolean|Indica se a criptografia é ou não necessária em um dispositivo móvel.|
|usbBlocked|Boolean|Indica se o usuário será ou não bloqueado da conexão USB.|
|voiceRecordingBlocked|Boolean|Indica se o usuário será ou não bloqueado da gravação de voz.|
|wiFiBlockAutomaticConnectHotspots|Boolean|Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada. Não terá impacto se o Wi-Fi estiver bloqueado.|
|wiFiBlocked|Boolean|Indica se o usuário será ou não impedido de usar o Wi-Fi.|
|wiFiBlockManualConfiguration|Boolean|Indica se o usuário será ou não impedido de usar a configuração manual do Wi-Fi.|
|wiFiScanInterval|Int32|Especificar com que frequência os dispositivos procuram redes Wi-Fi. Os valores compatíveis ficam entre 1 e 500, em que 100 = padrão e 500 = frequência baixa. Valores válidos de 1 a 500|
|wirelessDisplayBlockProjectionToThisDevice|Boolean|Indica se outros dispositivos poderão ou não descobrir este PC para fins de projeção.|
|wirelessDisplayBlockUserInputFromReceiver|Boolean|Indica se a entrada do usuário pelo receptor de vídeo sem fio será permitida ou não.|
|wirelessDisplayRequirePinForPairing|Boolean|Indica se será exigido um PIN para que novos dispositivo iniciem o emparelhamento.|
|windowsStoreBlocked|Boolean|Indica se o usuário será ou não impedido de usar a Windows Store.|
|appsAllowTrustedAppsSideloading|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indica se aplicativos de pacotes AppX assinados com um certificado confiável podem ser transferidos por sideload. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|windowsStoreBlockAutoUpdate|Boolean|Indica se a atualização automática de aplicativos pela Windows Store será bloqueada ou não.|
|developerUnlockSetting|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indica se o desbloqueio do desenvolver será permitido ou não. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|sharedUserAppDataAllowed|Boolean|Indica se vários usuários do mesmo aplicativo serão ou não impedidos de compartilhar dados.|
|appsBlockWindowsStoreOriginatedApps|Boolean|Indica se será desabilitada ou não a inicialização de todos os aplicativos da Windows Store pré-instalados ou baixados.|
|windowsStoreEnablePrivateStoreOnly|Boolean|Indica se o Repositório particular será ativado ou não.|
|storageRestrictAppDataToSystemVolume|Boolean|Indica se os dados do aplicativo ficarão restritos à unidade do sistema.|
|storageRestrictAppInstallToSystemVolume|Boolean|Indica se a instalação de aplicativos ficará restrita à unidade do sistema.|
|gameDvrBlocked|Boolean|Indica se DVR e difusão serão bloqueados ou não.|
|experienceBlockDeviceDiscovery|Boolean|Indica se a experiência de descoberta de dispositivos será ativada ou não.|
|experienceBlockErrorDialogWhenNoSIM|Boolean|Indica se a caixa de diálogo de erro poderá ou não ser exibida se nenhum cartão SIM for detectado.|
|experienceBlockTaskSwitcher|Boolean|Indica se a alternância de tarefas será ativada ou não no dispositivo.|
|logonBlockFastUserSwitching|Boolean|Desabilita a capacidade para alternar rapidamente entre os usuários conectados simultaneamente sem fazer logoff.|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Boleano|Se o dispositivo é necessário para se conectar à rede.|
|appManagementMSIAllowUserControlOverInstall|Boleano|Essa configuração de política permite que os usuários alterem as opções de instalação que normalmente estão disponíveis apenas para administradores do sistema.|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|Boleano|Essa configuração de política direciona Windows o Instalador a usar permissões elevadas quando instala qualquer programa no sistema.|
|dataProtectionBlockDirectMemoryAccess|Boleano|Essa configuração de política permite que você bloqueie o acesso direto à memória (DMA) para todas as portas de fluxo in-loqueável do PCI a quente até que um usuário entre no Windows.|
|appManagementPackageFamilyNamesToLaunchAfterLogOn|Coleção de cadeias de caracteres|Lista de nomes de família de pacotes delimitados por dois pontos de Windows aplicativos. Os Windows aplicativos listados devem ser lançados após o logon.|
|uninstallBuiltInApps|Booliano|Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.|
|configureTimeZone|Cadeia de caracteres|Especifica o fuso horário a ser aplicado ao dispositivo. Esse é o nome Windows padrão para o fuso horário de destino.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 15009

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "taskManagerBlockEndTask": true,
  "energySaverOnBatteryThresholdPercentage": 7,
  "energySaverPluggedInThresholdPercentage": 7,
  "powerLidCloseActionOnBattery": "noAction",
  "powerLidCloseActionPluggedIn": "noAction",
  "powerButtonActionOnBattery": "noAction",
  "powerButtonActionPluggedIn": "noAction",
  "powerSleepButtonActionOnBattery": "noAction",
  "powerSleepButtonActionPluggedIn": "noAction",
  "powerHybridSleepOnBattery": "enabled",
  "powerHybridSleepPluggedIn": "enabled",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
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
  "findMyFiles": "enabled",
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
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
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderBlockOnAccessProtection": true,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
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
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "activateAppsWithVoice": "enabled",
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
  "edgeBlockSearchEngineCustomization": true,
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
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ],
  "uninstallBuiltInApps": true,
  "configureTimeZone": "Configure Time Zone value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 15181

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
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
  "taskManagerBlockEndTask": true,
  "energySaverOnBatteryThresholdPercentage": 7,
  "energySaverPluggedInThresholdPercentage": 7,
  "powerLidCloseActionOnBattery": "noAction",
  "powerLidCloseActionPluggedIn": "noAction",
  "powerButtonActionOnBattery": "noAction",
  "powerButtonActionPluggedIn": "noAction",
  "powerSleepButtonActionOnBattery": "noAction",
  "powerSleepButtonActionPluggedIn": "noAction",
  "powerHybridSleepOnBattery": "enabled",
  "powerHybridSleepPluggedIn": "enabled",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
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
  "findMyFiles": "enabled",
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
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
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderRequireRealTimeMonitoring": true,
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderMonitorFileActivity": "disable",
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderScanMaxCpu": 2,
  "defenderScanArchiveFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderRequireCloudProtection": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScanType": "disabled",
  "defenderSystemScanSchedule": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderBlockOnAccessProtection": true,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
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
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "activateAppsWithVoice": "enabled",
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
  "edgeBlockSearchEngineCustomization": true,
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
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ],
  "uninstallBuiltInApps": true,
  "configureTimeZone": "Configure Time Zone value"
}
```



