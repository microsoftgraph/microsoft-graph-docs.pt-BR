---
title: Obter targetedManagedAppProtection
description: Ler propriedades e relações do objeto targetedManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d82421329246e0702c1e288b34f9be4dfbd9fa6f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755669"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="a0220-103">Obter targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="a0220-103">Get targetedManagedAppProtection</span></span>

<span data-ttu-id="a0220-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0220-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0220-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0220-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0220-106">Ler propriedades e relações do objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="a0220-106">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0220-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0220-107">Prerequisites</span></span>
<span data-ttu-id="a0220-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0220-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0220-110">Permission type</span></span>|<span data-ttu-id="a0220-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0220-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0220-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0220-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0220-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0220-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0220-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0220-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0220-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0220-115">Not supported.</span></span>|
|<span data-ttu-id="a0220-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0220-116">Application</span></span>|<span data-ttu-id="a0220-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0220-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0220-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0220-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0220-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0220-119">Optional query parameters</span></span>
<span data-ttu-id="a0220-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0220-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0220-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0220-121">Request headers</span></span>
|<span data-ttu-id="a0220-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0220-122">Header</span></span>|<span data-ttu-id="a0220-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a0220-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0220-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0220-124">Authorization</span></span>|<span data-ttu-id="a0220-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0220-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0220-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0220-126">Accept</span></span>|<span data-ttu-id="a0220-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0220-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0220-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0220-128">Request body</span></span>
<span data-ttu-id="a0220-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0220-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0220-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0220-130">Response</span></span>
<span data-ttu-id="a0220-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0220-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0220-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0220-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0220-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0220-133">Request</span></span>
<span data-ttu-id="a0220-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0220-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="a0220-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0220-135">Response</span></span>
<span data-ttu-id="a0220-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0220-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




