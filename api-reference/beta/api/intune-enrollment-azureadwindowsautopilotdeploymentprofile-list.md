---
title: Listar azureADWindowsAutopilotDeploymentProfiles
description: Listar propriedades e relações dos objetos azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 428d2af0bd87eac8da58319a8b9cc9bfea73806e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126252"
---
# <a name="list-azureadwindowsautopilotdeploymentprofiles"></a><span data-ttu-id="4a364-103">Listar azureADWindowsAutopilotDeploymentProfiles</span><span class="sxs-lookup"><span data-stu-id="4a364-103">List azureADWindowsAutopilotDeploymentProfiles</span></span>

<span data-ttu-id="4a364-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a364-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a364-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a364-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a364-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a364-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a364-107">Listar propriedades e relações dos objetos [azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="4a364-107">List properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a364-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a364-108">Prerequisites</span></span>
<span data-ttu-id="4a364-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a364-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a364-111">Permission type</span></span>|<span data-ttu-id="4a364-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a364-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a364-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a364-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a364-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a364-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4a364-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a364-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a364-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a364-116">Not supported.</span></span>|
|<span data-ttu-id="4a364-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a364-117">Application</span></span>|<span data-ttu-id="4a364-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a364-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a364-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a364-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="4a364-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a364-120">Request headers</span></span>
|<span data-ttu-id="4a364-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a364-121">Header</span></span>|<span data-ttu-id="4a364-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a364-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a364-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a364-123">Authorization</span></span>|<span data-ttu-id="4a364-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a364-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a364-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a364-125">Accept</span></span>|<span data-ttu-id="4a364-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a364-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a364-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a364-127">Request body</span></span>
<span data-ttu-id="4a364-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a364-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a364-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a364-129">Response</span></span>
<span data-ttu-id="4a364-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a364-130">If successful, this method returns a `200 OK` response code and a collection of [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a364-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a364-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a364-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a364-132">Request</span></span>
<span data-ttu-id="4a364-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a364-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="4a364-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a364-134">Response</span></span>
<span data-ttu-id="4a364-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a364-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1496

{
  "value": [
    {
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
      "deviceType": "surfaceHub2",
      "enableWhiteGlove": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




