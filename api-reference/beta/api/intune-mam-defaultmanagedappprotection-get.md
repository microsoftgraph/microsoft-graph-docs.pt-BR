---
title: Get defaultManagedAppProtection
description: Ler propriedades e relações do objeto defaultManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d7e8cd56a295fe3e0bf1024168ec823bddd4dec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145464"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="77d80-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="77d80-103">Get defaultManagedAppProtection</span></span>

<span data-ttu-id="77d80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77d80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77d80-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77d80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77d80-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77d80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77d80-107">Ler propriedades e relações do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="77d80-107">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77d80-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77d80-108">Prerequisites</span></span>
<span data-ttu-id="77d80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77d80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77d80-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77d80-111">Permission type</span></span>|<span data-ttu-id="77d80-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77d80-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77d80-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77d80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77d80-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d80-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77d80-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77d80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77d80-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77d80-116">Not supported.</span></span>|
|<span data-ttu-id="77d80-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77d80-117">Application</span></span>|<span data-ttu-id="77d80-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d80-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77d80-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77d80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77d80-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="77d80-120">Optional query parameters</span></span>
<span data-ttu-id="77d80-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="77d80-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77d80-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77d80-122">Request headers</span></span>
|<span data-ttu-id="77d80-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77d80-123">Header</span></span>|<span data-ttu-id="77d80-124">Valor</span><span class="sxs-lookup"><span data-stu-id="77d80-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77d80-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="77d80-125">Authorization</span></span>|<span data-ttu-id="77d80-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77d80-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77d80-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77d80-127">Accept</span></span>|<span data-ttu-id="77d80-128">application/json</span><span class="sxs-lookup"><span data-stu-id="77d80-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77d80-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77d80-129">Request body</span></span>
<span data-ttu-id="77d80-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77d80-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77d80-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="77d80-131">Response</span></span>
<span data-ttu-id="77d80-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77d80-132">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d80-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77d80-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="77d80-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77d80-134">Request</span></span>
<span data-ttu-id="77d80-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77d80-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="77d80-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="77d80-136">Response</span></span>
<span data-ttu-id="77d80-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77d80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5743

{
  "value": {
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
    "maximumRequiredOsVersion": "Maximum Required Os Version value",
    "maximumWarningOsVersion": "Maximum Warning Os Version value",
    "maximumWipeOsVersion": "Maximum Wipe Os Version value",
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
    "previousPinBlockCount": 5,
    "managedBrowser": "microsoftEdge",
    "maximumAllowedDeviceThreatLevel": "secured",
    "mobileThreatDefenseRemediationAction": "wipe",
    "blockDataIngestionIntoOrganizationDocuments": true,
    "allowedDataIngestionLocations": [
      "sharePoint"
    ],
    "appActionIfUnableToAuthenticateUser": "wipe",
    "dialerRestrictionLevel": "managedApps",
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
    "protectInboundDataFromUnknownSources": true,
    "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
    "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
    "requiredAndroidSafetyNetAppsVerificationType": "enabled",
    "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
    "customBrowserProtocol": "Custom Browser Protocol value",
    "customBrowserPackageId": "Custom Browser Package Id value",
    "customBrowserDisplayName": "Custom Browser Display Name value",
    "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
    "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
    "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
    "allowedAndroidDeviceModels": [
      "Allowed Android Device Models value"
    ],
    "appActionIfAndroidDeviceModelNotAllowed": "wipe",
    "customDialerAppProtocol": "Custom Dialer App Protocol value",
    "customDialerAppPackageId": "Custom Dialer App Package Id value",
    "customDialerAppDisplayName": "Custom Dialer App Display Name value",
    "biometricAuthenticationBlocked": true,
    "requiredAndroidSafetyNetEvaluationType": "hardwareBacked",
    "blockAfterCompanyPortalUpdateDeferralInDays": 11,
    "warnAfterCompanyPortalUpdateDeferralInDays": 10,
    "wipeAfterCompanyPortalUpdateDeferralInDays": 10,
    "deviceLockRequired": true,
    "appActionIfDeviceLockNotSet": "wipe"
  }
}
```




