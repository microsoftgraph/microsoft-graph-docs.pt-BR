---
title: Obter azureADWindowsAutopilotDeploymentProfile
description: Leia as propriedades e os relacionamentos do objeto azureADWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c01d9c3a62d7c75aa03b6c72bc7a2c9897a5ce0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954830"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="b9811-103">Obter azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="b9811-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="b9811-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9811-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9811-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9811-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9811-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9811-107">Leia as propriedades e os relacionamentos do objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b9811-107">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9811-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9811-108">Prerequisites</span></span>
<span data-ttu-id="b9811-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9811-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9811-111">Permission type</span></span>|<span data-ttu-id="b9811-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9811-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9811-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9811-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9811-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9811-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b9811-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9811-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9811-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9811-116">Not supported.</span></span>|
|<span data-ttu-id="b9811-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9811-117">Application</span></span>|<span data-ttu-id="b9811-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9811-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9811-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9811-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9811-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9811-120">Optional query parameters</span></span>
<span data-ttu-id="b9811-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9811-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9811-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9811-122">Request headers</span></span>
|<span data-ttu-id="b9811-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9811-123">Header</span></span>|<span data-ttu-id="b9811-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b9811-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9811-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9811-125">Authorization</span></span>|<span data-ttu-id="b9811-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9811-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9811-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9811-127">Accept</span></span>|<span data-ttu-id="b9811-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b9811-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9811-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9811-129">Request body</span></span>
<span data-ttu-id="b9811-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9811-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9811-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9811-131">Response</span></span>
<span data-ttu-id="b9811-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9811-132">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9811-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9811-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9811-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9811-134">Request</span></span>
<span data-ttu-id="b9811-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9811-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="b9811-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9811-136">Response</span></span>
<span data-ttu-id="b9811-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9811-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1283

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
    "deviceNameTemplate": "Device Name Template value"
  }
}
```





