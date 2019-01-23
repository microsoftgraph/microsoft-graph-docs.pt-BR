---
title: Lista depIOSEnrollmentProfiles
description: Lista as propriedades e os relacionamentos dos objetos depIOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 981806afcb24855cd9fb1a881a021c0e65cb983f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402311"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="36609-103">Lista depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="36609-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="36609-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="36609-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36609-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36609-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36609-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="36609-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36609-107">Lista as propriedades e os relacionamentos dos objetos [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="36609-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36609-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36609-108">Prerequisites</span></span>
<span data-ttu-id="36609-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="36609-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="36609-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36609-111">Permission type</span></span>|<span data-ttu-id="36609-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36609-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36609-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36609-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36609-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="36609-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="36609-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36609-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36609-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36609-116">Not supported.</span></span>|
|<span data-ttu-id="36609-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36609-117">Application</span></span>|<span data-ttu-id="36609-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36609-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36609-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36609-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="36609-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36609-120">Request headers</span></span>
|<span data-ttu-id="36609-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36609-121">Header</span></span>|<span data-ttu-id="36609-122">Valor</span><span class="sxs-lookup"><span data-stu-id="36609-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36609-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36609-123">Authorization</span></span>|<span data-ttu-id="36609-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36609-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36609-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36609-125">Accept</span></span>|<span data-ttu-id="36609-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36609-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36609-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36609-127">Request body</span></span>
<span data-ttu-id="36609-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36609-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36609-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="36609-129">Response</span></span>
<span data-ttu-id="36609-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36609-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36609-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36609-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="36609-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36609-132">Request</span></span>
<span data-ttu-id="36609-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36609-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="36609-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="36609-134">Response</span></span>
<span data-ttu-id="36609-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36609-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2006

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
      "screenTimeScreenDisabled": true,
      "simSetupScreenDisabled": true,
      "softwareUpdateScreenDisabled": true,
      "watchMigrationScreenDisabled": true
    }
  ]
}
```




