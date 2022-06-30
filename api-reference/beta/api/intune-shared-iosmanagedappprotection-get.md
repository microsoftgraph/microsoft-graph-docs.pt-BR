---
title: Obter iosManagedAppProtections
description: Ler propriedades e relações do objeto iosManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf0b4ee0a458a5afad2d1d1e7727f532549094ef
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446964"
---
# <a name="get-iosmanagedappprotection"></a>Obter iosManagedAppProtections

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ler propriedades e relações do objeto [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)||
| &nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo||
| &nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
| &nbsp;&nbsp; **Conjunto de Políticas** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2944

{
  "value": {
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
}
```






