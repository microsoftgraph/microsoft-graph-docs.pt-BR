---
title: Listar targetedManagedAppProtections
description: Listar propriedades e relações dos objetos targetedManagedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 261d792b7cc268188a7cb8a9e579d779b4065907
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159910"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="7134c-103">Listar targetedManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="7134c-103">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="7134c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7134c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7134c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7134c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7134c-106">Listar propriedades e relações dos objetos [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7134c-106">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7134c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7134c-107">Prerequisites</span></span>
<span data-ttu-id="7134c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7134c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7134c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7134c-110">Permission type</span></span>|<span data-ttu-id="7134c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7134c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7134c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7134c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7134c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7134c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7134c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7134c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7134c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7134c-115">Not supported.</span></span>|
|<span data-ttu-id="7134c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7134c-116">Application</span></span>|<span data-ttu-id="7134c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7134c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7134c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7134c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7134c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7134c-119">Request headers</span></span>
|<span data-ttu-id="7134c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7134c-120">Header</span></span>|<span data-ttu-id="7134c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7134c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7134c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7134c-122">Authorization</span></span>|<span data-ttu-id="7134c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7134c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7134c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7134c-124">Accept</span></span>|<span data-ttu-id="7134c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7134c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7134c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7134c-126">Request body</span></span>
<span data-ttu-id="7134c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7134c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7134c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7134c-128">Response</span></span>
<span data-ttu-id="7134c-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7134c-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7134c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7134c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7134c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7134c-131">Request</span></span>
<span data-ttu-id="7134c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7134c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="7134c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7134c-133">Response</span></span>
<span data-ttu-id="7134c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7134c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2675

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
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged"
    }
  ]
}
```





