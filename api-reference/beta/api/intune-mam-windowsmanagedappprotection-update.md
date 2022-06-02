---
title: Atualizar windowsManagedAppProtection
description: Atualize as propriedades de um objeto windowsManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ec1fbab7605a65a27139761fb8f14443186d4f3
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858513"
---
# <a name="update-windowsmanagedappprotection"></a>Atualizar windowsManagedAppProtection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagedAppProtections/{windowsManagedAppProtectionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|descrição|String|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
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



## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código `200 OK` de resposta e um objeto [windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagedAppProtections/{windowsManagedAppProtectionId}
Content-type: application/json
Content-length: 1453

{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "isAssigned": true,
  "deployedAppCount": 0,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "none",
  "allowedOutboundClipboardSharingLevel": "none",
  "allowedOutboundDataTransferDestinations": "none",
  "appActionIfUnableToAuthenticateUser": "wipe",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1625

{
  "@odata.type": "#microsoft.graph.windowsManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "c7894cd1-4cd1-c789-d14c-89c7d14c89c7",
  "version": "Version value",
  "isAssigned": true,
  "deployedAppCount": 0,
  "printBlocked": true,
  "allowedInboundDataTransferSources": "none",
  "allowedOutboundClipboardSharingLevel": "none",
  "allowedOutboundDataTransferDestinations": "none",
  "appActionIfUnableToAuthenticateUser": "wipe",
  "maximumAllowedDeviceThreatLevel": "secured",
  "mobileThreatDefenseRemediationAction": "wipe",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "maximumRequiredOsVersion": "Maximum Required Os Version value",
  "maximumWarningOsVersion": "Maximum Warning Os Version value",
  "maximumWipeOsVersion": "Maximum Wipe Os Version value",
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S"
}
```




