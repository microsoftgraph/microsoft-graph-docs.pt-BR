---
title: Obter depIOSEnrollmentProfile
description: Leia as propriedades e as relações do objeto depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1213e976ddd4e93aefaa0b1c539da1597829d07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467225"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="d70b3-103">Obter depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d70b3-103">Get depIOSEnrollmentProfile</span></span>

<span data-ttu-id="d70b3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d70b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d70b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d70b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d70b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70b3-107">Leia as propriedades e as relações do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d70b3-107">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d70b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d70b3-108">Prerequisites</span></span>
<span data-ttu-id="d70b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d70b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d70b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d70b3-111">Permission type</span></span>|<span data-ttu-id="d70b3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d70b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d70b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d70b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d70b3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d70b3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d70b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d70b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d70b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d70b3-116">Not supported.</span></span>|
|<span data-ttu-id="d70b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d70b3-117">Application</span></span>|<span data-ttu-id="d70b3-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d70b3-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d70b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d70b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d70b3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d70b3-120">Optional query parameters</span></span>
<span data-ttu-id="d70b3-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d70b3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d70b3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d70b3-122">Request headers</span></span>
|<span data-ttu-id="d70b3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d70b3-123">Header</span></span>|<span data-ttu-id="d70b3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d70b3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d70b3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d70b3-125">Authorization</span></span>|<span data-ttu-id="d70b3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d70b3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d70b3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d70b3-127">Accept</span></span>|<span data-ttu-id="d70b3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d70b3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d70b3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d70b3-129">Request body</span></span>
<span data-ttu-id="d70b3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d70b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d70b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d70b3-131">Response</span></span>
<span data-ttu-id="d70b3-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d70b3-132">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70b3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d70b3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d70b3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d70b3-134">Request</span></span>
<span data-ttu-id="d70b3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d70b3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="d70b3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d70b3-136">Response</span></span>
<span data-ttu-id="d70b3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d70b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

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
    "welcomeScreenDisabled": true
  }
}
```





