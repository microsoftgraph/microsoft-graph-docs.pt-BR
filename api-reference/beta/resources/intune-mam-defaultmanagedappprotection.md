---
title: Tipo de recurso defaultManagedAppProtection
description: Política usada para definir configurações de gerenciamento detalhadas para um conjunto especificado de aplicativos para todos os usuários não direcionados por uma política TargetedManagedAppProtection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 796eec6a1caa595fcc3bceef5d3c454ef34eecdb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155822"
---
# <a name="defaultmanagedappprotection-resource-type"></a>Tipo de recurso defaultManagedAppProtection

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|displayName|String|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|descrição|String|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo está conectado à Internet. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Fontes das quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Destinos para os quais os dados podem ser transferidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Indica se as credenciais organizacionais são obrigatórias para o uso do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|O nível em que a área de transferência pode ser compartilhada entre os aplicativos no dispositivo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Indica se o backup de dados de um aplicativo gerenciado está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|deviceComplianceRequired|Boolean|Indica se a compatibilidade de dispositivos é necessária. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas de repetição de PIN incorretas antes de o aplicativo gerenciado ser bloqueado ou apagado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdad de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|coleção [managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeOsVersion|String|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWipeAppVersion|String|Versões menores ou iguais à versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueio ou apagamento, quando o dispositivo é enraizada ou desbloqueado, se DeviceComplianceRequired estiver definido como true. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueio ou apagamento, com base no número máximo de tentativas de repetição de PIN incorretas. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Tempo limite em minutos para um PIN de aplicativo em vez de uma senha não biométrica herdada de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Tipo de criptografia que deve ser usada para dados em um aplicativo gerenciado. (somente iOS). Os valores possíveis são: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Boolean|Indica se a captura de tela está bloqueada. (Somente Android)|
|encryptAppData|Boolean|Indica se os dados de aplicativos gerenciados devem ser criptografados. (Somente Android)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Booliano|Quando essa configuração estiver habilitada, a criptografia no nível do aplicativo será desabilitada se a criptografia no nível do dispositivo estiver habilitada. (Somente Android)|
|minimumRequiredSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. (somente iOS)|
|customSettings|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos usuários afetados, não alterados por esse serviço|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|minimumRequiredPatchVersion|String|Define o nível mais antigo de patch de segurança do Android necessário que um usuário pode ter para obter acesso seguro ao aplicativo. (Somente Android)|
|minimumWarningPatchVersion|Cadeia de caracteres|Define o nível mais antigo de patch de segurança do Android recomendado que um usuário pode ter para obter acesso seguro ao aplicativo. (Somente Android)|
|exemptedAppProtocols|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|os aplicativos iOS nesta lista serão isentos da política e poderão receber dados de aplicativos gerenciados. (somente iOS)|
|exemptedAppPackages|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Os pacotes de aplicativos Android nesta lista serão isentos da política e poderão receber dados de aplicativos gerenciados. (Somente Android)|
|faceIdBlocked|Boolean|Indica se será permitido o uso do FaceID em vez de um pin se PinRequired estiver definido como True. (somente iOS)|
|minimumWipeSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|minimumWipePatchVersion|String|O nível de patch de segurança do Android menor ou igual ao valor especificado limpará o aplicativo gerenciado e os dados da empresa associados. (Somente Android)|
|allowedIosDeviceModels|String|Lista separada por ponto-e-vírgula de modelos de dispositivo permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione. (somente iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, seja Block ou apagamento, se o modelo de dispositivo especificado não for permitido. (somente iOS). Os valores possíveis são: `block`, `wipe`, `warn`.|
|allowedAndroidDeviceManufacturers|String|Lista separada por ponto-e-vírgula dos fabricantes de dispositivos permitidos, como uma cadeia de caracteres, para que o aplicativo gerenciado funcione. (Somente Android)|
|appActionIfAndroidDeviceManufacturerNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Define um comportamento de aplicativo gerenciado, bloqueio ou apagamento, caso o fabricante do dispositivo especificado não seja permitido. (Android somente). Os valores possíveis são: `block`, `wipe`, `warn`.|
|thirdPartyKeyboardsBlocked|Boolean|Define se os teclados de terceiros são permitidos ao acessar um aplicativo gerenciado. (somente iOS)|
|filterOpenInToOnlyManagedApps|Boolean|Define se a operação de abertura é suportada do aplicativo gerenciado para os locais de compartilhamento de filesharing selecionados. Essa configuração aplica-se somente quando AllowedOutboundDataTransferDestinations é definida como ManagedApps e Propriedadesdisableprotectionofmanagedoutboundopenindata é definida como false. (somente iOS)|
|Propriedadesdisableprotectionofmanagedoutboundopenindata|Boolean|Desabilitar a proteção de dados transferidos para outros aplicativos por meio da opção abrir do IOS. Essa configuração só pode ser true quando AllowedOutboundDataTransferDestinations está definida como ManagedApps. (somente iOS)|
|protectInboundDataFromUnknownSources|Boolean|Proteger dados de entrada de fonte desconhecida. Essa configuração só poderá ser true quando AllowedInboundDataTransferSources estiver definido como myapps. (somente iOS)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Aplicativos|Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lista de aplicativos em que a política é implantada.|
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
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
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
  "protectInboundDataFromUnknownSources": true
}
```




