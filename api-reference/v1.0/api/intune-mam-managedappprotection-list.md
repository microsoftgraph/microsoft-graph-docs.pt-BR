---
title: Listar managedAppProtections
description: Listar propriedades e relações dos objetos managedAppProtection.
author: tfitzmac
ms.openlocfilehash: ed4ea950c603b8ed8ce6bf350595ca8616bb5343
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323202"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="c84f1-103">Listar managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="c84f1-103">List managedAppProtections</span></span>

> <span data-ttu-id="c84f1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c84f1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c84f1-105">Listar propriedades e relações dos objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="c84f1-105">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c84f1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c84f1-106">Prerequisites</span></span>
<span data-ttu-id="c84f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c84f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c84f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c84f1-109">Permission type</span></span>|<span data-ttu-id="c84f1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c84f1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c84f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c84f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c84f1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c84f1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c84f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c84f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c84f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c84f1-114">Not supported.</span></span>|
|<span data-ttu-id="c84f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c84f1-115">Application</span></span>|<span data-ttu-id="c84f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c84f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c84f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c84f1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c84f1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c84f1-118">Request headers</span></span>
|<span data-ttu-id="c84f1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c84f1-119">Header</span></span>|<span data-ttu-id="c84f1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c84f1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c84f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c84f1-121">Authorization</span></span>|<span data-ttu-id="c84f1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c84f1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c84f1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c84f1-123">Accept</span></span>|<span data-ttu-id="c84f1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c84f1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c84f1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c84f1-125">Request body</span></span>
<span data-ttu-id="c84f1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c84f1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c84f1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84f1-127">Response</span></span>
<span data-ttu-id="c84f1-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c84f1-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84f1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c84f1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c84f1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c84f1-130">Request</span></span>
<span data-ttu-id="c84f1-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c84f1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="c84f1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84f1-132">Response</span></span>
<span data-ttu-id="c84f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c84f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1715

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
      "minimumWarningAppVersion": "Minimum Warning App Version value"
    }
  ]
}
```



