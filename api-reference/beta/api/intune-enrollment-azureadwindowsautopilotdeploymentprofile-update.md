---
title: Atualizar azureADWindowsAutopilotDeploymentProfile
description: Atualize as propriedades de um objeto azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c51ab8c146678aa6e01aaa187cee1fcc6d2145cb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149958"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="ac8de-103">Atualizar azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="ac8de-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="ac8de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac8de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac8de-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac8de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac8de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac8de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac8de-107">Atualize as propriedades de um [objeto azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-107">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac8de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac8de-108">Prerequisites</span></span>
<span data-ttu-id="ac8de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac8de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac8de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac8de-111">Permission type</span></span>|<span data-ttu-id="ac8de-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac8de-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac8de-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac8de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac8de-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac8de-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac8de-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac8de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac8de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac8de-116">Not supported.</span></span>|
|<span data-ttu-id="ac8de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac8de-117">Application</span></span>|<span data-ttu-id="ac8de-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac8de-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac8de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac8de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ac8de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac8de-120">Request headers</span></span>
|<span data-ttu-id="ac8de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac8de-121">Header</span></span>|<span data-ttu-id="ac8de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac8de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac8de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac8de-123">Authorization</span></span>|<span data-ttu-id="ac8de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac8de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac8de-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac8de-125">Accept</span></span>|<span data-ttu-id="ac8de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac8de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac8de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac8de-127">Request body</span></span>
<span data-ttu-id="ac8de-128">No corpo da solicitação, fornece uma representação JSON para o [objeto azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-128">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="ac8de-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ac8de-129">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="ac8de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac8de-130">Property</span></span>|<span data-ttu-id="ac8de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac8de-131">Type</span></span>|<span data-ttu-id="ac8de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac8de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac8de-133">id</span><span class="sxs-lookup"><span data-stu-id="ac8de-133">id</span></span>|<span data-ttu-id="ac8de-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac8de-134">String</span></span>|<span data-ttu-id="ac8de-135">Chave de Perfil Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ac8de-136">displayName</span></span>|<span data-ttu-id="ac8de-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac8de-137">String</span></span>|<span data-ttu-id="ac8de-138">Nome do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-139">descrição</span><span class="sxs-lookup"><span data-stu-id="ac8de-139">description</span></span>|<span data-ttu-id="ac8de-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac8de-140">String</span></span>|<span data-ttu-id="ac8de-141">Descrição do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-142">idioma</span><span class="sxs-lookup"><span data-stu-id="ac8de-142">language</span></span>|<span data-ttu-id="ac8de-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac8de-143">String</span></span>|<span data-ttu-id="ac8de-144">Idioma configurado no dispositivo Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac8de-145">createdDateTime</span></span>|<span data-ttu-id="ac8de-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac8de-146">DateTimeOffset</span></span>|<span data-ttu-id="ac8de-147">Tempo de criação de perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac8de-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ac8de-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac8de-149">DateTimeOffset</span></span>|<span data-ttu-id="ac8de-150">Tempo de última modificação do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="ac8de-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="ac8de-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="ac8de-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="ac8de-153">Configuração de experiência fora de caixa Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="ac8de-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="ac8de-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="ac8de-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="ac8de-156">Configuração da tela de status de registro Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="ac8de-157">extractHardwareHash</span></span>|<span data-ttu-id="ac8de-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="ac8de-158">Boolean</span></span>|<span data-ttu-id="ac8de-159">Extração de HardwareHash para o perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="ac8de-160">deviceNameTemplate</span></span>|<span data-ttu-id="ac8de-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac8de-161">String</span></span>|<span data-ttu-id="ac8de-162">O modelo usado para nomear o Dispositivo AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="ac8de-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="ac8de-163">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="ac8de-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="ac8de-164">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ac8de-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="ac8de-165">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="ac8de-166">deviceType</span></span>|[<span data-ttu-id="ac8de-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="ac8de-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="ac8de-168">O tipo de dispositivo AutoPilot ao qual esse perfil é aplicável.</span><span class="sxs-lookup"><span data-stu-id="ac8de-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="ac8de-169">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ac8de-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="ac8de-170">Os valores possíveis são: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="ac8de-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="ac8de-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="ac8de-171">enableWhiteGlove</span></span>|<span data-ttu-id="ac8de-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="ac8de-172">Boolean</span></span>|<span data-ttu-id="ac8de-173">Habilitar o Autopilot White Glove para o perfil.</span><span class="sxs-lookup"><span data-stu-id="ac8de-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="ac8de-174">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ac8de-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac8de-175">roleScopeTagIds</span></span>|<span data-ttu-id="ac8de-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac8de-176">String collection</span></span>|<span data-ttu-id="ac8de-177">Marcas de escopo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="ac8de-177">Scope tags for the profile.</span></span> <span data-ttu-id="ac8de-178">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac8de-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ac8de-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac8de-179">Response</span></span>
<span data-ttu-id="ac8de-180">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac8de-180">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac8de-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac8de-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac8de-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac8de-182">Request</span></span>
<span data-ttu-id="ac8de-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac8de-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac8de-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac8de-184">Response</span></span>
<span data-ttu-id="ac8de-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac8de-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




