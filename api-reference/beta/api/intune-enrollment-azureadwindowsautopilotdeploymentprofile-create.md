---
title: Criar azureADWindowsAutopilotDeploymentProfile
description: Crie um novo objeto azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c8816c71808a2ee7175cf89c90d78d0ba6cbd7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146045"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="1e6da-103">Criar azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="1e6da-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="1e6da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e6da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e6da-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e6da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e6da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e6da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e6da-107">Crie um novo [objeto azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e6da-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e6da-108">Prerequisites</span></span>
<span data-ttu-id="1e6da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e6da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e6da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e6da-111">Permission type</span></span>|<span data-ttu-id="1e6da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e6da-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e6da-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e6da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e6da-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e6da-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e6da-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e6da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e6da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e6da-116">Not supported.</span></span>|
|<span data-ttu-id="1e6da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e6da-117">Application</span></span>|<span data-ttu-id="1e6da-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e6da-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e6da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e6da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1e6da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e6da-120">Request headers</span></span>
|<span data-ttu-id="1e6da-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e6da-121">Header</span></span>|<span data-ttu-id="1e6da-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e6da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e6da-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e6da-123">Authorization</span></span>|<span data-ttu-id="1e6da-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e6da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e6da-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e6da-125">Accept</span></span>|<span data-ttu-id="1e6da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e6da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e6da-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e6da-127">Request body</span></span>
<span data-ttu-id="1e6da-128">No corpo da solicitação, fornece uma representação JSON para o objeto azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="1e6da-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="1e6da-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="1e6da-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="1e6da-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e6da-130">Property</span></span>|<span data-ttu-id="1e6da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e6da-131">Type</span></span>|<span data-ttu-id="1e6da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e6da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e6da-133">id</span><span class="sxs-lookup"><span data-stu-id="1e6da-133">id</span></span>|<span data-ttu-id="1e6da-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e6da-134">String</span></span>|<span data-ttu-id="1e6da-135">Chave de Perfil Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1e6da-136">displayName</span></span>|<span data-ttu-id="1e6da-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e6da-137">String</span></span>|<span data-ttu-id="1e6da-138">Nome do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-139">descrição</span><span class="sxs-lookup"><span data-stu-id="1e6da-139">description</span></span>|<span data-ttu-id="1e6da-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e6da-140">String</span></span>|<span data-ttu-id="1e6da-141">Descrição do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-142">idioma</span><span class="sxs-lookup"><span data-stu-id="1e6da-142">language</span></span>|<span data-ttu-id="1e6da-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e6da-143">String</span></span>|<span data-ttu-id="1e6da-144">Idioma configurado no dispositivo Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e6da-145">createdDateTime</span></span>|<span data-ttu-id="1e6da-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e6da-146">DateTimeOffset</span></span>|<span data-ttu-id="1e6da-147">Tempo de criação de perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e6da-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1e6da-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e6da-149">DateTimeOffset</span></span>|<span data-ttu-id="1e6da-150">Tempo de última modificação do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="1e6da-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="1e6da-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="1e6da-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="1e6da-153">Configuração de experiência fora de caixa Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="1e6da-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="1e6da-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="1e6da-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="1e6da-156">Configuração da tela de status de registro Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="1e6da-157">extractHardwareHash</span></span>|<span data-ttu-id="1e6da-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="1e6da-158">Boolean</span></span>|<span data-ttu-id="1e6da-159">Extração de HardwareHash para o perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="1e6da-160">deviceNameTemplate</span></span>|<span data-ttu-id="1e6da-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e6da-161">String</span></span>|<span data-ttu-id="1e6da-162">O modelo usado para nomear o Dispositivo AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="1e6da-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="1e6da-163">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="1e6da-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="1e6da-164">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1e6da-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="1e6da-165">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="1e6da-166">deviceType</span></span>|[<span data-ttu-id="1e6da-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="1e6da-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="1e6da-168">O tipo de dispositivo AutoPilot ao qual esse perfil é aplicável.</span><span class="sxs-lookup"><span data-stu-id="1e6da-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="1e6da-169">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="1e6da-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="1e6da-170">Os valores possíveis são: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="1e6da-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="1e6da-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="1e6da-171">enableWhiteGlove</span></span>|<span data-ttu-id="1e6da-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="1e6da-172">Boolean</span></span>|<span data-ttu-id="1e6da-173">Habilitar o Autopilot White Glove para o perfil.</span><span class="sxs-lookup"><span data-stu-id="1e6da-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="1e6da-174">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="1e6da-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e6da-175">roleScopeTagIds</span></span>|<span data-ttu-id="1e6da-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e6da-176">String collection</span></span>|<span data-ttu-id="1e6da-177">Marcas de escopo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="1e6da-177">Scope tags for the profile.</span></span> <span data-ttu-id="1e6da-178">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e6da-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1e6da-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e6da-179">Response</span></span>
<span data-ttu-id="1e6da-180">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e6da-180">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e6da-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e6da-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e6da-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e6da-182">Request</span></span>
<span data-ttu-id="1e6da-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e6da-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e6da-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e6da-184">Response</span></span>
<span data-ttu-id="1e6da-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e6da-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




