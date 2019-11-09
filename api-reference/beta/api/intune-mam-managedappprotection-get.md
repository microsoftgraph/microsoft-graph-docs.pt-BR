---
title: Get managedAppProtection
description: Ler propriedades e relações do objeto managedAppProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 816e777ce8d7c722b97fd7425c915fad11a2e3dd
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086827"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="1c87a-103">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1c87a-103">Get managedAppProtection</span></span>

> <span data-ttu-id="1c87a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c87a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c87a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c87a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c87a-106">Ler propriedades e relações do objeto [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="1c87a-106">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c87a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c87a-107">Prerequisites</span></span>
<span data-ttu-id="1c87a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c87a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c87a-110">Permission type</span></span>|<span data-ttu-id="1c87a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c87a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c87a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c87a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c87a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c87a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1c87a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c87a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c87a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c87a-115">Not supported.</span></span>|
|<span data-ttu-id="1c87a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c87a-116">Application</span></span>|<span data-ttu-id="1c87a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c87a-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c87a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c87a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c87a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c87a-119">Optional query parameters</span></span>
<span data-ttu-id="1c87a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c87a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c87a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c87a-121">Request headers</span></span>
|<span data-ttu-id="1c87a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c87a-122">Header</span></span>|<span data-ttu-id="1c87a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1c87a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c87a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c87a-124">Authorization</span></span>|<span data-ttu-id="1c87a-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c87a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c87a-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c87a-126">Accept</span></span>|<span data-ttu-id="1c87a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1c87a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c87a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c87a-128">Request body</span></span>
<span data-ttu-id="1c87a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c87a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c87a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c87a-130">Response</span></span>
<span data-ttu-id="1c87a-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedAppProtection](../resources/intune-mam-managedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c87a-131">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c87a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c87a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c87a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c87a-133">Request</span></span>
<span data-ttu-id="1c87a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c87a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="1c87a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c87a-135">Response</span></span>
<span data-ttu-id="1c87a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c87a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2289

{
  "value": {
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
    "mobileThreatDefenseRemediationAction": "wipe"
  }
}
```






