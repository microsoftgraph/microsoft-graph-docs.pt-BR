---
title: Listar iosManagedAppProtections
description: Listar propriedades e relações dos objetos iosManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ea34c971c6664930fb6131515f9670b585e088a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458375"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="06a83-103">Listar iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="06a83-103">List iosManagedAppProtections</span></span>

<span data-ttu-id="06a83-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06a83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06a83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06a83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06a83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06a83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06a83-107">Listar propriedades e relações dos objetos [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="06a83-107">List properties and relationships of the [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06a83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06a83-108">Prerequisites</span></span>
<span data-ttu-id="06a83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06a83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06a83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06a83-111">Permission type</span></span>|<span data-ttu-id="06a83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06a83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06a83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06a83-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="06a83-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="06a83-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="06a83-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a83-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="06a83-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="06a83-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="06a83-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a83-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="06a83-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06a83-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06a83-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06a83-119">Not supported.</span></span>|
|<span data-ttu-id="06a83-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a83-120">Application</span></span>||
| <span data-ttu-id="06a83-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="06a83-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="06a83-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a83-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="06a83-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="06a83-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="06a83-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a83-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06a83-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06a83-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="06a83-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06a83-126">Request headers</span></span>
|<span data-ttu-id="06a83-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06a83-127">Header</span></span>|<span data-ttu-id="06a83-128">Valor</span><span class="sxs-lookup"><span data-stu-id="06a83-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06a83-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="06a83-129">Authorization</span></span>|<span data-ttu-id="06a83-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06a83-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06a83-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06a83-131">Accept</span></span>|<span data-ttu-id="06a83-132">application/json</span><span class="sxs-lookup"><span data-stu-id="06a83-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06a83-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06a83-133">Request body</span></span>
<span data-ttu-id="06a83-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06a83-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06a83-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a83-135">Response</span></span>
<span data-ttu-id="06a83-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06a83-136">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a83-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06a83-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="06a83-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06a83-138">Request</span></span>
<span data-ttu-id="06a83-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06a83-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="06a83-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a83-140">Response</span></span>
<span data-ttu-id="06a83-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06a83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3088

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true,
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "wipe",
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true,
      "customBrowserProtocol": "Custom Browser Protocol value"
    }
  ]
}
```








