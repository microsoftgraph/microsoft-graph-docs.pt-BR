---
title: Obter iosManagedAppProtections
description: Ler propriedades e relações do objeto iosManagedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c54d104bb7b49e94988eefd5279376379d2145ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079505"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="9789f-103">Obter iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="9789f-103">Get iosManagedAppProtection</span></span>

<span data-ttu-id="9789f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9789f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9789f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9789f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9789f-106">Ler propriedades e relações do objeto [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="9789f-106">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9789f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9789f-107">Prerequisites</span></span>
<span data-ttu-id="9789f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9789f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9789f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9789f-110">Permission type</span></span>|<span data-ttu-id="9789f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9789f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9789f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9789f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9789f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9789f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9789f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9789f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9789f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9789f-115">Not supported.</span></span>|
|<span data-ttu-id="9789f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9789f-116">Application</span></span>|<span data-ttu-id="9789f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9789f-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9789f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9789f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9789f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9789f-119">Optional query parameters</span></span>
<span data-ttu-id="9789f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9789f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9789f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9789f-121">Request headers</span></span>
|<span data-ttu-id="9789f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9789f-122">Header</span></span>|<span data-ttu-id="9789f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9789f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9789f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9789f-124">Authorization</span></span>|<span data-ttu-id="9789f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9789f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9789f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9789f-126">Accept</span></span>|<span data-ttu-id="9789f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9789f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9789f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9789f-128">Request body</span></span>
<span data-ttu-id="9789f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9789f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9789f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9789f-130">Response</span></span>
<span data-ttu-id="9789f-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9789f-131">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9789f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9789f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9789f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9789f-133">Request</span></span>
<span data-ttu-id="9789f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9789f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="9789f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9789f-135">Response</span></span>
<span data-ttu-id="9789f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9789f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1942

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "managedBrowser": "microsoftEdge",
    "isAssigned": true,
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true,
    "customBrowserProtocol": "Custom Browser Protocol value"
  }
}
```






