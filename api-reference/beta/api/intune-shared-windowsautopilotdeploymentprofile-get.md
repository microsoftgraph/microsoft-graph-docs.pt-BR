---
title: Obter windowsAutopilotDeploymentProfile
description: Leia as propriedades e as relações do objeto windowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f1bf197f497924585d38db30097d440b312bd62
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702821"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="88ab2-103">Obter windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="88ab2-103">Get windowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="88ab2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ab2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88ab2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88ab2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88ab2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88ab2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88ab2-107">Leia as propriedades e as relações do objeto [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="88ab2-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88ab2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88ab2-108">Prerequisites</span></span>
<span data-ttu-id="88ab2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88ab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88ab2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88ab2-111">Permission type</span></span>|<span data-ttu-id="88ab2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88ab2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88ab2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88ab2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88ab2-114">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="88ab2-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="88ab2-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88ab2-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="88ab2-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="88ab2-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88ab2-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88ab2-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="88ab2-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88ab2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88ab2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88ab2-119">Not supported.</span></span>|
|<span data-ttu-id="88ab2-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88ab2-120">Application</span></span>||
| <span data-ttu-id="88ab2-121">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="88ab2-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="88ab2-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88ab2-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="88ab2-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="88ab2-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88ab2-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88ab2-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88ab2-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88ab2-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88ab2-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88ab2-126">Optional query parameters</span></span>
<span data-ttu-id="88ab2-127">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88ab2-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88ab2-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88ab2-128">Request headers</span></span>
|<span data-ttu-id="88ab2-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88ab2-129">Header</span></span>|<span data-ttu-id="88ab2-130">Valor</span><span class="sxs-lookup"><span data-stu-id="88ab2-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88ab2-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="88ab2-131">Authorization</span></span>|<span data-ttu-id="88ab2-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88ab2-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88ab2-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88ab2-133">Accept</span></span>|<span data-ttu-id="88ab2-134">application/json</span><span class="sxs-lookup"><span data-stu-id="88ab2-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88ab2-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88ab2-135">Request body</span></span>
<span data-ttu-id="88ab2-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88ab2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88ab2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="88ab2-137">Response</span></span>
<span data-ttu-id="88ab2-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88ab2-138">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88ab2-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88ab2-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="88ab2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88ab2-140">Request</span></span>
<span data-ttu-id="88ab2-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88ab2-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="88ab2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="88ab2-142">Response</span></span>
<span data-ttu-id="88ab2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88ab2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








