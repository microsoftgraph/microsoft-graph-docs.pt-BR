---
title: Obter depMacOSEnrollmentProfile
description: Leia as propriedades e as relações do objeto depMacOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64351ab4ebb88278412979356cfdcbdb9b942b40
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909131"
---
# <a name="get-depmacosenrollmentprofile"></a><span data-ttu-id="e8cbd-103">Obter depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e8cbd-103">Get depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="e8cbd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8cbd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8cbd-106">Leia as propriedades e as relações do objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e8cbd-106">Read properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8cbd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8cbd-107">Prerequisites</span></span>
<span data-ttu-id="e8cbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8cbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8cbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8cbd-110">Permission type</span></span>|<span data-ttu-id="e8cbd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8cbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8cbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8cbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8cbd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8cbd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e8cbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8cbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8cbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-115">Not supported.</span></span>|
|<span data-ttu-id="e8cbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8cbd-116">Application</span></span>|<span data-ttu-id="e8cbd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8cbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8cbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8cbd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8cbd-119">Optional query parameters</span></span>
<span data-ttu-id="e8cbd-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8cbd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8cbd-121">Request headers</span></span>
|<span data-ttu-id="e8cbd-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8cbd-122">Header</span></span>|<span data-ttu-id="e8cbd-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e8cbd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8cbd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8cbd-124">Authorization</span></span>|<span data-ttu-id="e8cbd-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8cbd-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8cbd-126">Accept</span></span>|<span data-ttu-id="e8cbd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8cbd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8cbd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8cbd-128">Request body</span></span>
<span data-ttu-id="e8cbd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8cbd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8cbd-130">Response</span></span>
<span data-ttu-id="e8cbd-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-131">If successful, this method returns a `200 OK` response code and [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8cbd-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8cbd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8cbd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8cbd-133">Request</span></span>
<span data-ttu-id="e8cbd-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="e8cbd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8cbd-135">Response</span></span>
<span data-ttu-id="e8cbd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8cbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




