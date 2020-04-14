---
title: Obter targetedManagedAppProtection
description: Ler propriedades e relações do objeto targetedManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e32081dfbf7fce6fa56879b4c37659bd53c291e1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386803"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="7ad3a-103">Obter targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7ad3a-103">Get targetedManagedAppProtection</span></span>

<span data-ttu-id="7ad3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ad3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ad3a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ad3a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ad3a-107">Ler propriedades e relações do objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7ad3a-107">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ad3a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ad3a-108">Prerequisites</span></span>
<span data-ttu-id="7ad3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ad3a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ad3a-111">Permission type</span></span>|<span data-ttu-id="7ad3a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ad3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ad3a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ad3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ad3a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ad3a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7ad3a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ad3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ad3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-116">Not supported.</span></span>|
|<span data-ttu-id="7ad3a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ad3a-117">Application</span></span>|<span data-ttu-id="7ad3a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ad3a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ad3a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ad3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ad3a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ad3a-120">Optional query parameters</span></span>
<span data-ttu-id="7ad3a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ad3a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ad3a-122">Request headers</span></span>
|<span data-ttu-id="7ad3a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ad3a-123">Header</span></span>|<span data-ttu-id="7ad3a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7ad3a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ad3a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ad3a-125">Authorization</span></span>|<span data-ttu-id="7ad3a-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ad3a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ad3a-127">Accept</span></span>|<span data-ttu-id="7ad3a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7ad3a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ad3a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ad3a-129">Request body</span></span>
<span data-ttu-id="7ad3a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ad3a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ad3a-131">Response</span></span>
<span data-ttu-id="7ad3a-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ad3a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ad3a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ad3a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ad3a-134">Request</span></span>
<span data-ttu-id="7ad3a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="7ad3a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ad3a-136">Response</span></span>
<span data-ttu-id="7ad3a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ad3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2549

{
  "value": {
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
}
```



