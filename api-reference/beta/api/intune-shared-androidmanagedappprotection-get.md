---
title: Get androidManagedAppProtection
description: Ler propriedades e relações do objeto androidManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0a2968bc14c90d5efd819370b261d971f6d8f13
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537153"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="7cbfd-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7cbfd-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="7cbfd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cbfd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cbfd-106">Ler propriedades e relações do objeto [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7cbfd-106">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cbfd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7cbfd-107">Prerequisites</span></span>
<span data-ttu-id="7cbfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cbfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cbfd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cbfd-110">Permission type</span></span>|<span data-ttu-id="7cbfd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7cbfd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cbfd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cbfd-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7cbfd-113">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="7cbfd-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7cbfd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cbfd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7cbfd-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="7cbfd-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7cbfd-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cbfd-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7cbfd-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cbfd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cbfd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-118">Not supported.</span></span>|
|<span data-ttu-id="7cbfd-119">Application</span><span class="sxs-lookup"><span data-stu-id="7cbfd-119">Application</span></span>||
| <span data-ttu-id="7cbfd-120">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="7cbfd-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7cbfd-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cbfd-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7cbfd-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="7cbfd-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7cbfd-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cbfd-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cbfd-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cbfd-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7cbfd-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7cbfd-125">Optional query parameters</span></span>
<span data-ttu-id="7cbfd-126">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cbfd-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cbfd-127">Request headers</span></span>
|<span data-ttu-id="7cbfd-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cbfd-128">Header</span></span>|<span data-ttu-id="7cbfd-129">Valor</span><span class="sxs-lookup"><span data-stu-id="7cbfd-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cbfd-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cbfd-130">Authorization</span></span>|<span data-ttu-id="7cbfd-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cbfd-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cbfd-132">Accept</span></span>|<span data-ttu-id="7cbfd-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7cbfd-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cbfd-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cbfd-134">Request body</span></span>
<span data-ttu-id="7cbfd-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cbfd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cbfd-136">Response</span></span>
<span data-ttu-id="7cbfd-137">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-137">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cbfd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cbfd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cbfd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cbfd-139">Request</span></span>
<span data-ttu-id="7cbfd-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="7cbfd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cbfd-141">Response</span></span>
<span data-ttu-id="7cbfd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cbfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3296

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
    "exemptedAppPackages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
    "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
    "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
    "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
    "requiredAndroidSafetyNetAppsVerificationType": "enabled",
    "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
    "customBrowserPackageId": "Custom Browser Package Id value",
    "customBrowserDisplayName": "Custom Browser Display Name value"
  }
}
```






