---
title: Criar iosManagedAppProtection
description: Cria um novo objeto iosManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 457badcc17f41c7ee568a684fc33084f5166c4b1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865499"
---
# <a name="create-iosmanagedappprotection"></a>Criar iosManagedAppProtection

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Cria um novo objeto [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)** | DeviceManagementApps.ReadWrite.All|
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application||
| &nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)** | DeviceManagementApps.ReadWrite.All|
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto iosManagedAppProtection.

A tabela a seguir mostra as propriedades que são necessárias ao criar iosManagedAppProtection.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
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
|managedBrowserToOpenLinksRequired|Boolean|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas de repetir pinos incorretos antes que o aplicativo gerenciado seja bloqueado ou apagado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[Coleção managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `oneDriveForBusiness`, `sharePoint`, `localStorage`.|
|contactSyncBlocked|Boolean|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|Cadeia de Caracteres|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|Cadeia de Caracteres|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja bloquear ou apagar, quando o dispositivo estiver enraizado ou com jailbroken, se DeviceComplianceRequired estiver definido como true. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueado ou apagado, com base no número máximo de tentativas de nova tentativa de pino incorretas. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Tempo de tempo em minutos para um pin de aplicativo em vez de senha não biométrica Herdada [de managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|Especifique o número de caracteres que podem ser cortados ou copiados de dados e contas de Org para qualquer aplicativo. Essa configuração substitui a restrição AllowedOutboundClipboardSharingLevel. O valor padrão de '0' significa que nenhuma exceção é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|notificationRestriction|[managedAppNotificationRestriction](../resources/intune-mam-managedappnotificationrestriction.md)|Especificar restrição de notificação de aplicativo Herdada [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allow`, `blockOrganizationalData`, `block`.|
|isAssigned|Boolean|Indica se a política foi implantada a grupos de inclusão ou não. Herdado de [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)|
|targetedAppManagementLevels|[appManagementLevel](../resources/intune-mam-appmanagementlevel.md)|Os níveis de gerenciamento de aplicativos pretendido para essa política Herdados de [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md). Os valores possíveis são: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Tipo de criptografia que deve ser usada para dados em um aplicativo gerenciado. Os valores possíveis são: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|minimumRequiredSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|faceIdBlocked|Boolean|Indica se será permitido o uso do FaceID em vez de um pin se PinRequired estiver definido como True.|
|exemptedAppProtocols|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Os aplicativos nesta lista estarão isentos da política e poderão receber dados de aplicativos gerenciados.|
|minimumWipeSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|allowedIosDeviceModels|Cadeia de Caracteres|Lista seperada de ponto e vírgula dos modelos de dispositivo permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione.|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloquear ou apagar, se o modelo de dispositivo especificado não for permitido. Os valores possíveis são: `block`, `wipe`, `warn`.|
|filterOpenInToOnlyManagedApps|Boolean|Define se a operação de abertura tem suporte do aplicativo gerenciado para os locais de compartilhamento de arquivos selecionados. Essa configuração só se aplica quando AllowedOutboundDataTransferDestinations é definida como ManagedApps e DisableProtectionOfManagedOutboundOpenInData é definida como False.|
|disableProtectionOfManagedOutboundOpenInData|Boolean|Desabilite a proteção de dados transferidos para outros aplicativos por meio da opção IOS OpenIn. Essa configuração só é permitida quando AllowedOutboundDataTransferDestinations é definida como ManagedApps.|
|protectInboundDataFromUnknownSources|Boolean|Proteja dados de entrada de origem desconhecida. Essa configuração só é permitida quando AllowedInboundDataTransferSources é definida como AllApps.|
|customBrowserProtocol|Cadeia de Caracteres|Um protocolo de navegador personalizado para abrir o weblink no iOS.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
Content-type: application/json
Content-length: 2623

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "customBrowserProtocol": "Custom Browser Protocol value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2795

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "unmanaged",
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "customBrowserProtocol": "Custom Browser Protocol value"
}
```







