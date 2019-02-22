---
title: Obter azureADWindowsAutopilotDeploymentProfile
description: Leia as propriedades e as relações do objeto azureADWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0fcdd0b9558fc0c7c225c85514ab9854b8b93c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156837"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="e9a15-103">Obter azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="e9a15-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="e9a15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9a15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9a15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9a15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9a15-106">Leia as propriedades e as relações do objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e9a15-106">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9a15-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9a15-107">Prerequisites</span></span>
<span data-ttu-id="e9a15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e9a15-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9a15-110">Permission type</span></span>|<span data-ttu-id="e9a15-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9a15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9a15-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9a15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9a15-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9a15-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e9a15-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9a15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9a15-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9a15-115">Not supported.</span></span>|
|<span data-ttu-id="e9a15-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9a15-116">Application</span></span>|<span data-ttu-id="e9a15-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9a15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9a15-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9a15-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9a15-119">Optional query parameters</span></span>
<span data-ttu-id="e9a15-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a15-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9a15-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a15-121">Request headers</span></span>
|<span data-ttu-id="e9a15-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9a15-122">Header</span></span>|<span data-ttu-id="e9a15-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e9a15-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9a15-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9a15-124">Authorization</span></span>|<span data-ttu-id="e9a15-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9a15-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9a15-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9a15-126">Accept</span></span>|<span data-ttu-id="e9a15-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e9a15-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9a15-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a15-128">Request body</span></span>
<span data-ttu-id="e9a15-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9a15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9a15-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a15-130">Response</span></span>
<span data-ttu-id="e9a15-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a15-131">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9a15-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9a15-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9a15-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a15-133">Request</span></span>
<span data-ttu-id="e9a15-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a15-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="e9a15-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a15-135">Response</span></span>
<span data-ttu-id="e9a15-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9a15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1314

{
  "value": {
    "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
    "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
    "displayName": "Display Name value",
    "description": "Description value",
    "language": "Language value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "outOfBoxExperienceSettings": {
      "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
      "hidePrivacySettings": true,
      "hideEULA": true,
      "userType": "standard",
      "deviceUsageType": "shared",
      "skipKeyboardSelectionPage": true,
      "hideEscapeLink": true
    },
    "enrollmentStatusScreenSettings": {
      "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
      "hideInstallationProgress": true,
      "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
      "blockDeviceSetupRetryByUser": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true
    },
    "extractHardwareHash": true,
    "deviceNameTemplate": "Device Name Template value",
    "enableWhiteGlove": true
  }
}
```




