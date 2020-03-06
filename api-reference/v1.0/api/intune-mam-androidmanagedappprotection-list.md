---
title: Listar androidManagedAppProtections
description: Listar propriedades e relações dos objetos androidManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28af156fc6cce3c11b4d12f1e4050060cf85a2cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513326"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="e4413-103">Listar androidManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="e4413-103">List androidManagedAppProtections</span></span>

<span data-ttu-id="e4413-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4413-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4413-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4413-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4413-106">Listar propriedades e relações dos objetos [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="e4413-106">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4413-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4413-107">Prerequisites</span></span>
<span data-ttu-id="e4413-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4413-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4413-110">Permission type</span></span>|<span data-ttu-id="e4413-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4413-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4413-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4413-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4413-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4413-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e4413-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4413-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4413-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4413-115">Not supported.</span></span>|
|<span data-ttu-id="e4413-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4413-116">Application</span></span>|<span data-ttu-id="e4413-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4413-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4413-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4413-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="e4413-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4413-119">Request headers</span></span>
|<span data-ttu-id="e4413-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4413-120">Header</span></span>|<span data-ttu-id="e4413-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e4413-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4413-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4413-122">Authorization</span></span>|<span data-ttu-id="e4413-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4413-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4413-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4413-124">Accept</span></span>|<span data-ttu-id="e4413-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4413-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4413-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4413-126">Request body</span></span>
<span data-ttu-id="e4413-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4413-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4413-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4413-128">Response</span></span>
<span data-ttu-id="e4413-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4413-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4413-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4413-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4413-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4413-131">Request</span></span>
<span data-ttu-id="e4413-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4413-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="e4413-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4413-133">Response</span></span>
<span data-ttu-id="e4413-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4413-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "isAssigned": true,
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
    }
  ]
}
```




