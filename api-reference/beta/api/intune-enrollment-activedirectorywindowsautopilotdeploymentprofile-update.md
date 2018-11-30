---
title: Atualizar activeDirectoryWindowsAutopilotDeploymentProfile
description: Atualize as propriedades de um objeto activeDirectoryWindowsAutopilotDeploymentProfile.
ms.openlocfilehash: 11b6122167ad29bfa29d9d86931436cc02aac690
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034809"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="8a029-103">Atualizar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="8a029-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="8a029-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a029-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a029-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a029-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a029-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a029-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a029-107">Atualize as propriedades de um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8a029-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a029-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a029-108">Prerequisites</span></span>
<span data-ttu-id="8a029-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a029-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a029-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a029-111">Permission type</span></span>|<span data-ttu-id="8a029-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a029-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a029-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a029-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a029-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a029-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8a029-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a029-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a029-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a029-116">Not supported.</span></span>|
|<span data-ttu-id="8a029-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a029-117">Application</span></span>|<span data-ttu-id="8a029-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a029-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a029-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a029-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="8a029-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a029-120">Request headers</span></span>
|<span data-ttu-id="8a029-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a029-121">Header</span></span>|<span data-ttu-id="8a029-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a029-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a029-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a029-123">Authorization</span></span>|<span data-ttu-id="8a029-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a029-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a029-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a029-125">Accept</span></span>|<span data-ttu-id="8a029-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a029-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a029-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a029-127">Request body</span></span>
<span data-ttu-id="8a029-128">No corpo da solicitação, fornece uma representação JSON para o objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8a029-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="8a029-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8a029-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="8a029-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a029-130">Property</span></span>|<span data-ttu-id="8a029-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a029-131">Type</span></span>|<span data-ttu-id="8a029-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a029-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a029-133">id</span><span class="sxs-lookup"><span data-stu-id="8a029-133">id</span></span>|<span data-ttu-id="8a029-134">String</span><span class="sxs-lookup"><span data-stu-id="8a029-134">String</span></span>|<span data-ttu-id="8a029-135">Herdado de chave de perfil de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8a029-136">displayName</span></span>|<span data-ttu-id="8a029-137">String</span><span class="sxs-lookup"><span data-stu-id="8a029-137">String</span></span>|<span data-ttu-id="8a029-138">Nome do perfil Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-139">description</span><span class="sxs-lookup"><span data-stu-id="8a029-139">description</span></span>|<span data-ttu-id="8a029-140">String</span><span class="sxs-lookup"><span data-stu-id="8a029-140">String</span></span>|<span data-ttu-id="8a029-141">Descrição do perfil de Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-142">idioma</span><span class="sxs-lookup"><span data-stu-id="8a029-142">language</span></span>|<span data-ttu-id="8a029-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a029-143">String</span></span>|<span data-ttu-id="8a029-144">Idioma configurado no dispositivo Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a029-145">createdDateTime</span></span>|<span data-ttu-id="8a029-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a029-146">DateTimeOffset</span></span>|<span data-ttu-id="8a029-147">Hora da criação do perfil Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a029-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8a029-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a029-149">DateTimeOffset</span></span>|<span data-ttu-id="8a029-150">Perfil da última modificação tempo Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="8a029-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="8a029-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="8a029-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="8a029-153">Configuração inicial pelo usuário Inherited a definição de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8a029-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="8a029-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8a029-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="8a029-156">Configuração Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) de tela de status de inscrição</span><span class="sxs-lookup"><span data-stu-id="8a029-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="8a029-157">extractHardwareHash</span></span>|<span data-ttu-id="8a029-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a029-158">Boolean</span></span>|<span data-ttu-id="8a029-159">Extração de HardwareHash para o perfil Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="8a029-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="8a029-160">deviceNameTemplate</span></span>|<span data-ttu-id="8a029-161">String</span><span class="sxs-lookup"><span data-stu-id="8a029-161">String</span></span>|<span data-ttu-id="8a029-162">O modelo usado para nomear o dispositivo piloto automático.</span><span class="sxs-lookup"><span data-stu-id="8a029-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="8a029-163">Isso pode ser um texto personalizado e também pode conter o número de série do dispositivo, ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="8a029-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="8a029-164">O comprimento total do texto gerado pelo modelo pode ser mais do que 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="8a029-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="8a029-165">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a029-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8a029-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a029-166">Response</span></span>
<span data-ttu-id="8a029-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a029-167">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a029-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a029-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a029-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a029-169">Request</span></span>
<span data-ttu-id="8a029-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a029-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1021

{
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="8a029-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a029-171">Response</span></span>
<span data-ttu-id="8a029-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a029-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

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
  "deviceNameTemplate": "Device Name Template value"
}
```





