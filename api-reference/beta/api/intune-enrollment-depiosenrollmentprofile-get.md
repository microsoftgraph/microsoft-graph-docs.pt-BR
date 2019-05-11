---
title: Obter depIOSEnrollmentProfile
description: Leia as propriedades e as relações do objeto depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d736230ca89e1e127eee8f008f51c9b185f54
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908837"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="5ca13-103">Obter depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5ca13-103">Get depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="5ca13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ca13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ca13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ca13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ca13-106">Leia as propriedades e as relações do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5ca13-106">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ca13-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ca13-107">Prerequisites</span></span>
<span data-ttu-id="5ca13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca13-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ca13-110">Permission type</span></span>|<span data-ttu-id="5ca13-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ca13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ca13-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ca13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ca13-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca13-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5ca13-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ca13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ca13-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ca13-115">Not supported.</span></span>|
|<span data-ttu-id="5ca13-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ca13-116">Application</span></span>|<span data-ttu-id="5ca13-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ca13-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ca13-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ca13-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ca13-119">Optional query parameters</span></span>
<span data-ttu-id="5ca13-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca13-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ca13-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca13-121">Request headers</span></span>
|<span data-ttu-id="5ca13-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ca13-122">Header</span></span>|<span data-ttu-id="5ca13-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5ca13-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ca13-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca13-124">Authorization</span></span>|<span data-ttu-id="5ca13-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca13-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ca13-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ca13-126">Accept</span></span>|<span data-ttu-id="5ca13-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5ca13-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ca13-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca13-128">Request body</span></span>
<span data-ttu-id="5ca13-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ca13-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca13-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca13-130">Response</span></span>
<span data-ttu-id="5ca13-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca13-131">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca13-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca13-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ca13-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca13-133">Request</span></span>
<span data-ttu-id="5ca13-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca13-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="5ca13-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca13-135">Response</span></span>
<span data-ttu-id="5ca13-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ca13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1955

{
  "value": {
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
    "screenTimeScreenDisabled": true,
    "simSetupScreenDisabled": true,
    "softwareUpdateScreenDisabled": true,
    "watchMigrationScreenDisabled": true
  }
}
```




