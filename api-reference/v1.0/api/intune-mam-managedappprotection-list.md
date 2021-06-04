---
title: Listar managedAppProtections
description: Listar propriedades e relações dos objetos managedAppProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ff9173889078fe89fc2966906d391e65bbf2dc9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753516"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="2e175-103">Listar managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="2e175-103">List managedAppProtections</span></span>

<span data-ttu-id="2e175-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e175-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e175-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e175-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e175-106">Listar propriedades e relações dos objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="2e175-106">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e175-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e175-107">Prerequisites</span></span>
<span data-ttu-id="2e175-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e175-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e175-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e175-110">Permission type</span></span>|<span data-ttu-id="2e175-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e175-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e175-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e175-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e175-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e175-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e175-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e175-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e175-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e175-115">Not supported.</span></span>|
|<span data-ttu-id="2e175-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e175-116">Application</span></span>|<span data-ttu-id="2e175-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e175-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e175-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e175-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2e175-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e175-119">Request headers</span></span>
|<span data-ttu-id="2e175-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e175-120">Header</span></span>|<span data-ttu-id="2e175-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2e175-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e175-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e175-122">Authorization</span></span>|<span data-ttu-id="2e175-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e175-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e175-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e175-124">Accept</span></span>|<span data-ttu-id="2e175-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e175-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e175-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e175-126">Request body</span></span>
<span data-ttu-id="2e175-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e175-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e175-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e175-128">Response</span></span>
<span data-ttu-id="2e175-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e175-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e175-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e175-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e175-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e175-131">Request</span></span>
<span data-ttu-id="2e175-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e175-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="2e175-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e175-133">Response</span></span>
<span data-ttu-id="2e175-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e175-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1757

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "managedBrowser": "microsoftEdge"
    }
  ]
}
```




