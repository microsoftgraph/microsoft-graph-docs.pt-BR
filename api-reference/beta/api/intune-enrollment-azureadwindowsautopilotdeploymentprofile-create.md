---
title: Criar azureADWindowsAutopilotDeploymentProfile
description: Criar um novo objeto azureADWindowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7eb84ed5865ae5ff4eba1f44aaa65bede9a5be3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467393"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="a449c-103">Criar azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="a449c-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="a449c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a449c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a449c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a449c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a449c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a449c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a449c-107">Criar um novo objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a449c-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a449c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a449c-108">Prerequisites</span></span>
<span data-ttu-id="a449c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a449c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a449c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a449c-111">Permission type</span></span>|<span data-ttu-id="a449c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a449c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a449c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a449c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a449c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a449c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a449c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a449c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a449c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a449c-116">Not supported.</span></span>|
|<span data-ttu-id="a449c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a449c-117">Application</span></span>|<span data-ttu-id="a449c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a449c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a449c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a449c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a449c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a449c-120">Request headers</span></span>
|<span data-ttu-id="a449c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a449c-121">Header</span></span>|<span data-ttu-id="a449c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a449c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a449c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a449c-123">Authorization</span></span>|<span data-ttu-id="a449c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a449c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a449c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a449c-125">Accept</span></span>|<span data-ttu-id="a449c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a449c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a449c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a449c-127">Request body</span></span>
<span data-ttu-id="a449c-128">No corpo da solicitação, forneça uma representação JSON do objeto azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="a449c-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="a449c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="a449c-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="a449c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a449c-130">Property</span></span>|<span data-ttu-id="a449c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a449c-131">Type</span></span>|<span data-ttu-id="a449c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a449c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a449c-133">id</span><span class="sxs-lookup"><span data-stu-id="a449c-133">id</span></span>|<span data-ttu-id="a449c-134">String</span><span class="sxs-lookup"><span data-stu-id="a449c-134">String</span></span>|<span data-ttu-id="a449c-135">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a449c-136">displayName</span></span>|<span data-ttu-id="a449c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a449c-137">String</span></span>|<span data-ttu-id="a449c-138">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-139">description</span><span class="sxs-lookup"><span data-stu-id="a449c-139">description</span></span>|<span data-ttu-id="a449c-140">String</span><span class="sxs-lookup"><span data-stu-id="a449c-140">String</span></span>|<span data-ttu-id="a449c-141">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-142">idioma</span><span class="sxs-lookup"><span data-stu-id="a449c-142">language</span></span>|<span data-ttu-id="a449c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a449c-143">String</span></span>|<span data-ttu-id="a449c-144">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a449c-145">createdDateTime</span></span>|<span data-ttu-id="a449c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a449c-146">DateTimeOffset</span></span>|<span data-ttu-id="a449c-147">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a449c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a449c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a449c-149">DateTimeOffset</span></span>|<span data-ttu-id="a449c-150">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a449c-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="a449c-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a449c-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="a449c-153">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a449c-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="a449c-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a449c-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="a449c-156">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="a449c-157">extractHardwareHash</span></span>|<span data-ttu-id="a449c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a449c-158">Boolean</span></span>|<span data-ttu-id="a449c-159">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="a449c-160">deviceNameTemplate</span></span>|<span data-ttu-id="a449c-161">String</span><span class="sxs-lookup"><span data-stu-id="a449c-161">String</span></span>|<span data-ttu-id="a449c-162">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="a449c-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="a449c-163">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="a449c-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="a449c-164">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a449c-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="a449c-165">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="a449c-166">deviceType</span></span>|[<span data-ttu-id="a449c-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="a449c-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="a449c-168">O tipo de dispositivo piloto automático ao qual esse perfil se aplica.</span><span class="sxs-lookup"><span data-stu-id="a449c-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="a449c-169">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a449c-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="a449c-170">Os valores possíveis são: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="a449c-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="a449c-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="a449c-171">enableWhiteGlove</span></span>|<span data-ttu-id="a449c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="a449c-172">Boolean</span></span>|<span data-ttu-id="a449c-173">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="a449c-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="a449c-174">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="a449c-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a449c-175">roleScopeTagIds</span></span>|<span data-ttu-id="a449c-176">String collection</span><span class="sxs-lookup"><span data-stu-id="a449c-176">String collection</span></span>|<span data-ttu-id="a449c-177">Marcas de escopo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="a449c-177">Scope tags for the profile.</span></span> <span data-ttu-id="a449c-178">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a449c-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a449c-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="a449c-179">Response</span></span>
<span data-ttu-id="a449c-180">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a449c-180">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a449c-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a449c-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="a449c-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a449c-182">Request</span></span>
<span data-ttu-id="a449c-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a449c-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
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

### <a name="response"></a><span data-ttu-id="a449c-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="a449c-184">Response</span></span>
<span data-ttu-id="a449c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a449c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





