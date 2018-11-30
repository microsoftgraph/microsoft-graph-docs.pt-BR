---
title: Listar managedAppProtections
description: Listar propriedades e relações dos objetos managedAppProtection.
ms.openlocfilehash: b4aebb5f904969769d18f708e46f3a9cfdd60221
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041138"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="7d951-103">Listar managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="7d951-103">List managedAppProtections</span></span>

> <span data-ttu-id="7d951-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d951-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d951-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d951-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d951-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d951-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d951-107">Listar propriedades e relações dos objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="7d951-107">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d951-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d951-108">Prerequisites</span></span>
<span data-ttu-id="7d951-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d951-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d951-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d951-111">Permission type</span></span>|<span data-ttu-id="7d951-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d951-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d951-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d951-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d951-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d951-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7d951-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d951-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d951-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d951-116">Not supported.</span></span>|
|<span data-ttu-id="7d951-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d951-117">Application</span></span>|<span data-ttu-id="7d951-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d951-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d951-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d951-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7d951-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d951-120">Request headers</span></span>
|<span data-ttu-id="7d951-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d951-121">Header</span></span>|<span data-ttu-id="7d951-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7d951-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d951-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d951-123">Authorization</span></span>|<span data-ttu-id="7d951-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d951-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d951-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d951-125">Accept</span></span>|<span data-ttu-id="7d951-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d951-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d951-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d951-127">Request body</span></span>
<span data-ttu-id="7d951-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d951-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d951-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d951-129">Response</span></span>
<span data-ttu-id="7d951-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppProtection](../resources/intune-mam-managedappprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d951-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d951-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d951-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d951-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d951-132">Request</span></span>
<span data-ttu-id="7d951-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d951-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="7d951-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d951-134">Response</span></span>
<span data-ttu-id="7d951-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d951-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2020

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
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S"
    }
  ]
}
```





