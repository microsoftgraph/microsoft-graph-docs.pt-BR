---
title: Get defaultManagedAppProtection
description: Ler propriedades e relações do objeto defaultManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0fc53c09d7f9e922d107b7e140ac9c01ceff476d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396480"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="fd8bf-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fd8bf-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="fd8bf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd8bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd8bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd8bf-107">Ler propriedades e relações do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fd8bf-107">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd8bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd8bf-108">Prerequisites</span></span>
<span data-ttu-id="fd8bf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd8bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd8bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd8bf-111">Permission type</span></span>|<span data-ttu-id="fd8bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd8bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd8bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd8bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd8bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd8bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fd8bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd8bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd8bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-116">Not supported.</span></span>|
|<span data-ttu-id="fd8bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd8bf-117">Application</span></span>|<span data-ttu-id="fd8bf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd8bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd8bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd8bf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd8bf-120">Optional query parameters</span></span>
<span data-ttu-id="fd8bf-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd8bf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd8bf-122">Request headers</span></span>
|<span data-ttu-id="fd8bf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd8bf-123">Header</span></span>|<span data-ttu-id="fd8bf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fd8bf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd8bf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd8bf-125">Authorization</span></span>|<span data-ttu-id="fd8bf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd8bf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd8bf-127">Accept</span></span>|<span data-ttu-id="fd8bf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fd8bf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd8bf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd8bf-129">Request body</span></span>
<span data-ttu-id="fd8bf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd8bf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd8bf-131">Response</span></span>
<span data-ttu-id="fd8bf-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-132">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd8bf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd8bf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd8bf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd8bf-134">Request</span></span>
<span data-ttu-id="fd8bf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="fd8bf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd8bf-136">Response</span></span>
<span data-ttu-id="fd8bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd8bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3574

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
}
```




