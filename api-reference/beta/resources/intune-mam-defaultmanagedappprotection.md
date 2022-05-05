---
title: Tipo de recurso defaultManagedAppProtection
description: Política usada para definir configurações de gerenciamento detalhadas para um conjunto especificado de aplicativos para todos os usuários não direcionados por uma política TargetedManagedAppProtection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d48dcfadd511b145483a3203f791688339083561
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206129"
---
# <a name="defaultmanagedappprotection-resource-type"></a>Tipo de recurso defaultManagedAppProtection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política usada para definir configurações de gerenciamento detalhadas para um conjunto especificado de aplicativos para todos os usuários não direcionados por uma política TargetedManagedAppProtection


Herda de [managedAppProtection](../resources/intune-mam-managedappprotection.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar defaultManagedAppProtections](../api/intune-mam-defaultmanagedappprotection-list.md)|Coleção [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Listar propriedades e relações dos objetos [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Obter defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Ler propriedades e relações do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Criar defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-create.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Criar um novo objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Excluir defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-delete.md)|Nenhum|Excluir um [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Atualizar defaultManagedAppProtection](../api/intune-mam-defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Atualizar as propriedades de um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|descrição|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo está conectado à Internet. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Fontes das quais os dados podem ser transferidos. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Destinos para os quais os dados podem ser transferidos. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Indica se as credenciais organizacionais são obrigatórias para o uso do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|O nível em que a área de transferência pode ser compartilhada entre os aplicativos no dispositivo gerenciado. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Indica se o backup de dados de um aplicativo gerenciado está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|deviceComplianceRequired|Boolean|Indica se a compatibilidade de dispositivos é necessária. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|Indica se os links da Internet devem ser abertos no aplicativo do navegador gerenciado ou em qualquer navegador personalizado especificado por CustomBrowserProtocol (para iOS) ou CustomBrowserPackageId/CustomBrowserDisplayName (para Android) Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas de repetição de pino incorretas antes que o aplicativo gerenciado seja bloqueado ou apagado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[Coleção managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumRequiredOsVersion|Cadeia de Caracteres|Versões maiores que a versão especificada impedirão que o aplicativo gerenciado acesse os dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumWarningOsVersion|Cadeia de Caracteres|Versões maiores que a versão especificada impedirão que o aplicativo gerenciado acesse os dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumWipeOsVersion|Cadeia de Caracteres|Versões maiores que a versão especificada impedirão que o aplicativo gerenciado acesse os dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|Cadeia de Caracteres|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|Cadeia de Caracteres|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja bloquear ou apagar, quando o dispositivo estiver com raiz ou com jailbreak, se DeviceComplianceRequired estiver definido como true. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja bloquear ou apagar, com base no número máximo de tentativas de repetição de pino incorretas. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Tempo limite em minutos para um pin de aplicativo em vez de senha não biométrica Herdada de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|Especifique o número de caracteres que podem ser cortados ou copiados de dados e contas da organização para qualquer aplicativo. Essa configuração substitui a restrição AllowedOutboundClipboardSharingLevel. O valor padrão de '0' significa que nenhuma exceção é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Especifique a restrição de notificação de aplicativo [herdada de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allow`, `blockOrganizationalData`, `block`.|
|previousPinBlockCount|Int32|Requer que um pino seja exclusivo do número especificado nesta propriedade. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|Indica em quais navegadores gerenciados os links da Internet devem ser abertos. Quando essa propriedade é configurada, ManagedBrowserToOpenLinksRequired deve ser true. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `notConfigured` e `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Nível máximo de ameaça de dispositivo permitido, conforme relatado pelo aplicativo MTD Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Determina qual ação executar se o limite de ameaças de defesa contra ameaças móveis não for atendido. Warn não é um valor com suporte para essa propriedade Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Booliano|Indica se um usuário pode trazer dados para documentos da organização. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataIngestionLocations|[Coleção managedAppDataIngestionLocation](../resources/intune-mam-managedappdataingestionlocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Se definido, ele especificará qual ação executar no caso em que o usuário não puder fazer check-in porque o token de autenticação é inválido. Isso acontece quando o usuário é excluído ou desabilitado no AAD. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|dialerRestrictionLevel|[managedAppPhoneNumberRedirectLevel](../resources/intune-mam-managedappphonenumberredirectlevel.md)|As classes de aplicativos discadores que têm permissão para clicar para abrir um número de telefone. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `customApp`, `blocked`.|
|gracePeriodToBlockAppsDuringOffClockHours|Duration|Um período de carência antes de bloquear o acesso ao aplicativo fora do horário comercial. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Tipo de criptografia que deve ser usada para dados em um aplicativo gerenciado. (Somente iOS). Os valores possíveis são: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Boolean|Indica se a captura de tela está bloqueada. (Somente Android)|
|encryptAppData|Boolean|Indica se os dados de aplicativos gerenciados devem ser criptografados. (Somente Android)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|Quando essa configuração estiver habilitada, a criptografia no nível do aplicativo será desabilitada se a criptografia no nível do dispositivo estiver habilitada. (Somente Android)|
|minimumRequiredSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. (Somente iOS)|
|customSettings|Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos usuários afetados, não alterados por esse serviço|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|minimumRequiredPatchVersion|String|Define o nível mais antigo de patch de segurança do Android necessário que um usuário pode ter para obter acesso seguro ao aplicativo. (Somente Android)|
|minimumWarningPatchVersion|String|Define o nível mais antigo de patch de segurança do Android recomendado que um usuário pode ter para obter acesso seguro ao aplicativo. (Somente Android)|
|exemptedAppProtocols|Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Os aplicativos iOS nesta lista serão isentos da política e poderão receber dados de aplicativos gerenciados. (Somente iOS)|
|exemptedAppPackages|Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Os pacotes de aplicativos Android nesta lista serão isentos da política e poderão receber dados de aplicativos gerenciados. (Somente Android)|
|faceIdBlocked|Boolean|Indica se será permitido o uso do FaceID em vez de um pin se PinRequired estiver definido como True. (Somente iOS)|
|minimumWipeSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|minimumWipePatchVersion|Cadeia de Caracteres|O nível de patch de segurança do Android menor ou igual ao valor especificado apagará o aplicativo gerenciado e os dados da empresa associados. (Somente Android)|
|allowedIosDeviceModels|Cadeia de Caracteres|Lista separada por ponto e vírgula de modelos de dispositivo permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione. (Somente iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja bloquear ou apagar, se o modelo de dispositivo especificado não for permitido. (Somente iOS). Os valores possíveis são: `block`, `wipe`, `warn`.|
|allowedAndroidDeviceManufacturers|Cadeia de Caracteres|A lista separada por ponto e vírgula de fabricantes de dispositivos permitiu, como uma cadeia de caracteres, que o aplicativo gerenciado funciona. (Somente Android)|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja bloquear ou apagar, se o fabricante do dispositivo especificado não for permitido. (somente Android). Os valores possíveis são: `block`, `wipe`, `warn`.|
|thirdPartyKeyboardsBlocked|Booliano|Define se teclados de terceiros são permitidos ao acessar um aplicativo gerenciado. (Somente iOS)|
|filterOpenInToOnlyManagedApps|Booliano|Define se a operação de abertura tem suporte do aplicativo gerenciado para os locais de compartilhamento de arquivos selecionados. Essa configuração só se aplica quando AllowedOutboundDataTransferDestinations é definido como ManagedApps e DisableProtectionOfManagedOutboundOpenInData é definido como False. (Somente iOS)|
|disableProtectionOfManagedOutboundOpenInData|Booliano|Desabilite a proteção de dados transferidos para outros aplicativos por meio da opção IOS OpenIn. Essa configuração só pode ser True quando AllowedOutboundDataTransferDestinations é definido como ManagedApps. (Somente iOS)|
|protectInboundDataFromUnknownSources|Booliano|Proteger dados de entrada de origem desconhecida. Essa configuração só pode ser True quando AllowedInboundDataTransferSources é definido como AllApps. (Somente iOS)|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Define o requisito de Atestado de Dispositivo Do Android SafetyNet para que um aplicativo gerenciado funcione. Os valores possíveis são: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, aviso ou bloqueio, se o requisito de atestado do Android SafetyNet especificado falhar. Os valores possíveis são: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Define o requisito de Verificação de Aplicativos SafetyNet do Android para que um aplicativo gerenciado funcione. Os valores possíveis são: `none` e `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, aviso ou bloqueio, se o requisito de Verificação de Aplicativo Android especificado falhar. Os valores possíveis são: `block`, `wipe`, `warn`.|
|customBrowserProtocol|Cadeia de Caracteres|Um protocolo de navegador personalizado para abrir o weblink no iOS. (somente iOS)|
|customBrowserPackageId|Cadeia de Caracteres|Identificador exclusivo de um navegador personalizado para abrir o weblink no Android. (Somente Android)|
|customBrowserDisplayName|Cadeia de Caracteres|Nome amigável do navegador personalizado preferencial para abrir o weblink no Android. (Somente Android)|
|minimumRequiredCompanyPortalVersion|Cadeia de Caracteres|A versão mínima do portal da empresa que deve ser instalada no dispositivo ou no acesso ao aplicativo será bloqueada|
|minimumWarningCompanyPortalVersion|Cadeia de Caracteres|Versão mínima do portal da empresa que deve ser instalada no dispositivo ou o usuário receberá um aviso|
|minimumWipeCompanyPortalVersion|Cadeia de Caracteres|A versão mínima do portal da empresa que deve ser instalada no dispositivo ou os dados da empresa no aplicativo serão apagados|
|allowedAndroidDeviceModels|Coleção de cadeias de caracteres|Lista de modelos de dispositivo permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione. (Somente Android)|
|appActionIfAndroidDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja bloquear ou apagar, se o modelo de dispositivo especificado não for permitido. (Somente Android). Os valores possíveis são: `block`, `wipe`, `warn`.|
|customDialerAppProtocol|Cadeia de Caracteres|Protocolo de um aplicativo de discagem personalizado para clicar para abrir um número de telefone no iOS, por exemplo, skype:.|
|customDialerAppPackageId|Cadeia de Caracteres|PackageId de um aplicativo de discagem personalizado para clicar para abrir um número de telefone no Android.|
|customDialerAppDisplayName|Cadeia de Caracteres|Nome amigável de um aplicativo de discagem personalizado para clicar para abrir um número de telefone no Android.|
|biometricAuthenticationBlocked|Booliano|Indica se o uso da autenticação biométrica será permitido no lugar de um pino se PinRequired estiver definido como True. (Somente Android)|
|requiredAndroidSafetyNetEvaluationType|[androidManagedAppSafetyNetEvaluationType](../resources/intune-mam-androidmanagedappsafetynetevaluationtype.md)|Define o requisito de tipo de avaliação do Android SafetyNet para que um aplicativo gerenciado funcione. (Somente Android). Os valores possíveis são: `basic` e `hardwareBacked`.|
|blockAfterCompanyPortalUpdateDeferralInDays|Int32|O número máximo de dias Portal da Empresa a atualização pode ser adiada no dispositivo ou o acesso ao aplicativo será bloqueado.|
|warnAfterCompanyPortalUpdateDeferralInDays|Int32|Número máximo de dias Portal da Empresa atualização pode ser adiada no dispositivo ou o usuário receberá o aviso|
|wipeAfterCompanyPortalUpdateDeferralInDays|Int32|Número máximo de dias Portal da Empresa atualização pode ser adiada no dispositivo ou os dados da empresa no aplicativo serão apagados|
|deviceLockRequired|Booliano|Define se qualquer tipo de bloqueio deve ser necessário no dispositivo. (somente android)|
|appActionIfDeviceLockNotSet|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, aviso, bloqueio ou apagamento, se o bloqueio de tela for necessário no dispositivo, mas não estiver definido. (somente android). Os valores possíveis são: `block`, `wipe`, `warn`.|
|connectToVpnOnLaunch|Booliano|Se o aplicativo deve se conectar à VPN configurada na inicialização (somente Android).|
|appActionIfDevicePasscodeComplexityLessThanLow|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Se o dispositivo não tiver uma senha de baixa complexidade ou superior, dispare a ação armazenada. Os valores possíveis são: `block`, `wipe`, `warn`.|
|appActionIfDevicePasscodeComplexityLessThanMedium|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Se o dispositivo não tiver uma senha de complexidade média ou superior, dispare a ação armazenada. Os valores possíveis são: `block`, `wipe`, `warn`.|
|appActionIfDevicePasscodeComplexityLessThanHigh|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Se o dispositivo não tiver uma senha de alta complexidade ou superior, dispare a ação armazenada. Os valores possíveis são: `block`, `wipe`, `warn`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|apps|Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lista de aplicativos em que a política é implantada.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Propriedade de navegação para o resumo de implantação da configuração.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "maximumRequiredOsVersion": "String",
  "maximumWarningOsVersion": "String",
  "maximumWipeOsVersion": "String",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": 1024,
  "notificationRestriction": "String",
  "previousPinBlockCount": 1024,
  "managedBrowser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "blockDataIngestionIntoOrganizationDocuments": true,
  "allowedDataIngestionLocations": [
    "String"
  ],
  "appActionIfUnableToAuthenticateUser": "String",
  "dialerRestrictionLevel": "String",
  "gracePeriodToBlockAppsDuringOffClockHours": "String (duration)",
  "appDataEncryptionType": "String",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "String",
  "minimumWipePatchVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserProtocol": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String",
  "customDialerAppProtocol": "String",
  "customDialerAppPackageId": "String",
  "customDialerAppDisplayName": "String",
  "biometricAuthenticationBlocked": true,
  "requiredAndroidSafetyNetEvaluationType": "String",
  "blockAfterCompanyPortalUpdateDeferralInDays": 1024,
  "warnAfterCompanyPortalUpdateDeferralInDays": 1024,
  "wipeAfterCompanyPortalUpdateDeferralInDays": 1024,
  "deviceLockRequired": true,
  "appActionIfDeviceLockNotSet": "String",
  "connectToVpnOnLaunch": true,
  "appActionIfDevicePasscodeComplexityLessThanLow": "String",
  "appActionIfDevicePasscodeComplexityLessThanMedium": "String",
  "appActionIfDevicePasscodeComplexityLessThanHigh": "String"
}
```




