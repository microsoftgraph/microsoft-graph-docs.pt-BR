---
title: Obter activeDirectoryWindowsAutopilotDeploymentProfile
description: Leia as propriedades e as relações do objeto activeDirectoryWindowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a46d75e8a1e1bf0af34f9f3d1a5d184824c0952
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467582"
---
# <a name="get-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="72022-103">Obter activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="72022-103">Get activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="72022-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72022-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72022-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72022-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72022-107">Leia as propriedades e as relações do objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="72022-107">Read properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72022-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72022-108">Prerequisites</span></span>
<span data-ttu-id="72022-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72022-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72022-111">Permission type</span></span>|<span data-ttu-id="72022-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72022-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72022-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72022-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72022-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72022-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="72022-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72022-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72022-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72022-116">Not supported.</span></span>|
|<span data-ttu-id="72022-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72022-117">Application</span></span>|<span data-ttu-id="72022-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72022-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72022-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72022-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72022-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72022-120">Optional query parameters</span></span>
<span data-ttu-id="72022-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72022-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72022-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72022-122">Request headers</span></span>
|<span data-ttu-id="72022-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72022-123">Header</span></span>|<span data-ttu-id="72022-124">Valor</span><span class="sxs-lookup"><span data-stu-id="72022-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72022-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72022-125">Authorization</span></span>|<span data-ttu-id="72022-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72022-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72022-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72022-127">Accept</span></span>|<span data-ttu-id="72022-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72022-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72022-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72022-129">Request body</span></span>
<span data-ttu-id="72022-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72022-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72022-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="72022-131">Response</span></span>
<span data-ttu-id="72022-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72022-132">If successful, this method returns a `200 OK` response code and [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72022-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72022-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="72022-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72022-134">Request</span></span>
<span data-ttu-id="72022-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72022-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="72022-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="72022-136">Response</span></span>
<span data-ttu-id="72022-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1477

{
  "value": {
    "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
    "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
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
    ],
    "hybridAzureADJoinSkipConnectivityCheck": true
  }
}
```





