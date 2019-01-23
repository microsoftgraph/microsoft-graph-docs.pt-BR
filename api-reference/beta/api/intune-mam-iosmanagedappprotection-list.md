---
title: Listar iosManagedAppProtections
description: Listar propriedades e relações dos objetos iosManagedAppProtection.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae174ff736d5e8cbbf320abeaf651ae5f34f1e5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404152"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="ead88-103">Listar iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="ead88-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="ead88-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ead88-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ead88-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ead88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ead88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ead88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ead88-107">Listar propriedades e relações dos objetos [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="ead88-107">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ead88-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ead88-108">Prerequisites</span></span>
<span data-ttu-id="ead88-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ead88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ead88-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ead88-111">Permission type</span></span>|<span data-ttu-id="ead88-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ead88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ead88-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ead88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ead88-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ead88-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ead88-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ead88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ead88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ead88-116">Not supported.</span></span>|
|<span data-ttu-id="ead88-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ead88-117">Application</span></span>|<span data-ttu-id="ead88-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ead88-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ead88-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ead88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="ead88-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ead88-120">Request headers</span></span>
|<span data-ttu-id="ead88-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ead88-121">Header</span></span>|<span data-ttu-id="ead88-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ead88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ead88-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ead88-123">Authorization</span></span>|<span data-ttu-id="ead88-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ead88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ead88-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ead88-125">Accept</span></span>|<span data-ttu-id="ead88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ead88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ead88-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ead88-127">Request body</span></span>
<span data-ttu-id="ead88-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ead88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ead88-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead88-129">Response</span></span>
<span data-ttu-id="ead88-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ead88-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ead88-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ead88-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ead88-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ead88-132">Request</span></span>
<span data-ttu-id="ead88-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ead88-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="ead88-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead88-134">Response</span></span>
<span data-ttu-id="ead88-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ead88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2944

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
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true
    }
  ]
}
```




