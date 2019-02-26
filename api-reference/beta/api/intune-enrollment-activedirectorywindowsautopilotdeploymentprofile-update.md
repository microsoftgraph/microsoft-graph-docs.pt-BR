---
title: Atualizar activeDirectoryWindowsAutopilotDeploymentProfile
description: Atualiza as propriedades de um objeto activeDirectoryWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e76fc466195989c82728bf1bba972e876c9ef186
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160057"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="da3f7-103">Atualizar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="da3f7-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="da3f7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da3f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da3f7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da3f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da3f7-106">Atualiza as propriedades de um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="da3f7-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da3f7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da3f7-107">Prerequisites</span></span>
<span data-ttu-id="da3f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="da3f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="da3f7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da3f7-110">Permission type</span></span>|<span data-ttu-id="da3f7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da3f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da3f7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da3f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da3f7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da3f7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="da3f7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da3f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da3f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da3f7-115">Not supported.</span></span>|
|<span data-ttu-id="da3f7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da3f7-116">Application</span></span>|<span data-ttu-id="da3f7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da3f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da3f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da3f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="da3f7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da3f7-119">Request headers</span></span>
|<span data-ttu-id="da3f7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da3f7-120">Header</span></span>|<span data-ttu-id="da3f7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="da3f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da3f7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="da3f7-122">Authorization</span></span>|<span data-ttu-id="da3f7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da3f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da3f7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da3f7-124">Accept</span></span>|<span data-ttu-id="da3f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da3f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da3f7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da3f7-126">Request body</span></span>
<span data-ttu-id="da3f7-127">No corpo da solicitação, forneça uma representação JSON do objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="da3f7-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="da3f7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="da3f7-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="da3f7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da3f7-129">Property</span></span>|<span data-ttu-id="da3f7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="da3f7-130">Type</span></span>|<span data-ttu-id="da3f7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="da3f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da3f7-132">id</span><span class="sxs-lookup"><span data-stu-id="da3f7-132">id</span></span>|<span data-ttu-id="da3f7-133">String</span><span class="sxs-lookup"><span data-stu-id="da3f7-133">String</span></span>|<span data-ttu-id="da3f7-134">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="da3f7-135">displayName</span></span>|<span data-ttu-id="da3f7-136">String</span><span class="sxs-lookup"><span data-stu-id="da3f7-136">String</span></span>|<span data-ttu-id="da3f7-137">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-138">description</span><span class="sxs-lookup"><span data-stu-id="da3f7-138">description</span></span>|<span data-ttu-id="da3f7-139">String</span><span class="sxs-lookup"><span data-stu-id="da3f7-139">String</span></span>|<span data-ttu-id="da3f7-140">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-141">idioma</span><span class="sxs-lookup"><span data-stu-id="da3f7-141">language</span></span>|<span data-ttu-id="da3f7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da3f7-142">String</span></span>|<span data-ttu-id="da3f7-143">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da3f7-144">createdDateTime</span></span>|<span data-ttu-id="da3f7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3f7-145">DateTimeOffset</span></span>|<span data-ttu-id="da3f7-146">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da3f7-147">lastModifiedDateTime</span></span>|<span data-ttu-id="da3f7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da3f7-148">DateTimeOffset</span></span>|<span data-ttu-id="da3f7-149">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="da3f7-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="da3f7-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="da3f7-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="da3f7-152">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="da3f7-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="da3f7-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="da3f7-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="da3f7-155">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="da3f7-156">extractHardwareHash</span></span>|<span data-ttu-id="da3f7-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3f7-157">Boolean</span></span>|<span data-ttu-id="da3f7-158">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="da3f7-159">deviceNameTemplate</span></span>|<span data-ttu-id="da3f7-160">String</span><span class="sxs-lookup"><span data-stu-id="da3f7-160">String</span></span>|<span data-ttu-id="da3f7-161">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="da3f7-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="da3f7-162">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="da3f7-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="da3f7-163">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="da3f7-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="da3f7-164">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="da3f7-165">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="da3f7-165">enableWhiteGlove</span></span>|<span data-ttu-id="da3f7-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="da3f7-166">Boolean</span></span>|<span data-ttu-id="da3f7-167">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="da3f7-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="da3f7-168">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="da3f7-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="da3f7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="da3f7-169">Response</span></span>
<span data-ttu-id="da3f7-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da3f7-170">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3f7-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da3f7-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="da3f7-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da3f7-172">Request</span></span>
<span data-ttu-id="da3f7-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da3f7-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1073

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
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="da3f7-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="da3f7-174">Response</span></span>
<span data-ttu-id="da3f7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da3f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

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
  "enableWhiteGlove": true
}
```




