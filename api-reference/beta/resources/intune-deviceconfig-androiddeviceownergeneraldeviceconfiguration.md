---
title: Tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration
description: Este tópico fornece descrições dos métodos, propriedades e relações declarados expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c20d7b658362ca5f05d79e6450019dc06c48fbe3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203222"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>Tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos, propriedades e relações declarados expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[coleção androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Listar propriedades e relações dos [objetos androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Obter androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Ler propriedades e relações do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Criar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Crie um novo [objeto androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Excluir androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Nenhuma|Exclui um [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Atualizar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Atualize as propriedades de um [objeto androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|azureAdSharedDeviceDataClearApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que terão seus dados limpos durante uma saída global AAD de dispositivo compartilhado. Esta coleção pode conter um máximo de 500 elementos.|
|accountsBlockModification|Booliano|Indica se a adição ou remoção de contas está desabilitada.|
|appsAllowInstallFromUnknownSources|Booliano|Indica se o usuário tem ou não permissão para habilitar a configuração de fontes desconhecidas.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Indica o valor da política de atualização automática do aplicativo. Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Indica a política de permissão para solicitações de permissões de runtime se uma não estiver definida especificamente para o aplicativo. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Booliano|Se todos os aplicativos devem ou não ignorar as dicas de uso da primeira vez que eles podem ter adicionado.|
|bluetoothBlockConfiguration|Booliano|Indica se um usuário deve ou não impedir a configuração de bluetooth.|
|bluetoothBlockContactSharing|Booliano|Indica se um usuário deve ou não bloquear o compartilhamento de contatos via bluetooth.|
|cameraBlocked|Boolean|Indica se o uso da câmera deve ou não ser desabilitado.|
|cellularBlockWiFiTethering|Boolean|Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.|
|certificateCredentialConfigurationDisabled|Booliano|Indica se os usuários devem ou não ser bloqueados de qualquer configuração de credencial de certificado.|
|crossProfilePoliciesAllowCopyPaste|Booliano|Indica se o texto copiado de um perfil (pessoal ou de trabalho) pode ou não ser colado no outro.|
|crossProfilePoliciesAllowDataSharing|[androidDeviceOwnerCrossProfileDataSharing](../resources/intune-deviceconfig-androiddeviceownercrossprofiledatasharing.md)|Indica se os dados de um perfil (pessoal ou de trabalho) podem ser compartilhados com aplicativos no outro perfil. Os valores possíveis são: `notConfigured`, `crossProfileDataSharingBlocked`, `dataSharingFromWorkToPersonalBlocked`, `crossProfileDataSharingAllowed`, `unkownFutureValue`.|
|crossProfilePoliciesShowWorkContactsInPersonalProfile|Booliano|Indica se os contatos armazenados no perfil de trabalho são mostrados ou não em pesquisas de contato de perfil pessoal/chamadas de entrada.|
|microsoftLauncherConfigurationEnabled|Booliano|Indica se você deseja ou não configurar Microsoft Launcher.|
|microsoftLauncherCustomWallpaperEnabled|Booliano|Indica se o papel de parede deve ou não ser configurado nos dispositivos de destino.|
|microsoftLauncherCustomWallpaperImageUrl|Cadeia de Caracteres|Indica a URL para o arquivo de imagem a ser usado como papel de parede nos dispositivos de destino.|
|microsoftLauncherCustomWallpaperAllowUserModification|Booliano|Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.|
|microsoftLauncherFeedEnabled|Booliano|Indica se você deseja ou não habilitar o feed do inicializador no dispositivo.|
|microsoftLauncherFeedAllowUserModification|Booliano|Indica se o usuário pode ou não modificar o feed do inicializador no dispositivo.|
|microsoftLauncherDockPresenceConfiguration|[microsoftLauncherDockPresence](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|Indica se você deseja ou não configurar o encaixe do dispositivo. Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.|
|microsoftLauncherDockPresenceAllowUserModification|Booliano|Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.|
|microsoftLauncherSearchBarPlacementConfiguration|[microsoftLauncherSearchBarPlacement](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|Indica a configuração de posicionamento da barra de pesquisa no dispositivo. Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.|
|enrollmentProfile|[androidDeviceOwnerEnrollmentProfileType](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|Indica qual perfil de registro você deseja configurar. Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.|
|dataRoamingBlocked|Booliano|Indica se um usuário deve ou não ser bloqueado do roaming de dados.|
|dateTimeConfigurationBlocked|Boolean|Indica se o usuário deve ou não bloquear a alteração manual da data ou hora no dispositivo|
|detailedHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|Representa o texto de ajuda detalhado personalizado fornecido aos usuários quando eles tentam modificar as configurações gerenciadas em seus dispositivos.|
|factoryResetDeviceAdministratorEmails|Conjunto de cadeias de caracteres|Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes que ele possa ser configurado.|
|factoryResetBlocked|Boolean|Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.|
|globalProxy|[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|O proxy é configurado diretamente com hosts host, porta e excluídos.|
|googleAccountsBlocked|Boolean|Indica se as contas do Google serão bloqueadas ou não.|
|kioskCustomizationDeviceSettingsBlocked|Booliano|Indica se um usuário pode acessar o aplicativo Configurações dispositivo enquanto estiver no Modo de Quiosque.|
|kioskCustomizationPowerButtonActionsBlocked|Boolean|Se o menu de energia é mostrado quando um usuário pressiona por muito tempo o botão Ligar/Desligar de um dispositivo no Modo de Quiosque.|
|kioskCustomizationStatusBar|[androidDeviceOwnerKioskCustomizationStatusBar](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|Indica se as informações e notificações do sistema estão desabilitadas no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.|
|kioskCustomizationSystemErrorWarnings|Booliano|Indica se as caixas de diálogo de erro do sistema para aplicativos com falha ou sem resposta são mostradas no Modo de Quiosque.|
|kioskCustomizationSystemNavigation|[androidDeviceOwnerKioskCustomizationSystemNavigation](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|Indica quais recursos de navegação estão habilitados no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.|
|kioskModeScreenSaverConfigurationEnabled|Booliano|Se deseja ou não habilitar o modo de proteção de tela ou não no Modo de Quiosque.|
|kioskModeScreenSaverImageUrl|Cadeia de Caracteres|URL para uma imagem que será a proteção de tela do dispositivo no Modo de Quiosque.|
|kioskModeScreenSaverDisplayTimeInSeconds|Int32|O número de segundos para os quais o dispositivo exibirá a proteção de tela no Modo de Quiosque. Valores válidos de 0 a 9999999|
|kioskModeScreenSaverStartDelayInSeconds|Int32|O número de segundos que o dispositivo precisa ficar inativo para antes que a proteção de tela seja mostrada no Modo de Quiosque. Valores válidos de 1 a 9999999|
|kioskModeScreenSaverDetectMediaDisabled|Booliano|Se a tela do dispositivo deve ou não mostrar a proteção de tela se o áudio/vídeo estiver sendo reproduzido no Modo de Quiosque.|
|kioskModeApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeWallpaperUrl|Cadeia de Caracteres|URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no Modo de Quiosque.|
|kioskModeExitCode|Cadeia de Caracteres|Saia do código para permitir que um usuário escape do Modo de Quiosque quando o dispositivo estiver no Modo de Quiosque.|
|kioskModeVirtualHomeButtonEnabled|Booliano|Se um botão página inicial virtual deve ou não ser exibido quando o dispositivo estiver no Modo de Quiosque.|
|kioskModeVirtualHomeButtonType|[androidDeviceOwnerVirtualHomeButtonType](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|Indica se o botão página inicial virtual é um botão passar o dedo para cima da página inicial ou um botão página inicial flutuante. Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.|
|kioskModeBluetoothConfigurationEnabled|Booliano|Se deseja ou não permitir que um usuário defina Bluetooth configurações no Modo de Quiosque.|
|kioskModeWiFiConfigurationEnabled|Booliano|Se deseja ou não permitir que um usuário defina Wi-Fi configurações no Modo de Quiosque.|
|kioskModeFlashlightConfigurationEnabled|Booliano|Se um usuário deve ou não usar a lanterna no Modo de Quiosque.|
|kioskModeMediaVolumeConfigurationEnabled|Booliano|Se um usuário pode ou não alterar o volume de mídia no Modo de Quiosque.|
|kioskModeShowDeviceInfo|Booliano|Se um usuário pode ou não acessar informações básicas do dispositivo.|
|kioskModeManagedSettingsEntryDisabled|Booliano|Se deseja ou não exibir o ponto de Configurações gerenciado na tela inicial gerenciada no Modo de Quiosque.|
|kioskModeDebugMenuEasyAccessEnabled|Booliano|Se um usuário pode ou não facilitar o acesso ao menu de depuração no Modo de Quiosque.|
|kioskModeShowAppNotificationBadge|Booliano|Se as notificações do aplicativo devem ou não ser exibidas no Modo de Quiosque.|
|kioskModeScreenOrientation|[androidDeviceOwnerKioskModeScreenOrientation](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|Configuração de orientação de tela para a tela inicial gerenciada no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.|
|kioskModeIconSize|[androidDeviceOwnerKioskModeIconSize](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|Configuração do tamanho do ícone para a tela inicial gerenciada no Modo de Quiosque. Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.|
|kioskModeFolderIcon|[androidDeviceOwnerKioskModeFolderIcon](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|Configuração de ícone de pasta para a tela inicial gerenciada no Modo de Quiosque. Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.|
|kioskModeWifiAllowedSsids|Coleção de cadeias de caracteres|O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppOrderEnabled|Booliano|Se deseja ou não habilitar a ordenação de aplicativos no Modo de Quiosque.|
|kioskModeAppsInFolderOrderedByName|Boolean|Se os aplicativos devem ou não ser alfabéticos dentro de uma pasta no Modo de Quiosque.|
|kioskModeGridHeight|Int32|Número de linhas para a grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo de Quiosque. Valores válidos de 1 a 9999999|
|kioskModeGridWidth|Int32|Número de colunas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo de Quiosque. Valores válidos de 1 a 9999999|
|kioskModeLockHomeScreen|Booliano|Se deseja ou não bloquear a tela inicial para o usuário final no Modo de Quiosque.|
|kioskModeManagedFolders|[coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)|Uma lista de pastas gerenciadas para um dispositivo no Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeAppPositions|[coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)|A ordenação de itens na Tela Inicial Gerenciada do Modo de Quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeManagedHomeScreenAutoSignout|Boolean|Se deseja ou não sair automaticamente dos aplicativos de modo de dispositivo compartilhado e MHS após inativo para a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds|Int32|Número de segundos para notificação do usuário antes de desacioná-los automaticamente para a Tela Inicial Gerenciada. Valores válidos de 0 a 9999999|
|kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds|Int32|Número de segundos em que o dispositivo está inativo antes de sair automaticamente do usuário para a Tela Inicial Gerenciada. Valores válidos de 0 a 9999999|
|kioskModeManagedHomeScreenPinComplexity|[kioskModeManagedHomeScreenPinComplexity](../resources/intune-deviceconfig-kioskmodemanagedhomescreenpincomplexity.md)|Complexidade do PIN para sessão de entrada para a Tela Inicial Gerenciada. Os valores possíveis são: `notConfigured`, `simple`, `complex`.|
|kioskModeManagedHomeScreenPinRequired|Booliano|Se o usuário precisa ou não definir um PIN para sessão de entrada para a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenPinRequiredToResume|Booliano|Se o usuário precisa ou não inserir o PIN da sessão se o protetor de tela tiver sido exibido para a Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInBackground|Cadeia de Caracteres|Tela de fundo da URL personalizada para a tela de entrada da Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInBrandingLogo|Cadeia de Caracteres|Logotipo de identidade visual de URL personalizado para tela de entrada e página de pino de sessão para Tela Inicial Gerenciada.|
|kioskModeManagedHomeScreenSignInEnabled|Booliano|Se a tela de entrada será exibida ou não para a Tela Inicial Gerenciada.|
|kioskModeUseManagedHomeScreenApp|[kioskModeType](../resources/intune-deviceconfig-kioskmodetype.md)|Se deseja ou não usar o modo de quiosque de aplicativo único ou o modo de quiosque de vários aplicativos. Os valores possíveis são: `notConfigured`, `singleAppMode`, `multiAppMode`.|
|microphoneForceMute|Booliano|Indica se o microfone deve ou não ser bloqueado no dispositivo.|
|networkEscapeHatchAllowed|Booliano|Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.|
|nfcBlockOutgoingBeam|Booliano|Indica se o raio de saída NFC deve ou não ser bloqueado.|
|passwordBlockKeyguard|Booliano|Indica se o keyguard está desabilitado ou não.|
|passwordBlockKeyguardFeatures|[coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Lista de recursos de keyguard do dispositivo a serem bloqueados. Essa coleção pode conter um máximo de 7 elementos.|
|passwordExpirationDays|Int32|Indica a quantidade de tempo para a qual uma senha pode ser definida antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Indica o comprimento mínimo da senha necessária no dispositivo. Valores válidos de 4 a 16|
|passwordMinimumLetterCharacters|Int32|Indica o número mínimo de caracteres de letra necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumLowerCaseCharacters|Int32|Indica o número mínimo de caracteres minúsculos necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumNonLetterCharacters|Int32|Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumNumericCharacters|Int32|Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumSymbolCharacters|Int32|Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinimumUpperCaseCharacters|Int32|Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo. Valores válidos de 1 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordCountToBlock|Int32|Indica o comprimento do histórico de senhas, em que o usuário não poderá inserir uma nova senha que seja a mesma que qualquer senha no histórico. Valores válidos de 0 a 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínima de senha necessária no dispositivo. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordRequireUnlock|[androidDeviceOwnerRequiredPasswordUnlock](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordunlock.md)|Indica o período de tempo limite após o qual um dispositivo deve ser desbloqueado usando uma forma de autenticação forte. Os valores possíveis são: `deviceDefault`, `daily`, `unkownFutureValue`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado. Valores válidos de 4 a 11|
|playStoreMode|[androidDeviceOwnerPlayStoreMode](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|Indica o modo da Play Store do dispositivo. Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.|
|screenCaptureBlocked|Boolean|Indica se a capacidade de fazer capturas de tela deve ou não ser desabilitada.|
|securityDeveloperSettingsEnabled|Booliano|Indica se o usuário tem ou não permissão para acessar configurações de desenvolvedor, como opções de desenvolvedor e inicialização segura no dispositivo.|
|securityRequireVerifyApps|Boolean|Indica se os aplicativos são necessários ou não.|
|shortHelpText|[androidDeviceOwnerUserFacingMessage](../resources/intune-deviceconfig-androiddeviceowneruserfacingmessage.md)|Representa o texto de ajuda curto personalizado fornecido aos usuários quando eles tentam modificar as configurações gerenciadas em seus dispositivos.|
|statusBarBlocked|Booliano|Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.|
|stayOnModes|[coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Lista de modos em que a exibição do dispositivo permanecerá ligada. Essa coleção pode conter um máximo de 4 elementos.|
|storageAllowUsb|Booliano|Indica se o armazenamento em massa USB deve ou não ser permitido.|
|storageBlockExternalMedia|Booliano|Indica se a mídia externa deve ou não ser bloqueado.|
|storageBlockUsbFileTransfer|Booliano|Indica se a transferência de arquivo USB deve ou não ser bloqueado.|
|systemUpdateFreezePeriods|[coleção androidDeviceOwnerSystemUpdateFreezePeriod](../resources/intune-deviceconfig-androiddeviceownersystemupdatefreezeperiod.md)|Indica os períodos de tempo de repetição anual durante os quais as atualizações do sistema são adiadas. Esta coleção pode conter um máximo de 500 elementos.|
|systemUpdateWindowStartMinutesAfterMiddate|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada. Valores válidos de 0 a 1440|
|systemUpdateWindowEndMinutesAfterMiddate|Int32|Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina. Valores válidos de 0 a 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|O tipo de configuração de atualização do sistema. Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Booliano|Se as janelas de prompt do sistema Android devem ou não ser bloqueados, como notificações do sistema, atividades telefônicas e alertas do sistema.|
|usersBlockAdd|Booliano|Indica se a adição de usuários e perfis está desabilitada ou não.|
|usersBlockRemove|Booliano|Indica se deseja ou não desabilitar a remoção de outros usuários do dispositivo.|
|volumeBlockAdjustment|Booliano|Indica se o ajuste do volume mestre está desabilitado ou não.|
|vpnAlwaysOnLockdownMode|Booliano|Se um nome de pacote VPN always on for especificado, se o tráfego de rede será bloqueado ou não quando essa VPN estiver desconectada.|
|vpnAlwaysOnPackageIdentifier|Cadeia de Caracteres|Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativada.|
|wifiBlockEditConfigurations|Booliano|Indica se o usuário deve ou não impedir a edição das configurações de conexão wi-fi.|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|Indica se o usuário deve ou não impedir a edição apenas das redes definidas pela política.|
|personalProfileAppsAllowInstallFromUnknownSources|Booliano|Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.|
|personalProfileCameraBlocked|Booliano|Indica se o uso da câmera no perfil pessoal deve ser desabilitado.|
|personalProfileScreenCaptureBlocked|Booliano|Indica se é necessário desabilitar a capacidade de fazer capturas de tela no perfil pessoal.|
|personalProfilePlayStoreMode|[personalProfilePersonalPlayStoreMode](../resources/intune-deviceconfig-personalprofilepersonalplaystoremode.md)|Usado junto com PersonalProfilePersonalApplications para controlar como os aplicativos no perfil pessoal são permitidos ou bloqueados. Os valores possíveis são: `notConfigured`, `blockedApps`, `allowedApps`.|
|personalProfilePersonalApplications|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Política aplicada a aplicativos no perfil pessoal. Esta coleção pode conter um máximo de 500 elementos.|
|workProfilePasswordExpirationDays|Int32|Indica o número de dias em que uma senha de perfil de trabalho pode ser definida antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|workProfilePasswordMinimumLength|Int32|Indica o comprimento mínimo da senha do perfil de trabalho. Valores válidos de 4 a 16|
|workProfilePasswordMinimumNumericCharacters|Int32|Indica o número mínimo de caracteres numéricos necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumNonLetterCharacters|Int32|Indica o número mínimo de caracteres que não são letras necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumLetterCharacters|Int32|Indica o número mínimo de caracteres de letra necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumLowerCaseCharacters|Int32|Indica o número mínimo de caracteres minúsculos necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumUpperCaseCharacters|Int32|Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordMinimumSymbolCharacters|Int32|Indica o número mínimo de caracteres de símbolo necessários para a senha do perfil de trabalho. Valores válidos de 1 a 16|
|workProfilePasswordPreviousPasswordCountToBlock|Int32|Indica o comprimento do histórico de senha do perfil de trabalho, em que o usuário não poderá inserir uma nova senha que seja a mesma que qualquer senha no histórico. Valores válidos de 0 a 24|
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
  "detailedHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "String",
        "value": "String"
      }
    ],
    "defaultMessage": "String"
  },
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
  "kioskModeUseManagedHomeScreenApp": "String",
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
  "passwordRequireUnlock": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "playStoreMode": "String",
  "screenCaptureBlocked": true,
  "securityDeveloperSettingsEnabled": true,
  "securityRequireVerifyApps": true,
  "shortHelpText": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage",
    "localizedMessages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "String",
        "value": "String"
      }
    ],
    "defaultMessage": "String"
  },
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateFreezePeriods": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
      "startMonth": 1024,
      "startDay": 1024,
      "endMonth": 1024,
      "endDay": 1024
    }
  ],
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




