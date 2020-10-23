---
title: Obter iosManagedAppProtections
description: Ler propriedades e relações do objeto iosManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd44f8d1ebc6d7e662e52034ec6b8d39bb4d7938
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724077"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="7b974-103">Obter iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="7b974-103">Get iosManagedAppProtection</span></span>

<span data-ttu-id="7b974-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b974-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b974-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b974-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b974-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b974-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b974-107">Ler propriedades e relações do objeto [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7b974-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b974-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b974-108">Prerequisites</span></span>
<span data-ttu-id="7b974-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b974-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b974-111">Permission type</span></span>|<span data-ttu-id="7b974-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b974-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b974-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b974-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7b974-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="7b974-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7b974-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b974-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7b974-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="7b974-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7b974-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b974-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7b974-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b974-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b974-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b974-119">Not supported.</span></span>|
|<span data-ttu-id="7b974-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b974-120">Application</span></span>||
| <span data-ttu-id="7b974-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="7b974-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7b974-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b974-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7b974-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="7b974-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7b974-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b974-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b974-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b974-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b974-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b974-126">Optional query parameters</span></span>
<span data-ttu-id="7b974-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b974-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b974-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b974-128">Request headers</span></span>
|<span data-ttu-id="7b974-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b974-129">Header</span></span>|<span data-ttu-id="7b974-130">Valor</span><span class="sxs-lookup"><span data-stu-id="7b974-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b974-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b974-131">Authorization</span></span>|<span data-ttu-id="7b974-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b974-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b974-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b974-133">Accept</span></span>|<span data-ttu-id="7b974-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7b974-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b974-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b974-135">Request body</span></span>
<span data-ttu-id="7b974-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b974-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b974-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b974-137">Response</span></span>
<span data-ttu-id="7b974-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b974-138">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b974-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b974-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b974-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b974-140">Request</span></span>
<span data-ttu-id="7b974-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b974-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="7b974-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b974-142">Response</span></span>
<span data-ttu-id="7b974-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b974-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2944

{
  "value": {
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
}
```








