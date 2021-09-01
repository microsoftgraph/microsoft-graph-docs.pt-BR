---
title: Atualizar androidDeviceOwnerGeneralDeviceConfiguration
description: Atualize as propriedades de um objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0791feafc97ded4943c566ad08968a01ec1206b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807199"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a>Atualizar androidDeviceOwnerGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)

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
No corpo da solicitação, fornece uma representação JSON para o [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).

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
|azureAdSharedDeviceDataClearApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que terão seus dados limpos durante uma saída global no modo de dispositivo compartilhado do AAD. Esta coleção pode conter um máximo de 500 elementos.|
|accountsBlockModification|Boleano|Indica se a adição ou remoção de contas está desabilitada.|
|appsAllowInstallFromUnknownSources|Boleano|Indica se o usuário tem ou não permissão para habilitar a configuração de fontes desconhecidas.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Indica o valor da política de atualização automática do aplicativo. Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Indica a política de permissão para solicitações de permissões de tempo de execução se uma não for definida especificamente para o aplicativo. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Booliano|Se todos os aplicativos devem ou não ignorar as dicas de uso pela primeira vez que eles possam ter adicionado.|
|bluetoothBlockConfiguration|Boleano|Indica se um usuário deve ou não bloquear a configuração do bluetooth.|
|bluetoothBlockContactSharing|Boleano|Indica se um usuário deve ou não bloquear o compartilhamento de contatos via bluetooth.|
|cameraBlocked|Boolean|Indica se o uso da câmera deve ou não ser desabilitado.|
|cellularBlockWiFiTethering|Boolean|Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.|
|certificateCredentialConfigurationDisabled|Boleano|Indica se os usuários podem ou não bloquear qualquer configuração de credencial de certificado.|
|microsoftLauncherConfigurationEnabled|Boleano|Indica se você deseja ou não configurar Microsoft Launcher.|
|microsoftLauncherCustomWallpaperEnabled|Boleano|Indica se o papel de parede deve ou não ser configurada nos dispositivos direcionados.|
|microsoftLauncherCustomWallpaperImageUrl|Cadeia de caracteres|Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos direcionados.|
|microsoftLauncherCustomWallpaperAllowUserModification|Boleano|Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.|
|microsoftLauncherFeedEnabled|Boleano|Indica se você deseja ou não habilitar o feed do launcher no dispositivo.|
|microsoftLauncherFeedAllowUserModification|Boleano|Indica se o usuário pode ou não modificar o feed do launcher no dispositivo.|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Indica se você deseja ou não configurar o encaixe do dispositivo. Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.|
|microsoftLauncherDockPresenceAllowUserModification|Boleano|Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Indica a configuração de posicionamento da barra de pesquisa no dispositivo. Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Indica qual perfil de registro você deseja configurar. Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Boleano|Indica se um usuário deve ou não bloquear o roaming de dados.|
|dateTimeConfigurationBlocked|Booliano|Indica se o usuário deve ou não bloquear a alteração manual da data ou hora no dispositivo|
|factoryResetDeviceAdministratorEmails|Coleção de cadeias de caracteres|Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes de poder ser definido.|
|factoryResetBlocked|Boolean|Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|O proxy é definido diretamente com host, porta e hosts excluídos.|
|googleAccountsBlocked|Booliano|Indica se as contas do Google serão ou não bloqueadas.|
|kioskCustomizationDeviceSettingsBlocked|Boleano|Indica se um usuário pode acessar o aplicativo Configurações do dispositivo enquanto estiver no modo Quiosque.|
|kioskCustomizationPowerButtonActionsBlocked|Boleano|Se o menu de energia é mostrado quando um usuário pressiona por muito tempo o botão Ligar de um dispositivo no Modo Quiosque.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Indica se as informações e notificações do sistema estão desabilitadas no modo Quiosque. Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Booliano|Indica se as caixas de diálogo de erro do sistema para aplicativos inativos ou não responsivos são mostradas no modo Quiosque.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Indica quais recursos de navegação estão habilitados no modo Quiosque. Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Booliano|Se deve ou não habilitar o modo de economia de tela ou não no modo Quiosque.|
|kioskModeScreenSaverImageUrl|Cadeia de caracteres|URL de uma imagem que será o protetor de tela do dispositivo no modo Quiosque.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|O número de segundos em que o dispositivo exibirá o protetor de tela no modo Quiosque. Valores válidos de 0 a 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|O número de segundos em que o dispositivo precisa estar inativo para antes que a economia de tela seja mostrada no modo Quiosque. Valores válidos de 1 a 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Boleano|Se a tela do dispositivo deve ou não mostrar o protetor de tela se o áudio/vídeo estiver sendo exibido no modo Quiosque.|
|kioskModeApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeWallpaperUrl|Cadeia de caracteres|URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo Quiosque.|
|kioskModeExitCode|Cadeia de caracteres|Código de saída para permitir que um usuário escape do Modo Quiosque quando o dispositivo estiver no modo Quiosque.|
|kioskModeVirtualHomeButtonEnabled|Boleano|Se será exibido ou não um botão home virtual quando o dispositivo estiver no modo Quiosque.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Indica se o botão home virtual é um botão de passar o dedo para cima ou um botão home flutuante. Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Boleano|Se um usuário pode ou não configurar Bluetooth configurações no modo Quiosque.|
|kioskModeWiFiConfigurationEnabled|Boleano|Se um usuário pode ou não configurar Wi-Fi configurações no Modo Quiosque.|
|kioskModeFlashlightConfigurationEnabled|Boleano|Se um usuário pode ou não usar a lanterna no modo Quiosque.|
|kioskModeMediaVolumeConfigurationEnabled|Boleano|Se um usuário pode ou não alterar o volume de mídia no modo Quiosque.|
|kioskModeShowDeviceInfo|Boleano|Se um usuário pode ou não acessar informações básicas do dispositivo.|
|kioskModeManagedSettingsEntryDisabled|Boleano|Se o ponto de entrada Gerenciado Configurações na tela inicial gerenciada no Modo Quiosque.|
|kioskModeDebugMenuEasyAccessEnabled|Boleano|Se um usuário pode ou não permitir acesso fácil ao menu de depuração no Modo Quiosque.|
|kioskModeShowAppNotificationBadge|Boleano|Se os selos de notificação do aplicativo serão exibidos ou não no modo Quiosque.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Configuração de orientação de tela para tela inicial gerenciada no modo Quiosque. Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Configuração do tamanho do ícone para a tela inicial gerenciada no Modo Quiosque. Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Configuração do ícone de pasta para a tela inicial gerenciada no modo Quiosque. Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Coleção de cadeias de caracteres|O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppOrderEnabled|Booliano|Se é ou não para habilitar a ordenação de aplicativos no modo Quiosque.|
|kioskModeAppsInFolderOrderedByName|Booliano|Se deve ou não alfabéticar aplicativos em uma pasta no modo Quiosque.|
|kioskModeGridHeight|Int32|Número de linhas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo Quiosque. Valores válidos de 1 a 9999999|
|kioskModeGridWidth|Int32|Número de colunas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo Quiosque. Valores válidos de 1 a 9999999|
|kioskModeLockHomeScreen|Boleano|Se deve ou não bloquear a tela inicial para o usuário final no Modo Quiosque.|
|kioskModeManagedFolders|[coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Uma lista de pastas gerenciadas para um dispositivo no modo Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppPositions|[coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|A ordenação de itens na Tela Inicial Gerenciada do Modo quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeManagedHomeScreenAutoSignout|Booliano|Se a saída automática dos aplicativos de modo de dispositivo compartilhado e MHS e MHS será automaticamente inativa após a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Número de segundos para notificação do usuário antes de assalá-los automaticamente para a Tela Inicial Gerenciada. Valores válidos de 1 a 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Número de segundos em que o dispositivo está inativo antes de assinar automaticamente o usuário para a Tela Inicial Gerenciada. Valores válidos de 1 a 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Complexidade do PIN para sessão de login para Tela Inicial Gerenciada. Os valores possíveis são: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Boleano|Se o usuário precisa ou não definir um PIN para sessão de login para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenPinRequiredToResume|Booliano|Se o usuário precisa ou não inserir PIN de sessão se o screensaver tiver sido exibido para a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInBackground|Cadeia de caracteres|Plano de fundo de URL personalizado para tela de login para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInBrandingLogo|Cadeia de caracteres|Logotipo de identidade visual de URL personalizado para tela de logon e página de pin de sessão para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInEnabled|Boleano|Se a tela de login será ou não para Tela Inicial Gerenciada.|
|microphoneForceMute|Boleano|Indica se o microfone deve ou não ser bloqueado no dispositivo.|
|networkEscapeHatchAllowed|Boleano|Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.|
|nfcBlockOutgoingBeam|Boleano|Indica se o raio de saída NFC deve ou não ser bloqueado.|
|passwordBlockKeyguard|Boleano|Indica se o keyguard está desabilitado ou não.|
|passwordBlockKeyguardFeatures|[coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Lista de recursos de proteção de chave do dispositivo a ser bloqueado. Essa coleção pode conter um máximo de 7 elementos. Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.|
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
|safeBootBlocked|Boleano|Indica se a reinicialização ou não do dispositivo na inicialização segura está desabilitada.|
|screenCaptureBlocked|Boolean|Indica se o recurso deve ou não ser desabilitado para fazer capturas de tela.|
|securityAllowDebuggingFeatures|Boleano|Indica se o usuário deve ou não bloquear a habilitação de recursos de depuração no dispositivo.|
|securityDeveloperSettingsEnabled|Boleano|Indica se o usuário tem ou não permissão para acessar configurações de desenvolvedor, como opções de desenvolvedor e inicialização segura no dispositivo.|
|securityRequireVerifyApps|Boolean|Indica se os aplicativos são ou não necessários.|
|statusBarBlocked|Boleano|Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.|
|stayOnModes|[coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Lista de modos em que a exibição do dispositivo permanecerá acionada. Essa coleção pode conter no máximo quatro elementos. Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.|
|storageAllowUsb|Boleano|Indica se é ou não para permitir o armazenamento em massa USB.|
|storageBlockExternalMedia|Boleano|Indica se a mídia externa deve ou não ser bloqueado.|
|storageBlockUsbFileTransfer|Boleano|Indica se a transferência de arquivo USB deve ou não ser bloqueado.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada. Valores válidos de 0 a 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina. Valores válidos de 0 a 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|O tipo de configuração de atualização do sistema. Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Boleano|Se deve ou não bloquear janelas de prompt do sistema Android, como notualizações, atividades telefônicas e alertas do sistema.|
|usersBlockAdd|Boleano|Indica se a adição ou não de usuários e perfis está desabilitada.|
|usersBlockRemove|Boleano|Indica se deve ou não desabilitar a remoção de outros usuários do dispositivo.|
|volumeBlockAdjustment|Boleano|Indica se o ajuste do volume mestre está desabilitado ou não.|
|vpnAlwaysOnLockdownMode|Boleano|Se um nome de pacote VPN sempre estiver especificado, se o tráfego de rede será ou não travado quando essa VPN estiver desconectada.|
|vpnAlwaysOnPackageIdentifier|Cadeia de caracteres|Nome do pacote do aplicativo Android para aplicativo que lidará com uma conexão VPN sempre on.|
|wifiBlockEditConfigurations|Boleano|Indica se o usuário deve ou não bloquear a edição das configurações de conexão wifi.|
|wifiBlockEditPolicyDefinedConfigurations|Boleano|Indica se o usuário deve ou não bloquear a edição apenas das redes definidas pela política.|
|personalProfileAppsAllowInstallFromUnknownSources|Boleano|Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.|
|personalProfileCameraBlocked|Booliano|Indica se o uso da câmera deve ser desabilitado no perfil pessoal.|
|personalProfileScreenCaptureBlocked|Boleano|Indica se a funcionalidade deve ser desabilitada para fazer capturas de tela no perfil pessoal.|
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



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8247

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
  "kioskModeManagedHomeScreenPinComplexity": "simple",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8419

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
  "azureAdSharedDeviceDataClearApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "kioskModeManagedHomeScreenAutoSignout": true,
  "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": 7,
  "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": 8,
  "kioskModeManagedHomeScreenPinComplexity": "simple",
  "kioskModeManagedHomeScreenPinRequired": true,
  "kioskModeManagedHomeScreenPinRequiredToResume": true,
  "kioskModeManagedHomeScreenSignInBackground": "Kiosk Mode Managed Home Screen Sign In Background value",
  "kioskModeManagedHomeScreenSignInBrandingLogo": "Kiosk Mode Managed Home Screen Sign In Branding Logo value",
  "kioskModeManagedHomeScreenSignInEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```



