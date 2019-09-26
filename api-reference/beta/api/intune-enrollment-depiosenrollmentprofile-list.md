---
title: Listar depIOSEnrollmentProfiles
description: Listar Propriedades e relações dos objetos depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e16198783ac9fdb9ae9af83a48a9552fd7fc3a4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185487"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="3df60-103">Listar depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="3df60-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="3df60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3df60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3df60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3df60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3df60-106">Listar Propriedades e relações dos objetos [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3df60-106">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3df60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3df60-107">Prerequisites</span></span>
<span data-ttu-id="3df60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3df60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3df60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3df60-110">Permission type</span></span>|<span data-ttu-id="3df60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3df60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3df60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3df60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3df60-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3df60-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3df60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3df60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3df60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3df60-115">Not supported.</span></span>|
|<span data-ttu-id="3df60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3df60-116">Application</span></span>|<span data-ttu-id="3df60-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3df60-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3df60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3df60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3df60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3df60-119">Request headers</span></span>
|<span data-ttu-id="3df60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3df60-120">Header</span></span>|<span data-ttu-id="3df60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3df60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3df60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3df60-122">Authorization</span></span>|<span data-ttu-id="3df60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3df60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3df60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3df60-124">Accept</span></span>|<span data-ttu-id="3df60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3df60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3df60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3df60-126">Request body</span></span>
<span data-ttu-id="3df60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3df60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3df60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3df60-128">Response</span></span>
<span data-ttu-id="3df60-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3df60-129">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3df60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3df60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3df60-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3df60-131">Request</span></span>
<span data-ttu-id="3df60-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3df60-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="3df60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3df60-133">Response</span></span>
<span data-ttu-id="3df60-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3df60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
      "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
      "iTunesPairingMode": "allow",
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreFromAndroidDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true,
      "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
      "enableSingleAppEnrollmentMode": true,
      "homeButtonScreenDisabled": true,
      "iMessageAndFaceTimeScreenDisabled": true,
      "onBoardingScreenDisabled": true,
      "simSetupScreenDisabled": true,
      "softwareUpdateScreenDisabled": true,
      "watchMigrationScreenDisabled": true,
      "appearanceScreenDisabled": true,
      "expressLanguageScreenDisabled": true,
      "preferredLanguageScreenDisabled": true,
      "deviceToDeviceMigrationDisabled": true,
      "welcomeScreenDisabled": true
    }
  ]
}
```




