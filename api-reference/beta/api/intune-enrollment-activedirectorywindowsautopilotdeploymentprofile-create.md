---
title: Criar activeDirectoryWindowsAutopilotDeploymentProfile
description: Criar um novo objeto activeDirectoryWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8eb470994fc0227cfce3ad497bfe933df646b049
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162969"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="2ac83-103">Criar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="2ac83-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="2ac83-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ac83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ac83-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ac83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac83-106">Criar um novo objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2ac83-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ac83-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ac83-107">Prerequisites</span></span>
<span data-ttu-id="2ac83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ac83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ac83-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ac83-110">Permission type</span></span>|<span data-ttu-id="2ac83-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ac83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ac83-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ac83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ac83-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac83-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ac83-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ac83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ac83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ac83-115">Not supported.</span></span>|
|<span data-ttu-id="2ac83-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ac83-116">Application</span></span>|<span data-ttu-id="2ac83-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ac83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ac83-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ac83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2ac83-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ac83-119">Request headers</span></span>
|<span data-ttu-id="2ac83-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ac83-120">Header</span></span>|<span data-ttu-id="2ac83-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ac83-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ac83-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ac83-122">Authorization</span></span>|<span data-ttu-id="2ac83-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ac83-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ac83-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ac83-124">Accept</span></span>|<span data-ttu-id="2ac83-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ac83-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ac83-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ac83-126">Request body</span></span>
<span data-ttu-id="2ac83-127">No corpo da solicitação, forneça uma representação JSON do objeto activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="2ac83-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="2ac83-128">A tabela a seguir mostra as propriedades que são necessárias ao criar activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="2ac83-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="2ac83-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ac83-129">Property</span></span>|<span data-ttu-id="2ac83-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ac83-130">Type</span></span>|<span data-ttu-id="2ac83-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ac83-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac83-132">id</span><span class="sxs-lookup"><span data-stu-id="2ac83-132">id</span></span>|<span data-ttu-id="2ac83-133">String</span><span class="sxs-lookup"><span data-stu-id="2ac83-133">String</span></span>|<span data-ttu-id="2ac83-134">Chave de perfil herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2ac83-135">displayName</span></span>|<span data-ttu-id="2ac83-136">String</span><span class="sxs-lookup"><span data-stu-id="2ac83-136">String</span></span>|<span data-ttu-id="2ac83-137">Nome do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-138">description</span><span class="sxs-lookup"><span data-stu-id="2ac83-138">description</span></span>|<span data-ttu-id="2ac83-139">String</span><span class="sxs-lookup"><span data-stu-id="2ac83-139">String</span></span>|<span data-ttu-id="2ac83-140">Descrição do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-141">idioma</span><span class="sxs-lookup"><span data-stu-id="2ac83-141">language</span></span>|<span data-ttu-id="2ac83-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ac83-142">String</span></span>|<span data-ttu-id="2ac83-143">Idioma configurado no dispositivo herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac83-144">createdDateTime</span></span>|<span data-ttu-id="2ac83-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac83-145">DateTimeOffset</span></span>|<span data-ttu-id="2ac83-146">Tempo de criação de perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac83-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2ac83-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac83-148">DateTimeOffset</span></span>|<span data-ttu-id="2ac83-149">Hora da última modificação do perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="2ac83-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="2ac83-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="2ac83-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="2ac83-152">Configuração de experiência inicial da caixa herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-153">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="2ac83-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="2ac83-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="2ac83-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="2ac83-155">Configuração da tela de status do registro herdada de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-156">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="2ac83-156">extractHardwareHash</span></span>|<span data-ttu-id="2ac83-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ac83-157">Boolean</span></span>|<span data-ttu-id="2ac83-158">Extração HardwareHash para o perfil herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-159">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="2ac83-159">deviceNameTemplate</span></span>|<span data-ttu-id="2ac83-160">String</span><span class="sxs-lookup"><span data-stu-id="2ac83-160">String</span></span>|<span data-ttu-id="2ac83-161">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="2ac83-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="2ac83-162">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="2ac83-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="2ac83-163">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2ac83-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="2ac83-164">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="2ac83-165">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="2ac83-165">enableWhiteGlove</span></span>|<span data-ttu-id="2ac83-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ac83-166">Boolean</span></span>|<span data-ttu-id="2ac83-167">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="2ac83-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="2ac83-168">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2ac83-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2ac83-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ac83-169">Response</span></span>
<span data-ttu-id="2ac83-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ac83-170">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ac83-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ac83-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ac83-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ac83-172">Request</span></span>
<span data-ttu-id="2ac83-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ac83-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
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

### <a name="response"></a><span data-ttu-id="2ac83-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ac83-174">Response</span></span>
<span data-ttu-id="2ac83-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ac83-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




