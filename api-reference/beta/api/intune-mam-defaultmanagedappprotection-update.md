---
title: Atualizar defaultManagedAppProtection
description: Atualizar as propriedades de um objeto defaultManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6e4cefd35aaa14e45fcbfc9ba2bb9991e3d68a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994850"
---
# <a name="update-defaultmanagedappprotection"></a>Atualizar defaultManagedAppProtection

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|descrição|String|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo está conectado à Internet. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Fontes das quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Destinos para os quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Booliano|Indica se as credenciais organizacionais são obrigatórias para o uso do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|O nível em que a área de transferência pode ser compartilhada entre os aplicativos no dispositivo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Booliano|Indica se o backup de dados de um aplicativo gerenciado está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|deviceComplianceRequired|Booliano|Indica se a compatibilidade de dispositivos é necessária. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Booliano|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Booliano|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Booliano|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas de repetição de PIN incorretas antes de o aplicativo gerenciado ser bloqueado ou apagado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|coleção [managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `oneDriveForBusiness`, `sharePoint`, `localStorage`.|
|contactSyncBlocked|Booliano|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Booliano|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Booliano|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Booliano|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|String|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|String|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueio ou apagamento, quando o dispositivo é enraizada ou desbloqueado, se DeviceComplianceRequired estiver definido como true. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueio ou apagamento, com base no número máximo de tentativas de repetição de PIN incorretas. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duração|Tempo limite em minutos para um PIN de aplicativo em vez de uma senha não biométrica herdada de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|Especifique o número de caracteres que podem ser recortados ou copiados de dados org e contas para qualquer aplicativo. Essa configuração substitui a restrição AllowedOutboundClipboardSharingLevel. O valor padrão de ' 0 ' significa que nenhuma exceção é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Especifique a restrição de notificação de aplicativo herdada de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allow`, `blockOrganizationalData`, `block`.|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Tipo de criptografia que deve ser usada para dados em um aplicativo gerenciado. (somente iOS). Os valores possíveis são: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Booliano|Indica se a captura de tela está bloqueada. (Somente Android)|
|encryptAppData|Boolean|Indica se os dados de aplicativos gerenciados devem ser criptografados. (Somente Android)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Booliano|Quando essa configuração estiver habilitada, a criptografia no nível do aplicativo será desabilitada se a criptografia no nível do dispositivo estiver habilitada. (Somente Android)|
|minimumRequiredSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. (somente iOS)|
|customSettings|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos usuários afetados, não alterados por esse serviço|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|minimumRequiredPatchVersion|String|Define o nível mais antigo de patch de segurança do Android necessário que um usuário pode ter para obter acesso seguro ao aplicativo. (Somente Android)|
|minimumWarningPatchVersion|String|Define o nível mais antigo de patch de segurança do Android recomendado que um usuário pode ter para obter acesso seguro ao aplicativo. (Somente Android)|
|exemptedAppProtocols|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|os aplicativos iOS nesta lista serão isentos da política e poderão receber dados de aplicativos gerenciados. (somente iOS)|
|exemptedAppPackages|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Os pacotes de aplicativos Android nesta lista serão isentos da política e poderão receber dados de aplicativos gerenciados. (Somente Android)|
|faceIdBlocked|Boolean|Indica se será permitido o uso do FaceID em vez de um pin se PinRequired estiver definido como True. (somente iOS)|
|minimumWipeSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|minimumWipePatchVersion|String|O nível de patch de segurança do Android menor ou igual ao valor especificado limpará o aplicativo gerenciado e os dados da empresa associados. (Somente Android)|
|allowedIosDeviceModels|String|Lista separada por ponto-e-vírgula de modelos de dispositivo permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione. (somente iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja Block ou apagamento, se o modelo de dispositivo especificado não for permitido. (somente iOS). Os valores possíveis são: `block`, `wipe`, `warn`.|
|allowedAndroidDeviceManufacturers|String|Lista separada por ponto-e-vírgula dos fabricantes de dispositivos permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione. (Somente Android)|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueio ou apagamento, caso o fabricante do dispositivo especificado não seja permitido. (Android somente). Os valores possíveis são: `block`, `wipe`, `warn`.|
|filterOpenInToOnlyManagedApps|Booliano|Define se a operação de abertura é suportada do aplicativo gerenciado para os locais de compartilhamento de filesharing selecionados. Essa configuração aplica-se somente quando AllowedOutboundDataTransferDestinations é definida como ManagedApps e Propriedadesdisableprotectionofmanagedoutboundopenindata é definida como false. (somente iOS)|
|Propriedadesdisableprotectionofmanagedoutboundopenindata|Booliano|Desabilitar a proteção de dados transferidos para outros aplicativos por meio da opção abrir do IOS. Essa configuração só pode ser true quando AllowedOutboundDataTransferDestinations está definida como ManagedApps. (somente iOS)|
|protectInboundDataFromUnknownSources|Booliano|Proteger dados de entrada de fonte desconhecida. Essa configuração só poderá ser true quando AllowedInboundDataTransferSources estiver definido como myapps. (somente iOS)|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Define o requisito de atestado de dispositivo do SafetyNet do Android para que um aplicativo gerenciado funcione. Os valores possíveis são: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, avisar ou bloquear, se o SafetyNet de atestado do Android especificado falhar. Os valores possíveis são: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Define o requisito de verificação de aplicativos do Android SafetyNet para que um aplicativo gerenciado funcione. Os valores possíveis são: `none` e `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, avisar ou bloquear, se a requirment de verificação de aplicativo Android não tiver êxito. Os valores possíveis são: `block`, `wipe`, `warn`.|
|customBrowserProtocol|String|Um protocolo de navegador personalizado para abrir o webLINK no iOS. (somente iOS)|
|customBrowserPackageId|String|Identificador exclusivo de um navegador personalizado para abrir o webLINK no Android. (Somente Android)|
|customBrowserDisplayName|String|Nome amigável do navegador personalizado preferencial para abrir o webLINK no Android. (Somente Android)|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
Content-type: application/json
Content-length: 3746

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
  "requiredAndroidSafetyNetAppsVerificationType": "enabled",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
  "customBrowserProtocol": "Custom Browser Protocol value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3918

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "allowedOutboundClipboardSharingExceptionLength": 14,
  "notificationRestriction": "blockOrganizationalData",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
  "requiredAndroidSafetyNetAppsVerificationType": "enabled",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
  "customBrowserProtocol": "Custom Browser Protocol value",
  "customBrowserPackageId": "Custom Browser Package Id value",
  "customBrowserDisplayName": "Custom Browser Display Name value"
}
```





