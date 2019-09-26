---
title: Atualizar azureADWindowsAutopilotDeploymentProfile
description: Atualiza as propriedades de um objeto azureADWindowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c70998cbbc4cb0f8e43210845590c97aeb9e2ae5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187944"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="586a7-103">Atualizar azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="586a7-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="586a7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="586a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="586a7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="586a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="586a7-106">Atualiza as propriedades de um objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="586a7-106">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="586a7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="586a7-107">Prerequisites</span></span>
<span data-ttu-id="586a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="586a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="586a7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="586a7-110">Permission type</span></span>|<span data-ttu-id="586a7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="586a7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="586a7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="586a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="586a7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="586a7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="586a7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="586a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="586a7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="586a7-115">Not supported.</span></span>|
|<span data-ttu-id="586a7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="586a7-116">Application</span></span>|<span data-ttu-id="586a7-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="586a7-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="586a7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="586a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="586a7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="586a7-119">Request headers</span></span>
|<span data-ttu-id="586a7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="586a7-120">Header</span></span>|<span data-ttu-id="586a7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="586a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="586a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="586a7-122">Authorization</span></span>|<span data-ttu-id="586a7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="586a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="586a7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="586a7-124">Accept</span></span>|<span data-ttu-id="586a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="586a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="586a7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="586a7-126">Request body</span></span>
<span data-ttu-id="586a7-127">No corpo da solicitação, forneça uma representação JSON do objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="586a7-127">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="586a7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="586a7-128">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="586a7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="586a7-129">Property</span></span>|<span data-ttu-id="586a7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="586a7-130">Type</span></span>|<span data-ttu-id="586a7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="586a7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="586a7-132">id</span><span class="sxs-lookup"><span data-stu-id="586a7-132">id</span></span>|<span data-ttu-id="586a7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="586a7-133">String</span></span>|<span data-ttu-id="586a7-134">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="586a7-135">displayName</span></span>|<span data-ttu-id="586a7-136">String</span><span class="sxs-lookup"><span data-stu-id="586a7-136">String</span></span>|<span data-ttu-id="586a7-137">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-138">descrição</span><span class="sxs-lookup"><span data-stu-id="586a7-138">description</span></span>|<span data-ttu-id="586a7-139">String</span><span class="sxs-lookup"><span data-stu-id="586a7-139">String</span></span>|<span data-ttu-id="586a7-140">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-141">idioma</span><span class="sxs-lookup"><span data-stu-id="586a7-141">language</span></span>|<span data-ttu-id="586a7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="586a7-142">String</span></span>|<span data-ttu-id="586a7-143">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="586a7-144">createdDateTime</span></span>|<span data-ttu-id="586a7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="586a7-145">DateTimeOffset</span></span>|<span data-ttu-id="586a7-146">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="586a7-147">lastModifiedDateTime</span></span>|<span data-ttu-id="586a7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="586a7-148">DateTimeOffset</span></span>|<span data-ttu-id="586a7-149">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="586a7-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="586a7-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="586a7-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="586a7-152">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="586a7-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="586a7-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="586a7-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="586a7-155">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="586a7-156">extractHardwareHash</span></span>|<span data-ttu-id="586a7-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="586a7-157">Boolean</span></span>|<span data-ttu-id="586a7-158">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="586a7-159">deviceNameTemplate</span></span>|<span data-ttu-id="586a7-160">String</span><span class="sxs-lookup"><span data-stu-id="586a7-160">String</span></span>|<span data-ttu-id="586a7-161">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="586a7-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="586a7-162">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="586a7-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="586a7-163">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="586a7-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="586a7-164">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="586a7-165">deviceType</span></span>|[<span data-ttu-id="586a7-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="586a7-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="586a7-167">O tipo de dispositivo piloto automático ao qual esse perfil se aplica.</span><span class="sxs-lookup"><span data-stu-id="586a7-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="586a7-168">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="586a7-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="586a7-169">Os valores possíveis são: `windowsPc` e `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="586a7-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="586a7-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="586a7-170">enableWhiteGlove</span></span>|<span data-ttu-id="586a7-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="586a7-171">Boolean</span></span>|<span data-ttu-id="586a7-172">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="586a7-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="586a7-173">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="586a7-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="586a7-174">roleScopeTagIds</span></span>|<span data-ttu-id="586a7-175">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="586a7-175">String collection</span></span>|<span data-ttu-id="586a7-176">Marcas de escopo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="586a7-176">Scope tags for the profile.</span></span> <span data-ttu-id="586a7-177">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="586a7-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="586a7-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="586a7-178">Response</span></span>
<span data-ttu-id="586a7-179">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="586a7-179">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="586a7-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="586a7-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="586a7-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="586a7-181">Request</span></span>
<span data-ttu-id="586a7-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="586a7-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1159

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="586a7-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="586a7-183">Response</span></span>
<span data-ttu-id="586a7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="586a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

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
```




