---
title: Listar defaultManagedAppProtections
description: Listar propriedades e relações dos objetos defaultManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0fdc1bb065d13abcf1d2c79ef8fb0a36bd71226
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260638"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="9e8b1-103">Listar defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="9e8b1-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="9e8b1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e8b1-105">Listar propriedades e relações dos objetos [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9e8b1-105">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e8b1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e8b1-106">Prerequisites</span></span>
<span data-ttu-id="9e8b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e8b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e8b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e8b1-109">Permission type</span></span>|<span data-ttu-id="9e8b1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e8b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e8b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e8b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e8b1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e8b1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9e8b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e8b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e8b1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-114">Not supported.</span></span>|
|<span data-ttu-id="9e8b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e8b1-115">Application</span></span>|<span data-ttu-id="9e8b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e8b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e8b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="9e8b1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e8b1-118">Request headers</span></span>
|<span data-ttu-id="9e8b1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e8b1-119">Header</span></span>|<span data-ttu-id="9e8b1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9e8b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e8b1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e8b1-121">Authorization</span></span>|<span data-ttu-id="9e8b1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e8b1-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e8b1-123">Accept</span></span>|<span data-ttu-id="9e8b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e8b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e8b1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e8b1-125">Request body</span></span>
<span data-ttu-id="9e8b1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e8b1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e8b1-127">Response</span></span>
<span data-ttu-id="9e8b1-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-128">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e8b1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e8b1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e8b1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e8b1-130">Request</span></span>
<span data-ttu-id="9e8b1-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="9e8b1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e8b1-132">Response</span></span>
<span data-ttu-id="9e8b1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e8b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2380

{
  "value": [
    {
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
  ]
}
```



