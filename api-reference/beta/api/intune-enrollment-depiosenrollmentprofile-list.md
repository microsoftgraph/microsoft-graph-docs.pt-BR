---
title: Listar depIOSEnrollmentProfiles
description: Listar propriedades e relações dos objetos depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80d2638a6e51c56968e5bcbaab42a616fed33a58
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145954"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="41ab9-103">Listar depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="41ab9-103">List depIOSEnrollmentProfiles</span></span>

<span data-ttu-id="41ab9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41ab9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41ab9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41ab9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41ab9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41ab9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41ab9-107">Listar propriedades e relações dos [objetos depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="41ab9-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41ab9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41ab9-108">Prerequisites</span></span>
<span data-ttu-id="41ab9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41ab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41ab9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41ab9-111">Permission type</span></span>|<span data-ttu-id="41ab9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41ab9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41ab9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41ab9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41ab9-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ab9-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="41ab9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41ab9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41ab9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41ab9-116">Not supported.</span></span>|
|<span data-ttu-id="41ab9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41ab9-117">Application</span></span>|<span data-ttu-id="41ab9-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ab9-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41ab9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41ab9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="41ab9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41ab9-120">Request headers</span></span>
|<span data-ttu-id="41ab9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41ab9-121">Header</span></span>|<span data-ttu-id="41ab9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="41ab9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41ab9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41ab9-123">Authorization</span></span>|<span data-ttu-id="41ab9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41ab9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41ab9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41ab9-125">Accept</span></span>|<span data-ttu-id="41ab9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41ab9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41ab9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41ab9-127">Request body</span></span>
<span data-ttu-id="41ab9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41ab9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41ab9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="41ab9-129">Response</span></span>
<span data-ttu-id="41ab9-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41ab9-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41ab9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41ab9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="41ab9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41ab9-132">Request</span></span>
<span data-ttu-id="41ab9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41ab9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="41ab9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="41ab9-134">Response</span></span>
<span data-ttu-id="41ab9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41ab9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2414

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
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "displayToneSetupDisabled": true,
      "privacyPaneDisabled": true,
      "screenTimeScreenDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "configurationWebUrl": true,
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
      "welcomeScreenDisabled": true,
      "passCodeDisabled": true,
      "zoomDisabled": true,
      "restoreCompletedScreenDisabled": true,
      "updateCompleteScreenDisabled": true
    }
  ]
}
```




