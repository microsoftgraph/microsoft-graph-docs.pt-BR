---
title: Listar windowsManagedAppProtections
description: Listar propriedades e relações dos objetos windowsManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59f36fee770c87292795091f199396e2bd51655c
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858460"
---
# <a name="list-windowsmanagedappprotections"></a>Listar windowsManagedAppProtections

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos [objetos windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagedAppProtections
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos windowsManagedAppProtection](../resources/intune-mam-windowsmanagedappprotection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagedAppProtections
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1786

{
  "value": [
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
  ]
}
```




