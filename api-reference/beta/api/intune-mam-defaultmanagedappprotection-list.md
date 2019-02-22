---
title: Listar defaultManagedAppProtections
description: Listar propriedades e relações dos objetos defaultManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8436ffc33effbfa932b1846b837bd9256e0a018
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165433"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="8b3d1-103">Listar defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="8b3d1-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="8b3d1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b3d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b3d1-106">Listar propriedades e relações dos objetos [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8b3d1-106">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b3d1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b3d1-107">Prerequisites</span></span>
<span data-ttu-id="8b3d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8b3d1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b3d1-110">Permission type</span></span>|<span data-ttu-id="8b3d1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8b3d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b3d1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b3d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b3d1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b3d1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8b3d1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b3d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b3d1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-115">Not supported.</span></span>|
|<span data-ttu-id="8b3d1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b3d1-116">Application</span></span>|<span data-ttu-id="8b3d1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b3d1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b3d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="8b3d1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b3d1-119">Request headers</span></span>
|<span data-ttu-id="8b3d1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b3d1-120">Header</span></span>|<span data-ttu-id="8b3d1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8b3d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b3d1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b3d1-122">Authorization</span></span>|<span data-ttu-id="8b3d1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b3d1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b3d1-124">Accept</span></span>|<span data-ttu-id="8b3d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b3d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b3d1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b3d1-126">Request body</span></span>
<span data-ttu-id="8b3d1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b3d1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b3d1-128">Response</span></span>
<span data-ttu-id="8b3d1-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-129">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b3d1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b3d1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b3d1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b3d1-131">Request</span></span>
<span data-ttu-id="8b3d1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="8b3d1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b3d1-133">Response</span></span>
<span data-ttu-id="8b3d1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b3d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3754

{
  "value": [
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
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true
    }
  ]
}
```




