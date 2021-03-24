---
title: Obter depIOSEnrollmentProfile
description: Leia propriedades e relações do objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04ae56c0edf0823b121db9b76c707f8f76486682
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126245"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="3d5bb-103">Obter depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3d5bb-103">Get depIOSEnrollmentProfile</span></span>

<span data-ttu-id="3d5bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d5bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d5bb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d5bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d5bb-107">Leia propriedades e relações do [objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="3d5bb-107">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d5bb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d5bb-108">Prerequisites</span></span>
<span data-ttu-id="3d5bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d5bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d5bb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d5bb-111">Permission type</span></span>|<span data-ttu-id="3d5bb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d5bb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d5bb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d5bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d5bb-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5bb-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d5bb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d5bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d5bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-116">Not supported.</span></span>|
|<span data-ttu-id="3d5bb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d5bb-117">Application</span></span>|<span data-ttu-id="3d5bb-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5bb-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d5bb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d5bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d5bb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d5bb-120">Optional query parameters</span></span>
<span data-ttu-id="3d5bb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d5bb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d5bb-122">Request headers</span></span>
|<span data-ttu-id="3d5bb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d5bb-123">Header</span></span>|<span data-ttu-id="3d5bb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3d5bb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d5bb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d5bb-125">Authorization</span></span>|<span data-ttu-id="3d5bb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d5bb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d5bb-127">Accept</span></span>|<span data-ttu-id="3d5bb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3d5bb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d5bb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d5bb-129">Request body</span></span>
<span data-ttu-id="3d5bb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d5bb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d5bb-131">Response</span></span>
<span data-ttu-id="3d5bb-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um objeto depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-132">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d5bb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d5bb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d5bb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d5bb-134">Request</span></span>
<span data-ttu-id="3d5bb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="3d5bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d5bb-136">Response</span></span>
<span data-ttu-id="3d5bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d5bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2288

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
}
```




