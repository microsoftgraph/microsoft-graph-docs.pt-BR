---
title: Obter windowsAutopilotDeploymentProfile
description: Leia as propriedades e as relações do objeto windowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42bbd6d7f57d5bb7951f56c74f69dfd1c01682c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532643"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="99645-103">Obter windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="99645-103">Get windowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="99645-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99645-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99645-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99645-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99645-106">Leia as propriedades e as relações do objeto [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="99645-106">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99645-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99645-107">Prerequisites</span></span>
<span data-ttu-id="99645-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99645-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99645-110">Permission type</span></span>|<span data-ttu-id="99645-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99645-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99645-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99645-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99645-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="99645-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="99645-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99645-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99645-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99645-115">Not supported.</span></span>|
|<span data-ttu-id="99645-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99645-116">Application</span></span>|<span data-ttu-id="99645-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99645-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99645-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99645-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99645-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99645-119">Optional query parameters</span></span>
<span data-ttu-id="99645-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99645-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99645-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99645-121">Request headers</span></span>
|<span data-ttu-id="99645-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99645-122">Header</span></span>|<span data-ttu-id="99645-123">Valor</span><span class="sxs-lookup"><span data-stu-id="99645-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99645-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="99645-124">Authorization</span></span>|<span data-ttu-id="99645-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99645-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99645-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99645-126">Accept</span></span>|<span data-ttu-id="99645-127">application/json</span><span class="sxs-lookup"><span data-stu-id="99645-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99645-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99645-128">Request body</span></span>
<span data-ttu-id="99645-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99645-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99645-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="99645-130">Response</span></span>
<span data-ttu-id="99645-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99645-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99645-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99645-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="99645-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99645-133">Request</span></span>
<span data-ttu-id="99645-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99645-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="99645-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="99645-135">Response</span></span>
<span data-ttu-id="99645-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99645-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1341

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
    "id": "9d6394a9-94a9-9d63-a994-639da994639d",
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
    "deviceType": "surfaceHub2",
    "enableWhiteGlove": true
  }
}
```





