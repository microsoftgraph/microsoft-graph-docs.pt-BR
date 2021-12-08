---
title: tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration
description: Este tópico fornece descrições dos métodos, propriedades e relações declarados expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d35ce8623390b1a6312f8807e7610fc3a9353ff
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347708"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos, propriedades e relações declarados expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[coleção androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Listar propriedades e relações dos objetos [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Obter androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Leia propriedades e relações do [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Criar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Crie um novo [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|
|[Excluir androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Nenhum|Exclui um [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Atualizar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Atualize as propriedades de [um objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|azureAdSharedDeviceDataClearApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que terão seus dados limpos durante uma saída global no AAD de dispositivo compartilhado. Esta coleção pode conter um máximo de 500 elementos.|
|accountsBlockModification|Boolean|Indica se a adição ou remoção de contas está desabilitada.|
|appsAllowInstallFromUnknownSources|Booliano|Indica se o usuário tem ou não permissão para habilitar a configuração de fontes desconhecidas.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Indica o valor da política de atualização automática do aplicativo. Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Indica a política de permissão para solicitações de permissões de tempo de execução se uma não for definida especificamente para o aplicativo. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Booliano|Se todos os aplicativos devem ou não ignorar as dicas de uso pela primeira vez que eles possam ter adicionado.|
|bluetoothBlockConfiguration|Boolean|Indica se um usuário deve ou não bloquear a configuração do bluetooth.|
|bluetoothBlockContactSharing|Booliano|Indica se um usuário deve ou não bloquear o compartilhamento de contatos via bluetooth.|
|cameraBlocked|Boolean|Indica se o uso da câmera deve ou não ser desabilitado.|
|cellularBlockWiFiTethering|Boolean|Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.|
|certificateCredentialConfigurationDisabled|Booliano|Indica se os usuários podem ou não bloquear qualquer configuração de credencial de certificado.|
|crossProfilePoliciesAllowCopyPaste|Boolean|Indica se o texto copiado de um perfil (pessoal ou profissional) pode ou não ser copiado no outro.|
|crossProfilePoliciesAllowDataSharing|[androidDeviceOwnerCrossProfileDataSharing](../resources/intune-deviceconfig-androiddeviceownercrossprofiledatasharing.md)|Indica se os dados de um perfil (pessoal ou de trabalho) podem ser compartilhados com aplicativos no outro perfil. Os valores possíveis são: `notConfigured`, `crossProfileDataSharingBlocked`, `dataSharingFromWorkToPersonalBlocked`, `crossProfileDataSharingAllowed`, `unkownFutureValue`.|
|crossProfilePoliciesShowWorkContactsInPersonalProfile|Booliano|Indica se os contatos armazenados no perfil de trabalho são mostrados em pesquisas de contato de perfil pessoal/chamadas de entrada.|
|microsoftLauncherConfigurationEnabled|Booliano|Indica se você deseja ou não configurar Microsoft Launcher.|
|microsoftLauncherCustomWallpaperEnabled|Booliano|Indica se o papel de parede deve ou não ser configurada nos dispositivos direcionados.|
|microsoftLauncherCustomWallpaperImageUrl|String|Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos direcionados.|
|microsoftLauncherCustomWallpaperAllowUserModification|Booliano|Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.|
|microsoftLauncherFeedEnabled|Boolean|Indica se você deseja ou não habilitar o feed do launcher no dispositivo.|
|microsoftLauncherFeedAllowUserModification|Boolean|Indica se o usuário pode ou não modificar o feed do launcher no dispositivo.|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Indica se você deseja ou não configurar o encaixe do dispositivo. Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.|
|microsoftLauncherDockPresenceAllowUserModification|Boolean|Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Indica a configuração de posicionamento da barra de pesquisa no dispositivo. Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Indica qual perfil de registro você deseja configurar. Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Boolean|Indica se um usuário deve ou não bloquear o roaming de dados.|
|dateTimeConfigurationBlocked|Booliano|Indica se o usuário deve ou não bloquear a alteração manual da data ou hora no dispositivo|
|factoryResetDeviceAdministratorEmails|Coleção de cadeias de caracteres|Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes de poder ser definido.|
|factoryResetBlocked|Boolean|Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|O proxy é definido diretamente com host, porta e hosts excluídos.|
|googleAccountsBlocked|Boolean|Indica se as contas do Google serão ou não bloqueadas.|
|kioskCustomizationDeviceSettingsBlocked|Booliano|Indica se um usuário pode acessar o aplicativo Configurações do dispositivo enquanto estiver no modo Quiosque.|
|kioskCustomizationPowerButtonActionsBlocked|Booliano|Se o menu de energia é mostrado quando um usuário pressiona por muito tempo o botão Ligar de um dispositivo no Modo Quiosque.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Indica se as informações e notificações do sistema estão desabilitadas no modo Quiosque. Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Booliano|Indica se as caixas de diálogo de erro do sistema para aplicativos inativos ou não responsivos são mostradas no modo Quiosque.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Indica quais recursos de navegação estão habilitados no modo Quiosque. Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Boolean|Se deve ou não habilitar o modo de economia de tela ou não no modo Quiosque.|
|kioskModeScreenSaverImageUrl|String|URL de uma imagem que será o protetor de tela do dispositivo no modo Quiosque.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|O número de segundos em que o dispositivo exibirá o protetor de tela no modo Quiosque. Valores válidos de 0 a 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|O número de segundos em que o dispositivo precisa estar inativo para antes que a economia de tela seja mostrada no modo Quiosque. Valores válidos de 1 a 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boolean|Se a tela do dispositivo deve ou não mostrar o protetor de tela se o áudio/vídeo estiver sendo exibido no modo Quiosque.|
|kioskModeApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeWallpaperUrl|String|URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo Quiosque.|
|kioskModeExitCode|String|Código de saída para permitir que um usuário escape do Modo Quiosque quando o dispositivo estiver no modo Quiosque.|
|kioskModeVirtualHomeButtonEnabled|Boolean|Se será exibido ou não um botão home virtual quando o dispositivo estiver no modo Quiosque.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Indica se o botão home virtual é um botão de passar o dedo para cima ou um botão home flutuante. Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Boolean|Se um usuário pode ou não configurar Bluetooth configurações no modo Quiosque.|
|kioskModeWiFiConfigurationEnabled|Booliano|Se um usuário pode ou não configurar Wi-Fi configurações no Modo Quiosque.|
|kioskModeFlashlightConfigurationEnabled|Boolean|Se um usuário pode ou não usar a lanterna no modo Quiosque.|
|kioskModeMediaVolumeConfigurationEnabled|Booliano|Se um usuário pode ou não alterar o volume de mídia no modo Quiosque.|
|kioskModeShowDeviceInfo|Boolean|Se um usuário pode ou não acessar informações básicas do dispositivo.|
|kioskModeManagedSettingsEntryDisabled|Boolean|Se o ponto de entrada Gerenciado Configurações na tela inicial gerenciada no Modo Quiosque.|
|kioskModeDebugMenuEasyAccessEnabled|Booliano|Se um usuário pode ou não permitir acesso fácil ao menu de depuração no Modo Quiosque.|
|kioskModeShowAppNotificationBadge|Booliano|Se os selos de notificação do aplicativo serão exibidos ou não no modo Quiosque.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Configuração de orientação de tela para tela inicial gerenciada no modo Quiosque. Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Configuração do tamanho do ícone para a tela inicial gerenciada no Modo Quiosque. Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Configuração do ícone de pasta para a tela inicial gerenciada no modo Quiosque. Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Coleção String|O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppOrderEnabled|Booliano|Se é ou não para habilitar a ordenação de aplicativos no modo Quiosque.|
|kioskModeAppsInFolderOrderedByName|Booliano|Se deve ou não alfabéticar aplicativos em uma pasta no modo Quiosque.|
|kioskModeGridHeight|Int32|Número de linhas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo Quiosque. Valores válidos de 1 a 9999999|
|kioskModeGridWidth|Int32|Número de colunas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo Quiosque. Valores válidos de 1 a 9999999|
|kioskModeLockHomeScreen|Booliano|Se deve ou não bloquear a tela inicial para o usuário final no Modo Quiosque.|
|kioskModeManagedFolders|[coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Uma lista de pastas gerenciadas para um dispositivo no modo Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppPositions|[coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|A ordenação de itens na Tela Inicial Gerenciada do Modo quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeManagedHomeScreenAutoSignout|Booliano|Se a saída automática dos aplicativos de modo de dispositivo compartilhado e MHS e MHS será automaticamente inativa após a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Número de segundos para notificação do usuário antes de assalá-los automaticamente para a Tela Inicial Gerenciada. Valores válidos de 0 a 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Número de segundos em que o dispositivo está inativo antes de assinar automaticamente o usuário para a Tela Inicial Gerenciada. Valores válidos de 0 a 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Complexidade do PIN para sessão de login para Tela Inicial Gerenciada. Os valores possíveis são: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Boolean|Se o usuário precisa ou não definir um PIN para sessão de login para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenPinRequiredToResume|Booliano|Se o usuário precisa ou não inserir PIN de sessão se o screensaver tiver sido exibido para a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInBackground|String|Plano de fundo de URL personalizado para tela de login para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInBrandingLogo|String|Logotipo de identidade visual de URL personalizado para tela de logon e página de pin de sessão para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInEnabled|Boolean|Se a tela de login será ou não para Tela Inicial Gerenciada.|
|microphoneForceMute|Booliano|Indica se o microfone deve ou não ser bloqueado no dispositivo.|
|networkEscapeHatchAllowed|Booliano|Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.|
|nfcBlockOutgoingBeam|Booliano|Indica se o raio de saída NFC deve ou não ser bloqueado.|
|passwordBlockKeyguard|Booliano|Indica se o keyguard está desabilitado ou não.|
|passwordBlockKeyguardFeatures|[coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Lista de recursos de proteção de chave do dispositivo a ser bloqueado. Essa coleção pode conter um máximo de 7 elementos.|
|passwordExpirationDays|Int32|Indica a quantidade de tempo em que uma senha pode ser definida antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Indica o tamanho mínimo da senha necessária no dispositivo. Valores válidos de 4 a 16|
|passwordMinimumLetterCharacters|Int32|Indica o número mínimo de caracteres de letra necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumLowerCaseCharacters|Int32|Indica o número mínimo de caracteres de caixa inferiores necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumNonLetterCharacters|Int32|Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumNumericCharacters|Int32|Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumSymbolCharacters|Int32|Indica o número mínimo de caracteres de símbolo necessário para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumUpperCaseCharacters|Int32|Indica o número mínimo de caracteres de letras maiúsculas de maiúsculas e médios necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordCountToBlock|Int32|Indica o tamanho do histórico de senhas, em que o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico. Valores válidos de 0 a 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínima de senha necessária no dispositivo. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado. Valores válidos de 4 a 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Indica o modo Play Store do dispositivo. Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.|
|screenCaptureBlocked|Boolean|Indica se o recurso deve ou não ser desabilitado para fazer capturas de tela.|
|securityDeveloperSettingsEnabled|Booliano|Indica se o usuário tem ou não permissão para acessar configurações de desenvolvedor, como opções de desenvolvedor e inicialização segura no dispositivo.|
|securityRequireVerifyApps|Boolean|Indica se os aplicativos são ou não necessários.|
|statusBarBlocked|Booliano|Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.|
|stayOnModes|[coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Lista de modos em que a exibição do dispositivo permanecerá acionada. Essa coleção pode conter no máximo quatro elementos.|
|storageAllowUsb|Booliano|Indica se é ou não para permitir o armazenamento em massa USB.|
|storageBlockExternalMedia|Booliano|Indica se a mídia externa deve ou não ser bloqueado.|
|storageBlockUsbFileTransfer|Booliano|Indica se a transferência de arquivo USB deve ou não ser bloqueado.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada. Valores válidos de 0 a 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina. Valores válidos de 0 a 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|O tipo de configuração de atualização do sistema. Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Boolean|Se deve ou não bloquear janelas de prompt do sistema Android, como notualizações, atividades telefônicas e alertas do sistema.|
|usersBlockAdd|Boolean|Indica se a adição ou não de usuários e perfis está desabilitada.|
|usersBlockRemove|Boolean|Indica se deve ou não desabilitar a remoção de outros usuários do dispositivo.|
|volumeBlockAdjustment|Boolean|Indica se o ajuste do volume mestre está desabilitado ou não.|
|vpnAlwaysOnLockdownMode|Booliano|Se um nome de pacote VPN sempre estiver especificado, se o tráfego de rede será ou não travado quando essa VPN estiver desconectada.|
|vpnAlwaysOnPackageIdentifier|String|Nome do pacote do aplicativo Android para aplicativo que lidará com uma conexão VPN sempre on.|
|wifiBlockEditConfigurations|Booliano|Indica se o usuário deve ou não bloquear a edição das configurações de conexão wifi.|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|Indica se o usuário deve ou não bloquear a edição apenas das redes definidas pela política.|
|personalProfileAppsAllowInstallFromUnknownSources|Booliano|Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.|
|personalProfileCameraBlocked|Booliano|Indica se o uso da câmera deve ser desabilitado no perfil pessoal.|
|personalProfileScreenCaptureBlocked|Booliano|Indica se a funcionalidade deve ser desabilitada para fazer capturas de tela no perfil pessoal.|
|personalProfilePlayStoreMode|[personalProfilePersonalPlayStoreMode](../resources/intune-deviceconfig-personalprofilepersonalplaystoremode.md)|Usado em conjunto com PersonalProfilePersonalApplications para controlar como os aplicativos no perfil pessoal são permitidos ou bloqueados. Os valores possíveis são: `notConfigured`, `blockedApps`, `allowedApps`.|
|personalProfilePersonalApplications|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Política aplicada a aplicativos no perfil pessoal. Esta coleção pode conter um máximo de 500 elementos.|
|workProfilePasswordExpirationDays|Int32|Indica o número de dias em que uma senha de perfil de trabalho pode ser definida antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|workProfilePasswordMinimumLength|Int32|Indica o tamanho mínimo da senha do perfil de trabalho. Valores válidos de 4 a 16|
|workProfilePasswordMinimumNumericCharacters|Int32|Indica o número mínimo de caracteres numéricos necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|Indica o número mínimo de caracteres que não são letras necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumLetterCharacters|Int32|Indica o número mínimo de caracteres de letra necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|Indica o número mínimo de caracteres de caso inferior necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|Indica o número mínimo de caracteres de letra de maiúsculas e altas necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|Indica o número mínimo de caracteres de símbolo necessário para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|Indica o tamanho do histórico de senhas do perfil de trabalho, onde o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico. Valores válidos de 0 a 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode inserir uma senha de perfil de trabalho incorreta antes que o dispositivo seja apagado. Valores válidos de 4 a 11|
|workProfilePasswordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínima de senha necessária na senha do perfil de trabalho. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|

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
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
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
  "crossProfilePoliciesAllowCopyPaste": true,
  "crossProfilePoliciesAllowDataSharing": "String",
  "crossProfilePoliciesShowWorkContactsInPersonalProfile": true,
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
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 1024,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 1024,
  "kioskModeManagedHomeScreenPinComplexity": "String",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "String",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "String",
  "kioskModeManagedHomeScreenSignInEnabled": true,
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
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
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
  "personalProfilePlayStoreMode": "String",
  "personalProfilePersonalApplications": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
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




