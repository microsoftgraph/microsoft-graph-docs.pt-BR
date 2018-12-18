---
title: Obter targetedManagedAppProtection
description: Ler propriedades e relações do objeto targetedManagedAppProtection.
author: tfitzmac
ms.openlocfilehash: c8612f46f1a5672b4ca3dd2f1b1d90703a5b7aad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343908"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="72f59-103">Obter targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="72f59-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="72f59-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72f59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72f59-105">Ler propriedades e relações do objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="72f59-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72f59-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72f59-106">Prerequisites</span></span>
<span data-ttu-id="72f59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72f59-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72f59-109">Permission type</span></span>|<span data-ttu-id="72f59-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72f59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72f59-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72f59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72f59-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72f59-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72f59-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72f59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72f59-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72f59-114">Not supported.</span></span>|
|<span data-ttu-id="72f59-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72f59-115">Application</span></span>|<span data-ttu-id="72f59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72f59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72f59-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72f59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72f59-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72f59-118">Optional query parameters</span></span>
<span data-ttu-id="72f59-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72f59-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="72f59-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72f59-120">Request headers</span></span>
|<span data-ttu-id="72f59-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72f59-121">Header</span></span>|<span data-ttu-id="72f59-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72f59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72f59-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72f59-123">Authorization</span></span>|<span data-ttu-id="72f59-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72f59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72f59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72f59-125">Accept</span></span>|<span data-ttu-id="72f59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72f59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72f59-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72f59-127">Request body</span></span>
<span data-ttu-id="72f59-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72f59-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72f59-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f59-129">Response</span></span>
<span data-ttu-id="72f59-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72f59-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72f59-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72f59-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="72f59-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72f59-132">Request</span></span>
<span data-ttu-id="72f59-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72f59-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="72f59-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72f59-134">Response</span></span>
<span data-ttu-id="72f59-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72f59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

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
    "isAssigned": true
  }
}
```



