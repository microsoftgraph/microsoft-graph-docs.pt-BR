---
title: Get androidManagedAppProtection
description: Ler propriedades e relações do objeto androidManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f03fef824797898761c1b162a05b37cdf166c78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400092"
---
# <a name="get-androidmanagedappprotection"></a><span data-ttu-id="a1ac2-103">Get androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="a1ac2-103">Get androidManagedAppProtection</span></span>

> <span data-ttu-id="a1ac2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1ac2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1ac2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1ac2-107">Ler propriedades e relações do objeto [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a1ac2-107">Read properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1ac2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1ac2-108">Prerequisites</span></span>
<span data-ttu-id="a1ac2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1ac2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1ac2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1ac2-111">Permission type</span></span>|<span data-ttu-id="a1ac2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1ac2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1ac2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1ac2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1ac2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1ac2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1ac2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1ac2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1ac2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-116">Not supported.</span></span>|
|<span data-ttu-id="a1ac2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1ac2-117">Application</span></span>|<span data-ttu-id="a1ac2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1ac2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1ac2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1ac2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1ac2-120">Optional query parameters</span></span>
<span data-ttu-id="a1ac2-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1ac2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ac2-122">Request headers</span></span>
|<span data-ttu-id="a1ac2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1ac2-123">Header</span></span>|<span data-ttu-id="a1ac2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a1ac2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1ac2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1ac2-125">Authorization</span></span>|<span data-ttu-id="a1ac2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1ac2-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1ac2-127">Accept</span></span>|<span data-ttu-id="a1ac2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a1ac2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1ac2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ac2-129">Request body</span></span>
<span data-ttu-id="a1ac2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1ac2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1ac2-131">Response</span></span>
<span data-ttu-id="a1ac2-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-132">If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1ac2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1ac2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1ac2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ac2-134">Request</span></span>
<span data-ttu-id="a1ac2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="a1ac2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1ac2-136">Response</span></span>
<span data-ttu-id="a1ac2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2773

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
    "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
  }
}
```




