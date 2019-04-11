---
title: Atualizar azureADWindowsAutopilotDeploymentProfile
description: Atualiza as propriedades de um objeto azureADWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 510d8360fb5192d5d3952c2fc56496760d6621d5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784273"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="413ee-103">Atualizar azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="413ee-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="413ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="413ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="413ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="413ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="413ee-106">Atualiza as propriedades de um objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="413ee-106">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="413ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="413ee-107">Prerequisites</span></span>
<span data-ttu-id="413ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="413ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="413ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="413ee-110">Permission type</span></span>|<span data-ttu-id="413ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="413ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="413ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="413ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="413ee-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="413ee-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="413ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="413ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="413ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="413ee-115">Not supported.</span></span>|
|<span data-ttu-id="413ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="413ee-116">Application</span></span>|<span data-ttu-id="413ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="413ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="413ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="413ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="413ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="413ee-119">Request headers</span></span>
|<span data-ttu-id="413ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="413ee-120">Header</span></span>|<span data-ttu-id="413ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="413ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="413ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="413ee-122">Authorization</span></span>|<span data-ttu-id="413ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="413ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="413ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="413ee-124">Accept</span></span>|<span data-ttu-id="413ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="413ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="413ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="413ee-126">Request body</span></span>
<span data-ttu-id="413ee-127">No corpo da solicitação, forneça uma representação JSON do objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="413ee-127">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="413ee-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="413ee-128">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="413ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="413ee-129">Property</span></span>|<span data-ttu-id="413ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="413ee-130">Type</span></span>|<span data-ttu-id="413ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="413ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="413ee-132">id</span><span class="sxs-lookup"><span data-stu-id="413ee-132">id</span></span>|<span data-ttu-id="413ee-133">String</span><span class="sxs-lookup"><span data-stu-id="413ee-133">String</span></span>|<span data-ttu-id="413ee-134">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-135">displayName</span><span class="sxs-lookup"><span data-stu-id="413ee-135">displayName</span></span>|<span data-ttu-id="413ee-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413ee-136">String</span></span>|<span data-ttu-id="413ee-137">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-138">description</span><span class="sxs-lookup"><span data-stu-id="413ee-138">description</span></span>|<span data-ttu-id="413ee-139">String</span><span class="sxs-lookup"><span data-stu-id="413ee-139">String</span></span>|<span data-ttu-id="413ee-140">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-141">idioma</span><span class="sxs-lookup"><span data-stu-id="413ee-141">language</span></span>|<span data-ttu-id="413ee-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413ee-142">String</span></span>|<span data-ttu-id="413ee-143">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="413ee-144">createdDateTime</span></span>|<span data-ttu-id="413ee-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413ee-145">DateTimeOffset</span></span>|<span data-ttu-id="413ee-146">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="413ee-147">lastModifiedDateTime</span></span>|<span data-ttu-id="413ee-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413ee-148">DateTimeOffset</span></span>|<span data-ttu-id="413ee-149">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="413ee-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="413ee-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="413ee-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="413ee-152">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="413ee-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="413ee-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="413ee-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="413ee-155">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="413ee-156">extractHardwareHash</span></span>|<span data-ttu-id="413ee-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="413ee-157">Boolean</span></span>|<span data-ttu-id="413ee-158">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="413ee-159">deviceNameTemplate</span></span>|<span data-ttu-id="413ee-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413ee-160">String</span></span>|<span data-ttu-id="413ee-161">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="413ee-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="413ee-162">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="413ee-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="413ee-163">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="413ee-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="413ee-164">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="413ee-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="413ee-165">deviceType</span></span>|[<span data-ttu-id="413ee-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="413ee-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="413ee-167">O tipo de dispositivo piloto automático ao qual esse perfil se aplica.</span><span class="sxs-lookup"><span data-stu-id="413ee-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="413ee-168">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="413ee-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="413ee-169">Os valores possíveis são: `windowsPc` e `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="413ee-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="413ee-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="413ee-170">enableWhiteGlove</span></span>|<span data-ttu-id="413ee-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="413ee-171">Boolean</span></span>|<span data-ttu-id="413ee-172">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="413ee-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="413ee-173">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="413ee-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="413ee-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="413ee-174">Response</span></span>
<span data-ttu-id="413ee-175">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="413ee-175">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="413ee-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="413ee-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="413ee-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="413ee-177">Request</span></span>
<span data-ttu-id="413ee-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="413ee-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1097

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
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
```

### <a name="response"></a><span data-ttu-id="413ee-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="413ee-179">Response</span></span>
<span data-ttu-id="413ee-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="413ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1269

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
  "enableWhiteGlove": true
}
```





