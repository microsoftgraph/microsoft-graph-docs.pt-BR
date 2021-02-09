---
title: Listar managedAppProtections
description: Listar propriedades e relações dos objetos managedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63689e0a0e48273df2d30a81a69298142df5305f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157922"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="4c55c-103">Listar managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="4c55c-103">List managedAppProtections</span></span>

<span data-ttu-id="4c55c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c55c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c55c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c55c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c55c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c55c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c55c-107">Listar propriedades e relações dos objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="4c55c-107">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c55c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c55c-108">Prerequisites</span></span>
<span data-ttu-id="4c55c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c55c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c55c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c55c-111">Permission type</span></span>|<span data-ttu-id="4c55c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c55c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c55c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c55c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c55c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c55c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4c55c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c55c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c55c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c55c-116">Not supported.</span></span>|
|<span data-ttu-id="4c55c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c55c-117">Application</span></span>|<span data-ttu-id="4c55c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c55c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c55c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c55c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="4c55c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c55c-120">Request headers</span></span>
|<span data-ttu-id="4c55c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c55c-121">Header</span></span>|<span data-ttu-id="4c55c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c55c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c55c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c55c-123">Authorization</span></span>|<span data-ttu-id="4c55c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c55c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c55c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c55c-125">Accept</span></span>|<span data-ttu-id="4c55c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c55c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c55c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c55c-127">Request body</span></span>
<span data-ttu-id="4c55c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c55c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c55c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c55c-129">Response</span></span>
<span data-ttu-id="4c55c-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c55c-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c55c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c55c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c55c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c55c-132">Request</span></span>
<span data-ttu-id="4c55c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c55c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="4c55c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c55c-134">Response</span></span>
<span data-ttu-id="4c55c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c55c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2843

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
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
      "maximumRequiredOsVersion": "Maximum Required Os Version value",
      "maximumWarningOsVersion": "Maximum Warning Os Version value",
      "maximumWipeOsVersion": "Maximum Wipe Os Version value",
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
      "dialerRestrictionLevel": "managedApps"
    }
  ]
}
```




