---
title: Get defaultManagedAppProtection
description: Ler propriedades e relações do objeto defaultManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42f3ee4c76d6573a1f98515ad47d8a951c0d09be
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978854"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="e9c77-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="e9c77-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="e9c77-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9c77-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9c77-105">Ler propriedades e relações do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e9c77-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9c77-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9c77-106">Prerequisites</span></span>
<span data-ttu-id="e9c77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9c77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9c77-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9c77-109">Permission type</span></span>|<span data-ttu-id="e9c77-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9c77-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9c77-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9c77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9c77-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9c77-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e9c77-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9c77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9c77-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9c77-114">Not supported.</span></span>|
|<span data-ttu-id="e9c77-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9c77-115">Application</span></span>|<span data-ttu-id="e9c77-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9c77-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9c77-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9c77-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9c77-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9c77-118">Optional query parameters</span></span>
<span data-ttu-id="e9c77-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9c77-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9c77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9c77-120">Request headers</span></span>
|<span data-ttu-id="e9c77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9c77-121">Header</span></span>|<span data-ttu-id="e9c77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e9c77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9c77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9c77-123">Authorization</span></span>|<span data-ttu-id="e9c77-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9c77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9c77-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9c77-125">Accept</span></span>|<span data-ttu-id="e9c77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9c77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9c77-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9c77-127">Request body</span></span>
<span data-ttu-id="e9c77-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9c77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9c77-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9c77-129">Response</span></span>
<span data-ttu-id="e9c77-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9c77-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9c77-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9c77-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9c77-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9c77-132">Request</span></span>
<span data-ttu-id="e9c77-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9c77-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="e9c77-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9c77-134">Response</span></span>
<span data-ttu-id="e9c77-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9c77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "faceIdBlocked": true
  }
}
```



