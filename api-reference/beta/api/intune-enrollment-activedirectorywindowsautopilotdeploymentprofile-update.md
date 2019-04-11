---
title: Atualizar activeDirectoryWindowsAutopilotDeploymentProfile
description: Atualiza as propriedades de um objeto activeDirectoryWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a35ae105260a5bf239280c27f85fb5152b17e74
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786214"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="472cc-103">Atualizar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="472cc-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="472cc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="472cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="472cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="472cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="472cc-106">Atualiza as propriedades de um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="472cc-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="472cc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="472cc-107">Prerequisites</span></span>
<span data-ttu-id="472cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="472cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="472cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="472cc-110">Permission type</span></span>|<span data-ttu-id="472cc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="472cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="472cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="472cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="472cc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472cc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="472cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="472cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="472cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="472cc-115">Not supported.</span></span>|
|<span data-ttu-id="472cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="472cc-116">Application</span></span>|<span data-ttu-id="472cc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="472cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="472cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="472cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="472cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="472cc-119">Request headers</span></span>
|<span data-ttu-id="472cc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="472cc-120">Header</span></span>|<span data-ttu-id="472cc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="472cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="472cc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="472cc-122">Authorization</span></span>|<span data-ttu-id="472cc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="472cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="472cc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="472cc-124">Accept</span></span>|<span data-ttu-id="472cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="472cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="472cc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="472cc-126">Request body</span></span>
<span data-ttu-id="472cc-127">No corpo da solicitação, forneça uma representação JSON do objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="472cc-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="472cc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="472cc-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="472cc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="472cc-129">Property</span></span>|<span data-ttu-id="472cc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="472cc-130">Type</span></span>|<span data-ttu-id="472cc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="472cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472cc-132">id</span><span class="sxs-lookup"><span data-stu-id="472cc-132">id</span></span>|<span data-ttu-id="472cc-133">String</span><span class="sxs-lookup"><span data-stu-id="472cc-133">String</span></span>|<span data-ttu-id="472cc-134">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="472cc-135">displayName</span></span>|<span data-ttu-id="472cc-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472cc-136">String</span></span>|<span data-ttu-id="472cc-137">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-138">description</span><span class="sxs-lookup"><span data-stu-id="472cc-138">description</span></span>|<span data-ttu-id="472cc-139">String</span><span class="sxs-lookup"><span data-stu-id="472cc-139">String</span></span>|<span data-ttu-id="472cc-140">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-141">idioma</span><span class="sxs-lookup"><span data-stu-id="472cc-141">language</span></span>|<span data-ttu-id="472cc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472cc-142">String</span></span>|<span data-ttu-id="472cc-143">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="472cc-144">createdDateTime</span></span>|<span data-ttu-id="472cc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="472cc-145">DateTimeOffset</span></span>|<span data-ttu-id="472cc-146">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="472cc-147">lastModifiedDateTime</span></span>|<span data-ttu-id="472cc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="472cc-148">DateTimeOffset</span></span>|<span data-ttu-id="472cc-149">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="472cc-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="472cc-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="472cc-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="472cc-152">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="472cc-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="472cc-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="472cc-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="472cc-155">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="472cc-156">extractHardwareHash</span></span>|<span data-ttu-id="472cc-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="472cc-157">Boolean</span></span>|<span data-ttu-id="472cc-158">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="472cc-159">deviceNameTemplate</span></span>|<span data-ttu-id="472cc-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="472cc-160">String</span></span>|<span data-ttu-id="472cc-161">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="472cc-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="472cc-162">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="472cc-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="472cc-163">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="472cc-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="472cc-164">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="472cc-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="472cc-165">deviceType</span></span>|[<span data-ttu-id="472cc-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="472cc-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="472cc-167">O tipo de dispositivo piloto automático ao qual esse perfil se aplica.</span><span class="sxs-lookup"><span data-stu-id="472cc-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="472cc-168">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="472cc-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="472cc-169">Os valores possíveis são: `windowsPc` e `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="472cc-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="472cc-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="472cc-170">enableWhiteGlove</span></span>|<span data-ttu-id="472cc-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="472cc-171">Boolean</span></span>|<span data-ttu-id="472cc-172">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="472cc-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="472cc-173">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="472cc-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="472cc-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="472cc-174">Response</span></span>
<span data-ttu-id="472cc-175">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="472cc-175">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="472cc-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="472cc-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="472cc-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="472cc-177">Request</span></span>
<span data-ttu-id="472cc-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="472cc-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1105

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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

### <a name="response"></a><span data-ttu-id="472cc-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="472cc-179">Response</span></span>
<span data-ttu-id="472cc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="472cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

{
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
  "enableWhiteGlove": true
}
```





