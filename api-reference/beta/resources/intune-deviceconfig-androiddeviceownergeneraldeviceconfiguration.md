---
title: Tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2bcdc14b586f29907424c7414b74ae1dfe763a3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159070"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>Tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[Coleção androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Listar propriedades e relações dos objetos [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Obter androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Leia as propriedades e as relações do [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Criar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Crie um novo [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Excluir androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Nenhum(a)|Exclui [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Atualizar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Atualizar as propriedades de um [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de Marcas de Escopo para esta instância de Entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountsBlockModification|Boolean|Indica se a adição ou remoção de contas está desabilitada ou não.|
|appsAllowInstallFromUnknownSources|Boolean|Indica se o usuário tem permissão ou não para habilitar a configuração de fontes desconhecidas.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Indica o valor da política de atualização automática do aplicativo. Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Indica a política de permissão para solicitações de permissões de tempo de execução se uma delas não estiver definida especificamente para o aplicativo. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Boolean|Se todos os aplicativos devem ou não ignorar qualquer dica de uso pela primeira vez que eles possam ter adicionado.|
|bluetoothBlockConfiguration|Boolean|Indica se um usuário será ou não bloqueado para configurar o bluetooth.|
|bluetoothBlockContactSharing|Boolean|Indica se um usuário será ou não bloqueado de compartilhar contatos via bluetooth.|
|cameraBlocked|Boolean|Indica se o uso da câmera deve ou não ser desabilitado.|
|cellularBlockWiFiTethering|Boolean|Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.|
|certificateCredentialConfigurationDisabled|Boolean|Indica se os usuários são ou não bloqueados de qualquer configuração de credencial de certificado.|
|microsoftLauncherConfigurationEnabled|Boolean|Indica se você deseja ou não configurar o Microsoft Launcher.|
|microsoftLauncherCustomWallpaperEnabled|Boolean|Indica se o papel de parede deve ou não ser configurado nos dispositivos de alvo.|
|microsoftLauncherCustomWallpaperImageUrl|String|Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos de alvo.|
|microsoftLauncherCustomWallpaperAllowUserModification|Boolean|Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.|
|microsoftLauncherFeedEnabled|Boolean|Indica se você deseja ou não habilitar o feed do launcher no dispositivo.|
|microsoftLauncherFeedAllowUserModification|Boolean|Indica se o usuário pode ou não modificar o feed do launcher no dispositivo.|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Indica se você deseja ou não configurar o encaixe do dispositivo. Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.|
|microsoftLauncherDockPresenceAllowUserModification|Boolean|Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Indica a configuração de posicionamento da barra de pesquisa no dispositivo. Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Indica qual perfil de registro você deseja configurar. Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Boolean|Indica se um usuário será ou não bloqueado de roaming de dados.|
|dateTimeConfigurationBlocked|Boolean|Indica se o usuário será ou não bloqueado alterando manualmente a data ou hora no dispositivo|
|factoryResetDeviceAdministratorEmails|Coleção de cadeias de caracteres|Lista de emails da conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes que ele possa ser definido.|
|factoryResetBlocked|Boolean|Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|O proxy é definido diretamente com hosts host, porta e hosts excluídos.|
|googleAccountsBlocked|Boolean|Indica se as contas do Google serão bloqueadas ou não.|
|kioskCustomizationDeviceSettingsBlocked|Boolean|Indica se um usuário pode acessar o aplicativo Configurações do dispositivo no Modo de Quiosque.|
|kioskCustomizationPowerButtonActionsBlocked|Boolean|Se o menu ligar/desligar é mostrado quando um usuário pressiona por muito tempo o botão Ligar/Desligar de um dispositivo no Modo de Quiosque.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Indica se as informações do sistema e as notificações estão desabilitadas no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Boolean|Indica se as caixas de diálogo de erro do sistema para aplicativos com falha ou sem resposta são mostradas no Modo de Quiosque.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Indica quais recursos de navegação estão habilitados no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Boolean|Se o modo de economia de tela deve ou não ser habilitado ou não no Modo de Quiosque.|
|kioskModeScreenSaverImageUrl|String|URL para uma imagem que será a economia de tela do dispositivo no Modo de Quiosque.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|O número de segundos que o dispositivo exibirá a economia de tela no Modo de Quiosque. Valores válidos de 0 a 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|O número de segundos que o dispositivo precisa ficar inativo para que a economia de tela seja mostrada no Modo de Quiosque. Valores válidos de 1 a 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|Se a tela do dispositivo deve ou não mostrar a economia de tela se o áudio/vídeo estiver sendo exibido no Modo de Quiosque.|
|kioskModeApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeWallpaperUrl|String|URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo está no modo quiosque.|
|kioskModeExitCode|String|Código de saída para permitir que um usuário escape do Modo de Quiosque quando o dispositivo estiver no Modo de Quiosque.|
|kioskModeVirtualHomeButtonEnabled|Boolean|Se um botão página virtual será exibido ou não quando o dispositivo estiver no Modo de Quiosque.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Indica se o botão página principal virtual é um botão página página principal ou um botão página página início flutuante. Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Boolean|Se um usuário poderá ou não definir as configurações de Bluetooth no Modo de Quiosque.|
|kioskModeWiFiConfigurationEnabled|Boolean|Se um usuário poderá ou não definir as configurações Wi-Fi no Modo de Quiosque.|
|kioskModeFlashlightConfigurationEnabled|Boolean|Se um usuário poderá ou não usar a lanterna no Modo de Quiosque.|
|kioskModeMediaVolumeConfigurationEnabled|Boolean|Se um usuário pode ou não alterar o volume de mídia no Modo de Quiosque.|
|kioskModeShowDeviceInfo|Boolean|Se um usuário poderá ou não acessar informações básicas do dispositivo.|
|kioskModeManagedSettingsEntryDisabled|Boolean|Se o ponto de entrada Configurações Gerenciadas deve ou não ser exibido na tela inicial gerenciada no Modo de Quiosque.|
|kioskModeDebugMenuEasyAccessEnabled|Boolean|Se um usuário poderá ou não acessar facilmente o menu de depuração no Modo de Quiosque.|
|kioskModeShowAppNotificationBadge|Boolean|Se os selos de notificação de aplicativo serão exibidos ou não no Modo de Quiosque.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Configuração de orientação da tela inicial gerenciada no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Configuração do tamanho do ícone para a tela inicial gerenciada no Modo de Quiosque. Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Configuração de ícone de pasta para tela inicial gerenciada no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Coleção de cadeias de caracteres|O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppOrderEnabled|Boolean|Se o pedido do aplicativo será habilitado ou não no Modo de Quiosque.|
|kioskModeAppsInFolderOrderedByName|Boolean|Se os aplicativos serão ou não alfabéticos em uma pasta no Modo de Quiosque.|
|kioskModeGridHeight|Int32|Número de linhas para grade da Tela Inicial Gerenciada com ordenação de aplicativos habilitada no Modo de Quiosque. Valores válidos de 1 a 9999999|
|kioskModeGridWidth|Int32|Número de colunas para grade da Tela Inicial Gerenciada com ordenação de aplicativos habilitada no Modo de Quiosque. Valores válidos de 1 a 9999999|
|kioskModeLockHomeScreen|Boolean|Se a tela inicial será ou não lock para o usuário final no Modo de Quiosque.|
|kioskModeManagedFolders|[Coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Uma lista de pastas gerenciadas para um dispositivo no Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppPositions|[Coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|A ordenação de itens na tela inicial gerenciada do Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|microphoneForceMute|Boolean|Indica se o microfone deve ou não ser bloqueado no dispositivo.|
|networkEscapeHatchAllowed|Boolean|Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.|
|nfcBlockOutgoingBeam|Boolean|Indica se o raio de saída NFC deve ou não ser bloqueado.|
|passwordBlockKeyguard|Boolean|Indica se a keyguard está ou não desabilitada.|
|passwordBlockKeyguardFeatures|[Coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Lista de recursos de proteção de chaves do dispositivo a ser bloqueado. Essa coleção pode conter um máximo de 7 elementos.|
|passwordExpirationDays|Int32|Indica quanto tempo uma senha pode ser definida antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Indica o comprimento mínimo da senha necessária no dispositivo. Valores válidos de 4 a 16|
|passwordMinimumLetterCharacters|Int32|Indica o número mínimo de caracteres de carta necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumLowerCaseCharacters|Int32|Indica o número mínimo de caracteres de casos inferiores necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumNonLetterCharacters|Int32|Indica o número mínimo de caracteres sem letra necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumNumericCharacters|Int32|Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumSymbolCharacters|Int32|Indica o número mínimo de caracteres de símbolos necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumUpperCaseCharacters|Int32|Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordCountToBlock|Int32|Indica a duração do histórico de senhas, em que o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico. Valores válidos de 0 a 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínima de senha necessária no dispositivo. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode inserir uma senha incorreta antes de o dispositivo ser apagado. Valores válidos de 4 a 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Indica o modo da Play Store do dispositivo. Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.|
|safeBootBlocked|Boolean|Indica se a reinicialização do dispositivo na inicialização segura está desabilitada ou não.|
|screenCaptureBlocked|Boolean|Indica se a funcionalidade deve ou não ser desabilitada para fazer capturas de tela.|
|securityAllowDebuggingFeatures|Boolean|Indica se o usuário será ou não bloqueado da habilitação de recursos de depuração no dispositivo.|
|securityRequireVerifyApps|Boolean|Indica se os aplicativos são necessários ou não.|
|statusBarBlocked|Boolean|Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.|
|stayOnModes|[Coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Lista de modos em que a exibição do dispositivo se manterá ligado. Essa coleção pode conter um máximo de 4 elementos.|
|storageAllowUsb|Boolean|Indica se o armazenamento em massa USB será ou não permitir.|
|storageBlockExternalMedia|Boolean|Indica se a mídia externa deve ou não ser bloqueado.|
|storageBlockUsbFileTransfer|Boolean|Indica se a transferência de arquivo USB deve ou não ser bloqueado.|
|systemUpdateWindowStartMinutesAfterMidafter|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada. Valores válidos de 0 a 1440|
|systemUpdateWindowEndMinutesAfterMidafter|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina. Valores válidos de 0 a 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|O tipo de configuração de atualização do sistema. Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Boolean|Se as janelas de prompt do sistema Android serão ou não bloqueados, como notualizações do sistema, atividades de telefone e alertas do sistema.|
|usersBlockAdd|Boolean|Indica se a adição de usuários e perfis está desabilitada ou não.|
|usersBlockRemove|Boolean|Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.|
|volumeBlockAdjustment|Boolean|Indica se o ajuste do volume mestre está desabilitado ou não.|
|vpnAlwaysOnLockdownMode|Boolean|Se um nome de pacote VPN sempre em uso for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.|
|vpnAlwaysOnPackageIdentifier|String|Nome do pacote do aplicativo Android para o aplicativo que lidará com uma conexão VPN sempre on.|
|wifiBlockEditConfigurations|Boolean|Indica se o usuário será ou não bloqueado para editar as configurações de conexão wi-fi.|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|Indica se o usuário será ou não bloqueado de editar apenas as redes definidas pela política.|
|personalProfileAppsAllowInstallFromUnknownSources|Boolean|Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.|
|personalProfileCameraBlocked|Boolean|Indica se o uso da câmera no perfil pessoal deve ser desabilitado.|
|personalProfileScreenCaptureBlocked|Boolean|Indica se a funcionalidade deve ser desabilitada para fazer capturas de tela no perfil pessoal.|
|workProfilePasswordExpirationDays|Int32|Indica o número de dias que uma senha de perfil de trabalho pode ser definida antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|workProfilePasswordMinimumLength|Int32|Indica o comprimento mínimo da senha do perfil de trabalho. Valores válidos de 4 a 16|
|workProfilePasswordMinimumNumericCharacters|Int32|Indica o número mínimo de caracteres numéricos necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|Indica o número mínimo de caracteres sem letra necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumLetterCharacters|Int32|Indica o número mínimo de caracteres de carta necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|Indica o número mínimo de caracteres de casos inferiores necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|Indica o número mínimo de caracteres de letra maiúscula necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|Indica o número mínimo de caracteres de símbolos necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|Indica a duração do histórico de senhas do perfil de trabalho, em que o usuário não poderá inserir uma nova senha igual à de qualquer senha no histórico. Valores válidos de 0 a 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode inserir uma senha de perfil de trabalho incorreta antes que o dispositivo seja apagado. Valores válidos de 4 a 11|
|workProfilePasswordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínima de senha necessária na senha do perfil de trabalho. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "String",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "String",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "String",
  "enrollmentProfile": "String",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "String"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "String",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "String",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "String",
  "kioskModeScreenSaverDisplayTimeInSeconds": 1024,
  "kioskModeScreenSaverStartDelayInSeconds": 1024,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "kioskModeWallpaperUrl": "String",
  "kioskModeExitCode": "String",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "String",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "String",
  "kioskModeIconSize": "String",
  "kioskModeFolderIcon": "String",
  "kioskModeWifiAllowedSsids": [
    "String"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 1024,
  "kioskModeGridWidth": 1024,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "String",
      "folderIdentifier": "String",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "String",
          "link": "String"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 1024,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "String",
        "link": "String"
      }
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumLetterCharacters": 1024,
  "passwordMinimumLowerCaseCharacters": 1024,
  "passwordMinimumNonLetterCharacters": 1024,
  "passwordMinimumNumericCharacters": 1024,
  "passwordMinimumSymbolCharacters": 1024,
  "passwordMinimumUpperCaseCharacters": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "playStoreMode": "String",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinimumNumericCharacters": 1024,
  "workProfilePasswordMinimumNonLetterCharacters": 1024,
  "workProfilePasswordMinimumLetterCharacters": 1024,
  "workProfilePasswordMinimumLowerCaseCharacters": 1024,
  "workProfilePasswordMinimumUpperCaseCharacters": 1024,
  "workProfilePasswordMinimumSymbolCharacters": 1024,
  "workProfilePasswordPreviousPasswordCountToBlock": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String"
}
```




