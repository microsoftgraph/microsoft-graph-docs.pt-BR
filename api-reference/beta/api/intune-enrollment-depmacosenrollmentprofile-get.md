---
title: Obter depMacOSEnrollmentProfile
description: Leia as propriedades e as relações do objeto depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36a02018e7b753129705af33a24e473e577360c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533329"
---
# <a name="get-depmacosenrollmentprofile"></a><span data-ttu-id="cafad-103">Obter depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cafad-103">Get depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="cafad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cafad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cafad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cafad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cafad-106">Leia as propriedades e as relações do objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cafad-106">Read properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cafad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cafad-107">Prerequisites</span></span>
<span data-ttu-id="cafad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cafad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cafad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cafad-110">Permission type</span></span>|<span data-ttu-id="cafad-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cafad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cafad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cafad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cafad-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cafad-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cafad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cafad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cafad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cafad-115">Not supported.</span></span>|
|<span data-ttu-id="cafad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cafad-116">Application</span></span>|<span data-ttu-id="cafad-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cafad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cafad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cafad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cafad-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cafad-119">Optional query parameters</span></span>
<span data-ttu-id="cafad-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cafad-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cafad-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cafad-121">Request headers</span></span>
|<span data-ttu-id="cafad-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cafad-122">Header</span></span>|<span data-ttu-id="cafad-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cafad-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cafad-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cafad-124">Authorization</span></span>|<span data-ttu-id="cafad-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cafad-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cafad-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cafad-126">Accept</span></span>|<span data-ttu-id="cafad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cafad-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cafad-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cafad-128">Request body</span></span>
<span data-ttu-id="cafad-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cafad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cafad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cafad-130">Response</span></span>
<span data-ttu-id="cafad-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cafad-131">If successful, this method returns a `200 OK` response code and [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cafad-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cafad-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cafad-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cafad-133">Request</span></span>
<span data-ttu-id="cafad-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cafad-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="cafad-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cafad-135">Response</span></span>
<span data-ttu-id="cafad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cafad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "value": {
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
    "deviceNameTemplate": "Device Name Template value",
    "registrationDisabled": true,
    "fileVaultDisabled": true,
    "iCloudDiagnosticsDisabled": true,
    "iCloudStorageDisabled": true,
    "chooseYourLockScreenDisabled": true
  }
}
```





