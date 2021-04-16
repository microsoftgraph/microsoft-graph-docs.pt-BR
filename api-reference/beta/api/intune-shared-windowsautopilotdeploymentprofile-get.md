---
title: Obter windowsAutopilotDeploymentProfile
description: Leia propriedades e relações do objeto windowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ab309a198887601778724f473f31e622a6ec9c0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866395"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="2e252-103">Obter windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="2e252-103">Get windowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="2e252-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e252-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e252-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e252-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e252-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e252-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e252-107">Leia propriedades e relações do [objeto windowsAutopilotDeploymentProfile.](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2e252-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e252-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e252-108">Prerequisites</span></span>
<span data-ttu-id="2e252-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e252-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e252-111">Permission type</span></span>|<span data-ttu-id="2e252-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e252-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e252-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e252-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2e252-114">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="2e252-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="2e252-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e252-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="2e252-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="2e252-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2e252-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e252-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2e252-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e252-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e252-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e252-119">Not supported.</span></span>|
|<span data-ttu-id="2e252-120">Application</span><span class="sxs-lookup"><span data-stu-id="2e252-120">Application</span></span>||
| <span data-ttu-id="2e252-121">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="2e252-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="2e252-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e252-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="2e252-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="2e252-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2e252-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e252-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e252-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e252-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e252-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e252-126">Optional query parameters</span></span>
<span data-ttu-id="2e252-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e252-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e252-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e252-128">Request headers</span></span>
|<span data-ttu-id="2e252-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e252-129">Header</span></span>|<span data-ttu-id="2e252-130">Valor</span><span class="sxs-lookup"><span data-stu-id="2e252-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e252-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e252-131">Authorization</span></span>|<span data-ttu-id="2e252-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e252-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e252-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e252-133">Accept</span></span>|<span data-ttu-id="2e252-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2e252-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e252-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e252-135">Request body</span></span>
<span data-ttu-id="2e252-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e252-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e252-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e252-137">Response</span></span>
<span data-ttu-id="2e252-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e252-138">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e252-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e252-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e252-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e252-140">Request</span></span>
<span data-ttu-id="2e252-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e252-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="2e252-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e252-142">Response</span></span>
<span data-ttu-id="2e252-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e252-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

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
    "enableWhiteGlove": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```







