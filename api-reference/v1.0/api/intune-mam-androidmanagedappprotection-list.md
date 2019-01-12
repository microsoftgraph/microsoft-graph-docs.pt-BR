---
title: Listar androidManagedAppProtections
description: Listar propriedades e relações dos objetos androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2faee995d847ed2b3a3aa11e8a08c0d96436736c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951891"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="10aaa-103">Listar androidManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="10aaa-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="10aaa-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="10aaa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10aaa-105">Listar propriedades e relações dos objetos [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="10aaa-105">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10aaa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10aaa-106">Prerequisites</span></span>
<span data-ttu-id="10aaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10aaa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10aaa-109">Permission type</span></span>|<span data-ttu-id="10aaa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10aaa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10aaa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10aaa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10aaa-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10aaa-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10aaa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10aaa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10aaa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10aaa-114">Not supported.</span></span>|
|<span data-ttu-id="10aaa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10aaa-115">Application</span></span>|<span data-ttu-id="10aaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10aaa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10aaa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10aaa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="10aaa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10aaa-118">Request headers</span></span>
|<span data-ttu-id="10aaa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10aaa-119">Header</span></span>|<span data-ttu-id="10aaa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="10aaa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10aaa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="10aaa-121">Authorization</span></span>|<span data-ttu-id="10aaa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10aaa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10aaa-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10aaa-123">Accept</span></span>|<span data-ttu-id="10aaa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="10aaa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10aaa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10aaa-125">Request body</span></span>
<span data-ttu-id="10aaa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10aaa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10aaa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="10aaa-127">Response</span></span>
<span data-ttu-id="10aaa-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10aaa-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10aaa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10aaa-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="10aaa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10aaa-130">Request</span></span>
<span data-ttu-id="10aaa-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10aaa-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="10aaa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="10aaa-132">Response</span></span>
<span data-ttu-id="10aaa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10aaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



