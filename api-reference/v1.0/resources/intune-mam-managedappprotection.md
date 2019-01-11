---
title: Tipo de recurso managedAppProtection
description: Política usada para definir configurações de gerenciamento detalhadas para um conjunto específico de aplicativos
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb5c6f6a158a79bdc9bd19094b79ef7510db1f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861814"
---
# <a name="managedappprotection-resource-type"></a>Tipo de recurso managedAppProtection

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política usada para definir configurações de gerenciamento detalhadas para um conjunto específico de aplicativos

Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppProtections](../api/intune-mam-managedappprotection-list.md)|Coleção [managedAppProtection](../resources/intune-mam-managedappprotection.md)|Listar propriedades e relações dos objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|[Obter managedAppProtection](../api/intune-mam-managedappprotection-get.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md)|Ler propriedades e relações do objeto [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|[Ação targetApps](../api/intune-mam-managedappprotection-targetapps.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet.|
|periodOnlineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo está conectado à Internet.|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Fontes dos quais os dados podem ser transferidos. Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Destinos para os quais os dados podem ser transferidos. Os valores possíveis são: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Booliano|Indica se as credenciais organizacionais são obrigatórias para o uso do aplicativo.|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|O nível em que a área de transferência pode ser compartilhada entre os aplicativos no dispositivo gerenciado. Os valores possíveis são: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Booliano|Indica se o backup de dados de um aplicativo gerenciado está bloqueado.|
|deviceComplianceRequired|Booliano|Indica se a compatibilidade de dispositivos é necessária.|
|managedBrowserToOpenLinksRequired|Booliano|Indica se os links da Internet devem ser abertos no aplicativo de navegador gerenciado.|
|saveAsBlocked|Booliano|Indica se os usuários podem usar o item de menu "Salvar como" para salvar uma cópia dos arquivos protegidos.|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados.|
|pinRequired|Booliano|Indica se é necessário um pin no nível do aplicativo.|
|maximumPinRetries|Int32|Número máximo de repetição de pin incorreto tentativas antes do aplicativo gerenciado é bloqueado ou apagado.|
|simplePinBlocked|Booliano|Indica se simplePin está bloqueado.|
|minimumPinLength|Int32|Tamanho mínimo de pin necessário para um pin no nível do aplicativo se PinRequired estiver definido como True|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Conjunto de caracteres que poderá ser usado para um pin no nível do aplicativo se PinRequired estiver definido como True. Os valores possíveis são: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duração|TimePeriod antes que o pin em todos os níveis tenha que ser redefinido, caso PinRequired esteja definido como True.|
|allowedDataStorageLocations|coleção [managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)|Locais de armazenamento de dados em que um usuário pode armazenar dados gerenciados.|
|contactSyncBlocked|Booliano|Indica se os contatos podem ser sincronizados com o dispositivo do usuário.|
|printBlocked|Booliano|Indica se a impressão a partir de aplicativos gerenciados é permitida.|
|fingerprintBlocked|Booliano|Indica se será permitido o uso do leitor de impressão digital em vez de um pin se PinRequired estiver definido como True.|
|disableAppPinIfDevicePinIsSet|Booliano|Indica se o uso do pin do aplicativo será obrigatório se o pin do dispositivo estiver definido.|
|minimumRequiredOsVersion|Cadeia de caracteres|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|minimumWarningOsVersion|Cadeia de caracteres|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado.|
|minimumRequiredAppVersion|Cadeia de caracteres|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa.|
|minimumWarningAppVersion|Cadeia de caracteres|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
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
  "minimumWarningAppVersion": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


