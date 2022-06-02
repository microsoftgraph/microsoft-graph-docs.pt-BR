---
title: Tipo de recurso windowsManagedAppProtection
description: Política usada para definir configurações de gerenciamento detalhadas direcionadas a grupos de segurança específicos e para um conjunto especificado de aplicativos em um Windows dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d3116545d5d9bf8480f8c35dcd7ed7703739304
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858476"
---
# <a name="windowsmanagedappprotection-resource-type"></a>Tipo de recurso windowsManagedAppProtection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política usada para definir configurações de gerenciamento detalhadas direcionadas a grupos de segurança específicos e para um conjunto especificado de aplicativos em um Windows dispositivo


Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsManagedAppProtections](../api/intune-mam-windowsmanagedappprotection-list.md)|[coleção windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Listar propriedades e relações dos [objetos windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Obter windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-get.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Ler propriedades e relações do [objeto windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Criar windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-create.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Crie um novo [objeto windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Excluir windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-delete.md)|Nenhum|Exclui um [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md).|
|[Atualizar windowsManagedAppProtection](../api/intune-mam-windowsmanagedappprotection-update.md)|[windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md)|Atualize as propriedades de um [objeto windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .|
|[Ação targetApps](../api/intune-mam-windowsmanagedappprotection-targetapps.md)|Nenhum|Ainda não documentado|
|[atribuir ação](../api/intune-mam-windowsmanagedappprotection-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|String|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|isAssigned|Boolean|Quando TRUE, indica que a política é implantada em alguns grupos de inclusão. Quando FALSE, indica que a política não é implantada em nenhum grupo de inclusão. O valor padrão é FALSE.|
|deployedAppCount|Int32|Indica o número total de aplicativos para os quais a política atual é implantada.|
|printBlocked|Boolean|Quando TRUE, indica que a impressão está bloqueada de aplicativos gerenciados. Quando FALSE, indica que a impressão é permitida de aplicativos gerenciados. O valor padrão é FALSE.|
|allowedInboundDataTransferSources|[windowsManagedAppDataTransferLevel](../resources/intune-mam-windowsmanagedappdatatransferlevel.md)|Indica as fontes das quais os dados podem ser transferidos. Alguns valores possíveis são allApps ou nenhum. Os valores possíveis são: `allApps` e `none`.|
|allowedOutboundClipboardSharingLevel|[windowsManagedAppClipboardSharingLevel](../resources/intune-mam-windowsmanagedappclipboardsharinglevel.md)|Indica o nível para o qual a área de transferência pode ser compartilhada entre & recursos não organizações. Alguns valores possíveis são anyDestinationAnySource ou nenhum. Os valores possíveis são: `anyDestinationAnySource` e `none`.|
|allowedOutboundDataTransferDestinations|[windowsManagedAppDataTransferLevel](../resources/intune-mam-windowsmanagedappdatatransferlevel.md)|Indica os destinos para os quais os dados podem ser transferidos. Alguns valores possíveis são allApps ou nenhum. Os valores possíveis são: `allApps` e `none`.|
|appActionIfUnableToAuthenticateUser|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Se definido, ele especificará qual ação executar no caso em que o usuário não puder fazer check-in porque o token de autenticação é inválido. Isso acontece quando o usuário é excluído ou desabilitado no AAD. Alguns valores possíveis são bloquear ou apagar. Se essa propriedade não estiver definida, nenhuma ação será executada. Os valores possíveis são: `block`, `wipe`, `warn`.|
|maximumAllowedDeviceThreatLevel|[managedAppDeviceThreatLevel](../resources/intune-mam-managedappdevicethreatlevel.md)|Nível máximo de ameaça de dispositivo permitido, conforme relatado pelo aplicativo de Defesa contra Ameaças Móveis. Os valores possíveis são: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Determina qual ação executar se o limite de ameaças de defesa contra ameaças móveis não for atendido. Alguns valores possíveis são bloquear ou apagar. Avisar não é um valor com suporte para essa propriedade. Os valores possíveis são: `block`, `wipe`, `warn`.|
|minimumRequiredSdkVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumWipeSdkVersion|String|Versões menores que a versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumRequiredOsVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumWarningOsVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumWipeOsVersion|String|Versões menores que a versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumRequiredAppVersion|String|Versões anteriores à versão especificada impedirão o aplicativo gerenciado de acessar dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumWarningAppVersion|String|Versões anteriores à versão especificada resultarão em uma mensagem de aviso no aplicativo gerenciado ao acessar dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|minimumWipeAppVersion|String|Versões menores que a versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Por exemplo: '8.1.0' ou '13.1.1'.|
|maximumRequiredOsVersion|String|Versões maiores que a versão especificada impedirão que o aplicativo gerenciado acesse os dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|maximumWarningOsVersion|String|Versões maiores que a versão especificada resultarão na mensagem de aviso no aplicativo gerenciado de acessar dados da empresa. Por exemplo: '8.1.0' ou '13.1.1'.|
|maximumWipeOsVersion|String|Versões maiores que a versão especificada apagarão o aplicativo gerenciado e os dados da empresa associados. Por exemplo: '8.1.0' ou '13.1.1'.|
|periodOfflineBeforeWipeIsEnforced|Duração|A quantidade de tempo que um aplicativo pode permanecer desconectado da Internet antes que todos os dados gerenciados sejam apagados. Por exemplo, P5D indica que o intervalo é de 5 dias de duração. Um valor de período de tempo de PT0S indica que os dados gerenciados nunca serão apagados quando o dispositivo não estiver conectado à Internet.|
|periodOfflineBeforeAccessCheck|Duração|Período após o qual o acesso é verificado quando o dispositivo não está conectado à Internet. Por exemplo, PT5M indica que o intervalo é de 5 minutos de duração. Um valor de período de tempo de PT0S indica que o acesso será bloqueado imediatamente quando o dispositivo não estiver conectado à Internet.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada.|
|Aplicativos|Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lista de aplicativos em que a política é implantada.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "isAssigned": true,
  "deployedAppCount": 1024,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundClipboardSharingLevel": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "appActionIfUnableToAuthenticateUser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "minimumRequiredSdkVersion": "String",
  "minimumWipeSdkVersion": "String",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeAppVersion": "String",
  "maximumRequiredOsVersion": "String",
  "maximumWarningOsVersion": "String",
  "maximumWipeOsVersion": "String",
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "periodOfflineBeforeAccessCheck": "String (duration)"
}
```




