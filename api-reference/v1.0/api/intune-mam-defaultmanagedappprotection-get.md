---
title: Get defaultManagedAppProtection
description: Ler propriedades e relações do objeto defaultManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9f221dca8326ed9987491ca86e9136703872141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513277"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="464d3-103">Get defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="464d3-103">Get defaultManagedAppProtection</span></span>

<span data-ttu-id="464d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="464d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="464d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="464d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="464d3-106">Ler propriedades e relações do objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="464d3-106">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="464d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="464d3-107">Prerequisites</span></span>
<span data-ttu-id="464d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="464d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="464d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="464d3-110">Permission type</span></span>|<span data-ttu-id="464d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="464d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="464d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="464d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="464d3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="464d3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="464d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="464d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="464d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="464d3-115">Not supported.</span></span>|
|<span data-ttu-id="464d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="464d3-116">Application</span></span>|<span data-ttu-id="464d3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="464d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="464d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="464d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="464d3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="464d3-119">Optional query parameters</span></span>
<span data-ttu-id="464d3-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="464d3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="464d3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="464d3-121">Request headers</span></span>
|<span data-ttu-id="464d3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="464d3-122">Header</span></span>|<span data-ttu-id="464d3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="464d3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="464d3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="464d3-124">Authorization</span></span>|<span data-ttu-id="464d3-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="464d3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="464d3-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="464d3-126">Accept</span></span>|<span data-ttu-id="464d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="464d3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="464d3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="464d3-128">Request body</span></span>
<span data-ttu-id="464d3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="464d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="464d3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="464d3-130">Response</span></span>
<span data-ttu-id="464d3-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="464d3-131">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="464d3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="464d3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="464d3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="464d3-133">Request</span></span>
<span data-ttu-id="464d3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="464d3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="464d3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="464d3-135">Response</span></span>
<span data-ttu-id="464d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="464d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




