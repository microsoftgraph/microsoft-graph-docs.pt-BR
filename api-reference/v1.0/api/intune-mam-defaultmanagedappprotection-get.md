---
title: Get defaultManagedAppProtection
description: Ler propriedades e relações do objeto defaultManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 988567af535fa672f9d99a5cab718d39a8703885
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363868"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="8ddcc-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="8ddcc-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="8ddcc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ddcc-105">Ler propriedades e relações do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="8ddcc-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ddcc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ddcc-106">Prerequisites</span></span>
<span data-ttu-id="8ddcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ddcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ddcc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ddcc-109">Permission type</span></span>|<span data-ttu-id="8ddcc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ddcc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ddcc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ddcc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ddcc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ddcc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8ddcc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ddcc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ddcc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-114">Not supported.</span></span>|
|<span data-ttu-id="8ddcc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ddcc-115">Application</span></span>|<span data-ttu-id="8ddcc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ddcc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ddcc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ddcc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ddcc-118">Optional query parameters</span></span>
<span data-ttu-id="8ddcc-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ddcc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ddcc-120">Request headers</span></span>
|<span data-ttu-id="8ddcc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ddcc-121">Header</span></span>|<span data-ttu-id="8ddcc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ddcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ddcc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ddcc-123">Authorization</span></span>|<span data-ttu-id="8ddcc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ddcc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ddcc-125">Accept</span></span>|<span data-ttu-id="8ddcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ddcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ddcc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ddcc-127">Request body</span></span>
<span data-ttu-id="8ddcc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ddcc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ddcc-129">Response</span></span>
<span data-ttu-id="8ddcc-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ddcc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ddcc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ddcc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ddcc-132">Request</span></span>
<span data-ttu-id="8ddcc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="8ddcc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ddcc-134">Response</span></span>
<span data-ttu-id="8ddcc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ddcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




