---
title: Obter targetedManagedAppProtection
description: Ler propriedades e relações do objeto targetedManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 463077d3d47177162900b748528f05f08ea66f65
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177643"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="bbff4-103">Obter targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="bbff4-103">Get targetedManagedAppProtection</span></span>

<span data-ttu-id="bbff4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbff4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbff4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbff4-106">Ler propriedades e relações do objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="bbff4-106">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbff4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbff4-107">Prerequisites</span></span>
<span data-ttu-id="bbff4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbff4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbff4-110">Permission type</span></span>|<span data-ttu-id="bbff4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbff4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbff4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bbff4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbff4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bbff4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbff4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbff4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbff4-115">Not supported.</span></span>|
|<span data-ttu-id="bbff4-116">Application</span><span class="sxs-lookup"><span data-stu-id="bbff4-116">Application</span></span>|<span data-ttu-id="bbff4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbff4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbff4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbff4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbff4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bbff4-119">Optional query parameters</span></span>
<span data-ttu-id="bbff4-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bbff4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbff4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbff4-121">Request headers</span></span>
|<span data-ttu-id="bbff4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbff4-122">Header</span></span>|<span data-ttu-id="bbff4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bbff4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbff4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbff4-124">Authorization</span></span>|<span data-ttu-id="bbff4-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbff4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbff4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbff4-126">Accept</span></span>|<span data-ttu-id="bbff4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bbff4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbff4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbff4-128">Request body</span></span>
<span data-ttu-id="bbff4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbff4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbff4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbff4-130">Response</span></span>
<span data-ttu-id="bbff4-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbff4-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbff4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbff4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbff4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbff4-133">Request</span></span>
<span data-ttu-id="bbff4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbff4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="bbff4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbff4-135">Response</span></span>
<span data-ttu-id="bbff4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbff4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1704

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "managedBrowser": "microsoftEdge",
    "isAssigned": true
  }
}
```



