---
title: Atualizar activeDirectoryWindowsAutopilotDeploymentProfile
description: Atualize as propriedades de um objeto activeDirectoryWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69d91e90dfd21f67690c58931e4204a94da96622
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126273"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="e9eca-103">Atualizar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="e9eca-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="e9eca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9eca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9eca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9eca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9eca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9eca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9eca-107">Atualize as propriedades de [um objeto activeDirectoryWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9eca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9eca-108">Prerequisites</span></span>
<span data-ttu-id="e9eca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9eca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9eca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9eca-111">Permission type</span></span>|<span data-ttu-id="e9eca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9eca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9eca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9eca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9eca-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9eca-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9eca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9eca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9eca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9eca-116">Not supported.</span></span>|
|<span data-ttu-id="e9eca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9eca-117">Application</span></span>|<span data-ttu-id="e9eca-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9eca-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9eca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9eca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="e9eca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9eca-120">Request headers</span></span>
|<span data-ttu-id="e9eca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9eca-121">Header</span></span>|<span data-ttu-id="e9eca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e9eca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9eca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9eca-123">Authorization</span></span>|<span data-ttu-id="e9eca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9eca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9eca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9eca-125">Accept</span></span>|<span data-ttu-id="e9eca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9eca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9eca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9eca-127">Request body</span></span>
<span data-ttu-id="e9eca-128">No corpo da solicitação, fornece uma representação JSON para o [objeto activeDirectoryWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="e9eca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e9eca-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="e9eca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9eca-130">Property</span></span>|<span data-ttu-id="e9eca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9eca-131">Type</span></span>|<span data-ttu-id="e9eca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9eca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9eca-133">id</span><span class="sxs-lookup"><span data-stu-id="e9eca-133">id</span></span>|<span data-ttu-id="e9eca-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9eca-134">String</span></span>|<span data-ttu-id="e9eca-135">Chave de Perfil Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e9eca-136">displayName</span></span>|<span data-ttu-id="e9eca-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9eca-137">String</span></span>|<span data-ttu-id="e9eca-138">Nome do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-139">descrição</span><span class="sxs-lookup"><span data-stu-id="e9eca-139">description</span></span>|<span data-ttu-id="e9eca-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9eca-140">String</span></span>|<span data-ttu-id="e9eca-141">Descrição do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-142">idioma</span><span class="sxs-lookup"><span data-stu-id="e9eca-142">language</span></span>|<span data-ttu-id="e9eca-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9eca-143">String</span></span>|<span data-ttu-id="e9eca-144">Idioma configurado no dispositivo Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9eca-145">createdDateTime</span></span>|<span data-ttu-id="e9eca-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9eca-146">DateTimeOffset</span></span>|<span data-ttu-id="e9eca-147">Tempo de criação de perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9eca-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e9eca-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9eca-149">DateTimeOffset</span></span>|<span data-ttu-id="e9eca-150">Tempo de última modificação do perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e9eca-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="e9eca-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e9eca-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="e9eca-153">Configuração de experiência fora de caixa Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="e9eca-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="e9eca-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="e9eca-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="e9eca-156">Configuração da tela de status de registro Herdada do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="e9eca-157">extractHardwareHash</span></span>|<span data-ttu-id="e9eca-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="e9eca-158">Boolean</span></span>|<span data-ttu-id="e9eca-159">Extração de HardwareHash para o perfil Herdado do [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="e9eca-160">deviceNameTemplate</span></span>|<span data-ttu-id="e9eca-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9eca-161">String</span></span>|<span data-ttu-id="e9eca-162">O modelo usado para nomear o Dispositivo AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="e9eca-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="e9eca-163">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="e9eca-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="e9eca-164">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e9eca-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="e9eca-165">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="e9eca-166">deviceType</span></span>|[<span data-ttu-id="e9eca-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="e9eca-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="e9eca-168">O tipo de dispositivo AutoPilot ao qual esse perfil é aplicável.</span><span class="sxs-lookup"><span data-stu-id="e9eca-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="e9eca-169">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e9eca-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="e9eca-170">Os valores possíveis são: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="e9eca-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="e9eca-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="e9eca-171">enableWhiteGlove</span></span>|<span data-ttu-id="e9eca-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="e9eca-172">Boolean</span></span>|<span data-ttu-id="e9eca-173">Habilitar o Autopilot White Glove para o perfil.</span><span class="sxs-lookup"><span data-stu-id="e9eca-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="e9eca-174">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e9eca-175">roleScopeTagIds</span></span>|<span data-ttu-id="e9eca-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9eca-176">String collection</span></span>|<span data-ttu-id="e9eca-177">Marcas de escopo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="e9eca-177">Scope tags for the profile.</span></span> <span data-ttu-id="e9eca-178">Herdado [do windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e9eca-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e9eca-179">hybridAzureADJoinSkipConnectivityCheck</span><span class="sxs-lookup"><span data-stu-id="e9eca-179">hybridAzureADJoinSkipConnectivityCheck</span></span>|<span data-ttu-id="e9eca-180">Booleano</span><span class="sxs-lookup"><span data-stu-id="e9eca-180">Boolean</span></span>|<span data-ttu-id="e9eca-181">O fluxo de junção do Azure AD híbrido do Autopilot continuará mesmo que ele não estabeleça a conectividade do controlador de domínio durante o OOBE.</span><span class="sxs-lookup"><span data-stu-id="e9eca-181">The Autopilot Hybrid Azure AD join flow will continue even if it does not establish domain controller connectivity during OOBE.</span></span>|



## <a name="response"></a><span data-ttu-id="e9eca-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9eca-182">Response</span></span>
<span data-ttu-id="e9eca-183">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9eca-183">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9eca-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9eca-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9eca-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9eca-185">Request</span></span>
<span data-ttu-id="e9eca-186">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9eca-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1218

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
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```

### <a name="response"></a><span data-ttu-id="e9eca-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9eca-187">Response</span></span>
<span data-ttu-id="e9eca-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9eca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1390

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
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```




