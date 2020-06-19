---
title: Listar targetedManagedAppProtections
description: Listar propriedades e relações dos objetos targetedManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c4e73fad4f577accd9bdfe8b86d0280f51d6f37
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791879"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="14905-103">Listar targetedManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="14905-103">List targetedManagedAppProtections</span></span>

<span data-ttu-id="14905-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14905-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14905-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14905-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14905-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14905-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14905-107">Listar propriedades e relações dos objetos [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="14905-107">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14905-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14905-108">Prerequisites</span></span>
<span data-ttu-id="14905-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="14905-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="14905-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14905-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14905-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14905-111">Permission type</span></span>|<span data-ttu-id="14905-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14905-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14905-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14905-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14905-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="14905-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="14905-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14905-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14905-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14905-116">Not supported.</span></span>|
|<span data-ttu-id="14905-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14905-117">Application</span></span>|<span data-ttu-id="14905-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="14905-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14905-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14905-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="14905-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14905-120">Request headers</span></span>
|<span data-ttu-id="14905-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14905-121">Header</span></span>|<span data-ttu-id="14905-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14905-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14905-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14905-123">Authorization</span></span>|<span data-ttu-id="14905-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14905-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14905-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14905-125">Accept</span></span>|<span data-ttu-id="14905-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14905-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14905-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14905-127">Request body</span></span>
<span data-ttu-id="14905-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14905-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14905-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="14905-129">Response</span></span>
<span data-ttu-id="14905-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14905-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14905-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14905-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14905-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14905-132">Request</span></span>
<span data-ttu-id="14905-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14905-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="14905-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14905-134">Response</span></span>
<span data-ttu-id="14905-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="14905-135">Here is an example of the response.</span></span> <span data-ttu-id="14905-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="14905-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14905-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="14905-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2723

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "b6b92266-2266-b6b9-6622-b9b66622b9b6",
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
      "previousPinBlockCount": 5,
      "managedBrowser": "microsoftEdge",
      "maximumAllowedDeviceThreatLevel": "secured",
      "mobileThreatDefenseRemediationAction": "wipe",
      "blockDataIngestionIntoOrganizationDocuments": true,
      "allowedDataIngestionLocations": [
        "sharePoint"
      ],
      "appActionIfUnableToAuthenticateUser": "wipe",
      "dialerRestrictionLevel": "managedApps",
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged"
    }
  ]
}
```



