---
title: Lista depIOSEnrollmentProfiles
description: Lista as propriedades e os relacionamentos dos objetos depIOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5493628c79ebdc396df907ac3f2556e762cf6091
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919026"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="b36ea-103">Lista depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="b36ea-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="b36ea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b36ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b36ea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b36ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b36ea-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b36ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b36ea-107">Lista as propriedades e os relacionamentos dos objetos [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b36ea-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b36ea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b36ea-108">Prerequisites</span></span>
<span data-ttu-id="b36ea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b36ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b36ea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b36ea-111">Permission type</span></span>|<span data-ttu-id="b36ea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b36ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b36ea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b36ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b36ea-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b36ea-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b36ea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b36ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b36ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b36ea-116">Not supported.</span></span>|
|<span data-ttu-id="b36ea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b36ea-117">Application</span></span>|<span data-ttu-id="b36ea-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b36ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b36ea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b36ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="b36ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b36ea-120">Request headers</span></span>
|<span data-ttu-id="b36ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b36ea-121">Header</span></span>|<span data-ttu-id="b36ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b36ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b36ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b36ea-123">Authorization</span></span>|<span data-ttu-id="b36ea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b36ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b36ea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b36ea-125">Accept</span></span>|<span data-ttu-id="b36ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b36ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b36ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b36ea-127">Request body</span></span>
<span data-ttu-id="b36ea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b36ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b36ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b36ea-129">Response</span></span>
<span data-ttu-id="b36ea-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b36ea-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b36ea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b36ea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b36ea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b36ea-132">Request</span></span>
<span data-ttu-id="b36ea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b36ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="b36ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b36ea-134">Response</span></span>
<span data-ttu-id="b36ea-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b36ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1559

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
      "enableSingleAppEnrollmentMode": true
    }
  ]
}
```





