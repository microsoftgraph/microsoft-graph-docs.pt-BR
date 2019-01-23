---
title: Atualizar activeDirectoryWindowsAutopilotDeploymentProfile
description: Atualize as propriedades de um objeto activeDirectoryWindowsAutopilotDeploymentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 929ab9b026052422187eb4e94446011f3abb6f26
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404362"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="9a6ef-103">Atualizar activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="9a6ef-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="9a6ef-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a6ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a6ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a6ef-107">Atualize as propriedades de um objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9a6ef-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a6ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a6ef-108">Prerequisites</span></span>
<span data-ttu-id="9a6ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a6ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a6ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a6ef-111">Permission type</span></span>|<span data-ttu-id="9a6ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a6ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a6ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a6ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a6ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-116">Not supported.</span></span>|
|<span data-ttu-id="9a6ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a6ef-117">Application</span></span>|<span data-ttu-id="9a6ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a6ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a6ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="9a6ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a6ef-120">Request headers</span></span>
|<span data-ttu-id="9a6ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a6ef-121">Header</span></span>|<span data-ttu-id="9a6ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a6ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a6ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a6ef-123">Authorization</span></span>|<span data-ttu-id="9a6ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a6ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a6ef-125">Accept</span></span>|<span data-ttu-id="9a6ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a6ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a6ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a6ef-127">Request body</span></span>
<span data-ttu-id="9a6ef-128">No corpo da solicitação, fornece uma representação JSON para o objeto [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9a6ef-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="9a6ef-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9a6ef-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="9a6ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a6ef-130">Property</span></span>|<span data-ttu-id="9a6ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a6ef-131">Type</span></span>|<span data-ttu-id="9a6ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a6ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a6ef-133">id</span><span class="sxs-lookup"><span data-stu-id="9a6ef-133">id</span></span>|<span data-ttu-id="9a6ef-134">String</span><span class="sxs-lookup"><span data-stu-id="9a6ef-134">String</span></span>|<span data-ttu-id="9a6ef-135">Herdado de chave de perfil de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9a6ef-136">displayName</span></span>|<span data-ttu-id="9a6ef-137">String</span><span class="sxs-lookup"><span data-stu-id="9a6ef-137">String</span></span>|<span data-ttu-id="9a6ef-138">Nome do perfil Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-139">description</span><span class="sxs-lookup"><span data-stu-id="9a6ef-139">description</span></span>|<span data-ttu-id="9a6ef-140">String</span><span class="sxs-lookup"><span data-stu-id="9a6ef-140">String</span></span>|<span data-ttu-id="9a6ef-141">Descrição do perfil de Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-142">idioma</span><span class="sxs-lookup"><span data-stu-id="9a6ef-142">language</span></span>|<span data-ttu-id="9a6ef-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a6ef-143">String</span></span>|<span data-ttu-id="9a6ef-144">Idioma configurado no dispositivo Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a6ef-145">createdDateTime</span></span>|<span data-ttu-id="9a6ef-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a6ef-146">DateTimeOffset</span></span>|<span data-ttu-id="9a6ef-147">Hora da criação do perfil Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a6ef-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9a6ef-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a6ef-149">DateTimeOffset</span></span>|<span data-ttu-id="9a6ef-150">Perfil da última modificação tempo Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="9a6ef-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="9a6ef-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="9a6ef-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="9a6ef-153">Configuração inicial pelo usuário Inherited a definição de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="9a6ef-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="9a6ef-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="9a6ef-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="9a6ef-156">Configuração Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) de tela de status de inscrição</span><span class="sxs-lookup"><span data-stu-id="9a6ef-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="9a6ef-157">extractHardwareHash</span></span>|<span data-ttu-id="9a6ef-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a6ef-158">Boolean</span></span>|<span data-ttu-id="9a6ef-159">Extração de HardwareHash para o perfil Inherited de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="9a6ef-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="9a6ef-160">deviceNameTemplate</span></span>|<span data-ttu-id="9a6ef-161">String</span><span class="sxs-lookup"><span data-stu-id="9a6ef-161">String</span></span>|<span data-ttu-id="9a6ef-162">O modelo usado para nomear o dispositivo piloto automático.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="9a6ef-163">Isso pode ser um texto personalizado e também pode conter o número de série do dispositivo, ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="9a6ef-164">O comprimento total do texto gerado pelo modelo pode ser mais do que 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="9a6ef-165">Herdado de [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9a6ef-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9a6ef-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a6ef-166">Response</span></span>
<span data-ttu-id="9a6ef-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-167">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a6ef-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a6ef-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a6ef-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a6ef-169">Request</span></span>
<span data-ttu-id="9a6ef-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1044

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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="9a6ef-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a6ef-171">Response</span></span>
<span data-ttu-id="9a6ef-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a6ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




