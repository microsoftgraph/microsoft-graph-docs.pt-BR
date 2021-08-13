---
title: Tipo de recurso iosManagedAppProtection
description: Política usada para definir configurações de gerenciamento detalhadas direcionadas a grupos de segurança específicos e para um conjunto especificado de aplicativos em um dispositivo iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 73bb94517550cc6be42256f44237ee8f213b1eb766671e8e2ffe23ffa91e57ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202277"
---
# <a name="iosmanagedappprotection-resource-type"></a>Tipo de recurso iosManagedAppProtection

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política usada para definir configurações de gerenciamento detalhadas direcionadas a grupos de segurança específicos e para um conjunto especificado de aplicativos em um dispositivo iOS


Herda de [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosManagedAppProtections](../api/intune-mam-iosmanagedappprotection-list.md)|Coleção [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Listar propriedades e relações dos objetos [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Obter iosManagedAppProtections](../api/intune-mam-iosmanagedappprotection-get.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Ler propriedades e relações do objeto [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Criar iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-create.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Cria um novo objeto [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Excluir iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-delete.md)|Nenhum|Excluir um [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Atualizar iosManagedAppProtection](../api/intune-mam-iosmanagedappprotection-update.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Atualizar as propriedades de um objeto [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
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
|managedBrowserToOpenLinksRequired|Boolean|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado ou em qualquer navegador personalizado especificado por CustomBrowserProtocol (para iOS) ou CustomBrowserPackageId/CustomBrowserDisplayName (para Android) herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|saveAsBlocked|Boolean|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinRequired|Boolean|Indica se é necessário um pin no nível do aplicativo. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|maximumPinRetries|Int32|Número máximo de tentativas de repetir pinos incorretos antes que o aplicativo gerenciado seja bloqueado ou apagado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|simplePinBlocked|Boolean|Indica se simplePin está bloqueado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|allowedDataStorageLocations|[Coleção managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|contactSyncBlocked|Boolean|Indica se os contatos podem ser sincronizados com o dispositivo do usuário. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|printBlocked|Boolean|Indica se a impressão a partir de aplicativos gerenciados é permitida. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|fingerprintBlocked|Boolean|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado. Herdado de [managedAppProtection](../resources/intune-mam-managedappprotection.md)|
|managedBrowser|[managedBrowserType](../resources/intune-mam-managedbrowsertype.md)|Indica em quais navegadores gerenciados os links da Internet devem ser abertos. Quando essa propriedade é configurada, ManagedBrowserToOpenLinksRequired deve ser true. Herdado [de managedAppProtection](../resources/intune-mam-managedappprotection.md). Os valores possíveis são: `notConfigured` e `microsoftEdge`.|
|isAssigned|Boolean|Indica se a política foi implantada a grupos de inclusão ou não. Herdado de [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Tipo de criptografia que deve ser usada para dados em um aplicativo gerenciado. Os valores possíveis são: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|minimumRequiredSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|deployedAppCount|Int32|Contagem de aplicativos em que a política atual é implantada.|
|faceIdBlocked|Boolean|Indica se será permitido o uso do FaceID em vez de um pin se PinRequired estiver definido como True.|
|customBrowserProtocol|Cadeia de caracteres|Um protocolo de navegador personalizado para abrir o weblink no iOS. Quando essa propriedade é configurada, ManagedBrowserToOpenLinksRequired deve ser true.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada. Herdado de [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)|
|aplicativos|Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lista de aplicativos em que a política é implantada.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Propriedade de navegação para o resumo de implantação da configuração.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
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
  "managedBrowser": "String",
  "isAssigned": true,
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true,
  "customBrowserProtocol": "String"
}
```




