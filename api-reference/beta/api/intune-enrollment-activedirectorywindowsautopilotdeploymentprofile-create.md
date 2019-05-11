---
title: Criar activeDirectoryWindowsAutopilotDeploymentProfile
description: Criar um novo objeto activeDirectoryWindowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e2f09d3c64630881f84cef7e4690cf82b230a61
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909166"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="94da4-103">Criar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="94da4-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="94da4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94da4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94da4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94da4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94da4-106">Criar um novo objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="94da4-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94da4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94da4-107">Prerequisites</span></span>
<span data-ttu-id="94da4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94da4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94da4-110">Permission type</span></span>|<span data-ttu-id="94da4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94da4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94da4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94da4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94da4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94da4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94da4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94da4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94da4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94da4-115">Not supported.</span></span>|
|<span data-ttu-id="94da4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94da4-116">Application</span></span>|<span data-ttu-id="94da4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94da4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94da4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94da4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="94da4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94da4-119">Request headers</span></span>
|<span data-ttu-id="94da4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94da4-120">Header</span></span>|<span data-ttu-id="94da4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94da4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94da4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94da4-122">Authorization</span></span>|<span data-ttu-id="94da4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94da4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94da4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94da4-124">Accept</span></span>|<span data-ttu-id="94da4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94da4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94da4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94da4-126">Request body</span></span>
<span data-ttu-id="94da4-127">No corpo da solicitação, forneça uma representação JSON do objeto activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="94da4-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="94da4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="94da4-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="94da4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94da4-129">Property</span></span>|<span data-ttu-id="94da4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="94da4-130">Type</span></span>|<span data-ttu-id="94da4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="94da4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94da4-132">id</span><span class="sxs-lookup"><span data-stu-id="94da4-132">id</span></span>|<span data-ttu-id="94da4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94da4-133">String</span></span>|<span data-ttu-id="94da4-134">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="94da4-135">displayName</span></span>|<span data-ttu-id="94da4-136">String</span><span class="sxs-lookup"><span data-stu-id="94da4-136">String</span></span>|<span data-ttu-id="94da4-137">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-138">description</span><span class="sxs-lookup"><span data-stu-id="94da4-138">description</span></span>|<span data-ttu-id="94da4-139">String</span><span class="sxs-lookup"><span data-stu-id="94da4-139">String</span></span>|<span data-ttu-id="94da4-140">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-141">idioma</span><span class="sxs-lookup"><span data-stu-id="94da4-141">language</span></span>|<span data-ttu-id="94da4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94da4-142">String</span></span>|<span data-ttu-id="94da4-143">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94da4-144">createdDateTime</span></span>|<span data-ttu-id="94da4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94da4-145">DateTimeOffset</span></span>|<span data-ttu-id="94da4-146">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94da4-147">lastModifiedDateTime</span></span>|<span data-ttu-id="94da4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94da4-148">DateTimeOffset</span></span>|<span data-ttu-id="94da4-149">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="94da4-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="94da4-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="94da4-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="94da4-152">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="94da4-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="94da4-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="94da4-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="94da4-155">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="94da4-156">extractHardwareHash</span></span>|<span data-ttu-id="94da4-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="94da4-157">Boolean</span></span>|<span data-ttu-id="94da4-158">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="94da4-159">deviceNameTemplate</span></span>|<span data-ttu-id="94da4-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94da4-160">String</span></span>|<span data-ttu-id="94da4-161">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="94da4-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="94da4-162">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="94da4-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="94da4-163">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="94da4-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="94da4-164">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="94da4-165">deviceType</span></span>|[<span data-ttu-id="94da4-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="94da4-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="94da4-167">O tipo de dispositivo piloto automático ao qual esse perfil se aplica.</span><span class="sxs-lookup"><span data-stu-id="94da4-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="94da4-168">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="94da4-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="94da4-169">Os valores possíveis são: `windowsPc` e `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="94da4-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="94da4-170">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="94da4-170">enableWhiteGlove</span></span>|<span data-ttu-id="94da4-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="94da4-171">Boolean</span></span>|<span data-ttu-id="94da4-172">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="94da4-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="94da4-173">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="94da4-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="94da4-174">roleScopeTagIds</span></span>|<span data-ttu-id="94da4-175">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94da4-175">String collection</span></span>|<span data-ttu-id="94da4-176">Marcas de escopo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="94da4-176">Scope tags for the profile.</span></span> <span data-ttu-id="94da4-177">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94da4-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="94da4-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="94da4-178">Response</span></span>
<span data-ttu-id="94da4-179">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94da4-179">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94da4-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94da4-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="94da4-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94da4-181">Request</span></span>
<span data-ttu-id="94da4-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94da4-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1167

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="94da4-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="94da4-183">Response</span></span>
<span data-ttu-id="94da4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94da4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1339

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




