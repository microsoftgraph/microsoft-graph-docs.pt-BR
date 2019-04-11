---
title: tipo de recurso windowsAutopilotDeploymentProfile
description: Perfil de implantação do Windows AutoPilot
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f82d48422ecff99f106d4a62b07ac8532cb546c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794537"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="03850-103">tipo de recurso windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="03850-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="03850-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03850-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03850-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03850-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03850-106">Perfil de implantação do Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="03850-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="03850-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="03850-107">Methods</span></span>
|<span data-ttu-id="03850-108">Método</span><span class="sxs-lookup"><span data-stu-id="03850-108">Method</span></span>|<span data-ttu-id="03850-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03850-109">Return Type</span></span>|<span data-ttu-id="03850-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03850-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03850-111">Obter windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="03850-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="03850-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="03850-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="03850-113">Leia as propriedades e as relações do objeto [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="03850-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="03850-114">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="03850-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="03850-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="03850-115">None</span></span>|<span data-ttu-id="03850-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="03850-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="03850-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03850-117">Properties</span></span>
|<span data-ttu-id="03850-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03850-118">Property</span></span>|<span data-ttu-id="03850-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="03850-119">Type</span></span>|<span data-ttu-id="03850-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="03850-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03850-121">id</span><span class="sxs-lookup"><span data-stu-id="03850-121">id</span></span>|<span data-ttu-id="03850-122">String</span><span class="sxs-lookup"><span data-stu-id="03850-122">String</span></span>|<span data-ttu-id="03850-123">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="03850-123">Profile Key</span></span>|
|<span data-ttu-id="03850-124">displayName</span><span class="sxs-lookup"><span data-stu-id="03850-124">displayName</span></span>|<span data-ttu-id="03850-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03850-125">String</span></span>|<span data-ttu-id="03850-126">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="03850-126">Name of the profile</span></span>|
|<span data-ttu-id="03850-127">description</span><span class="sxs-lookup"><span data-stu-id="03850-127">description</span></span>|<span data-ttu-id="03850-128">String</span><span class="sxs-lookup"><span data-stu-id="03850-128">String</span></span>|<span data-ttu-id="03850-129">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="03850-129">Description of the profile</span></span>|
|<span data-ttu-id="03850-130">idioma</span><span class="sxs-lookup"><span data-stu-id="03850-130">language</span></span>|<span data-ttu-id="03850-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03850-131">String</span></span>|<span data-ttu-id="03850-132">Idioma configurado no dispositivo</span><span class="sxs-lookup"><span data-stu-id="03850-132">Language configured on the device</span></span>|
|<span data-ttu-id="03850-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03850-133">createdDateTime</span></span>|<span data-ttu-id="03850-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03850-134">DateTimeOffset</span></span>|<span data-ttu-id="03850-135">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="03850-135">Profile creation time</span></span>|
|<span data-ttu-id="03850-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03850-136">lastModifiedDateTime</span></span>|<span data-ttu-id="03850-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03850-137">DateTimeOffset</span></span>|<span data-ttu-id="03850-138">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="03850-138">Profile last modified time</span></span>|
|<span data-ttu-id="03850-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="03850-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="03850-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="03850-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="03850-141">Configuração de experiência inicial da caixa</span><span class="sxs-lookup"><span data-stu-id="03850-141">Out of box experience setting</span></span>|
|<span data-ttu-id="03850-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="03850-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="03850-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="03850-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="03850-144">Configuração da tela status do registro</span><span class="sxs-lookup"><span data-stu-id="03850-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="03850-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="03850-145">extractHardwareHash</span></span>|<span data-ttu-id="03850-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="03850-146">Boolean</span></span>|<span data-ttu-id="03850-147">Extração HardwareHash para o perfil</span><span class="sxs-lookup"><span data-stu-id="03850-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="03850-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="03850-148">deviceNameTemplate</span></span>|<span data-ttu-id="03850-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03850-149">String</span></span>|<span data-ttu-id="03850-150">O modelo usado para nomear o dispositivo de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="03850-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="03850-151">Pode ser um texto personalizado e também pode conter o número de série do dispositivo ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="03850-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="03850-152">O comprimento total do texto gerado pelo modelo não pode ter mais de 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="03850-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="03850-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="03850-153">deviceType</span></span>|[<span data-ttu-id="03850-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="03850-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="03850-155">O tipo de dispositivo piloto automático ao qual esse perfil se aplica.</span><span class="sxs-lookup"><span data-stu-id="03850-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="03850-156">Os valores possíveis são: `windowsPc` e `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="03850-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="03850-157">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="03850-157">enableWhiteGlove</span></span>|<span data-ttu-id="03850-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="03850-158">Boolean</span></span>|<span data-ttu-id="03850-159">Habilite o Glove branco do piloto automático para o perfil.</span><span class="sxs-lookup"><span data-stu-id="03850-159">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03850-160">Relações</span><span class="sxs-lookup"><span data-stu-id="03850-160">Relationships</span></span>
|<span data-ttu-id="03850-161">Relação</span><span class="sxs-lookup"><span data-stu-id="03850-161">Relationship</span></span>|<span data-ttu-id="03850-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="03850-162">Type</span></span>|<span data-ttu-id="03850-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="03850-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03850-164">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="03850-164">assignedDevices</span></span>|<span data-ttu-id="03850-165">coleção [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="03850-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="03850-166">A lista de dispositivos atribuídos para o perfil.</span><span class="sxs-lookup"><span data-stu-id="03850-166">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="03850-167">assignments</span><span class="sxs-lookup"><span data-stu-id="03850-167">assignments</span></span>|<span data-ttu-id="03850-168">coleção [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03850-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="03850-169">A lista de atribuições de grupo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="03850-169">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03850-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03850-170">JSON Representation</span></span>
<span data-ttu-id="03850-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03850-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true
}
```





