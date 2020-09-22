---
title: Listar depMacOSEnrollmentProfiles
description: Listar Propriedades e relações dos objetos depMacOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69fb01d11340aa1d2029e8afb179d838124b6888
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093816"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="80149-103">Listar depMacOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="80149-103">List depMacOSEnrollmentProfiles</span></span>

<span data-ttu-id="80149-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80149-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80149-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80149-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80149-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80149-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80149-107">Listar Propriedades e relações dos objetos [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="80149-107">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80149-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80149-108">Prerequisites</span></span>
<span data-ttu-id="80149-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80149-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80149-111">Permission type</span></span>|<span data-ttu-id="80149-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80149-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80149-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80149-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80149-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="80149-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="80149-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80149-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80149-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80149-116">Not supported.</span></span>|
|<span data-ttu-id="80149-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80149-117">Application</span></span>|<span data-ttu-id="80149-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="80149-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80149-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80149-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="80149-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80149-120">Request headers</span></span>
|<span data-ttu-id="80149-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80149-121">Header</span></span>|<span data-ttu-id="80149-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80149-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80149-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80149-123">Authorization</span></span>|<span data-ttu-id="80149-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80149-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80149-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80149-125">Accept</span></span>|<span data-ttu-id="80149-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80149-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80149-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80149-127">Request body</span></span>
<span data-ttu-id="80149-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80149-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80149-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="80149-129">Response</span></span>
<span data-ttu-id="80149-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80149-130">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80149-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80149-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="80149-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80149-132">Request</span></span>
<span data-ttu-id="80149-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80149-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="80149-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="80149-134">Response</span></span>
<span data-ttu-id="80149-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80149-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1478

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "displayToneSetupDisabled": true,
      "privacyPaneDisabled": true,
      "screenTimeScreenDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "configurationWebUrl": true,
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true,
      "iCloudStorageDisabled": true,
      "chooseYourLockScreenDisabled": true
    }
  ]
}
```






