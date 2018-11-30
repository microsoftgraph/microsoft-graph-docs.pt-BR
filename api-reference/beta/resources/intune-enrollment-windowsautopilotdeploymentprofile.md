---
title: tipo de recurso de windowsAutopilotDeploymentProfile
description: Perfil de implantação de piloto automático do Windows
ms.openlocfilehash: ed109af370d73d22d46198b206ba42dc4ebab2da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034509"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="605f6-103">tipo de recurso de windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="605f6-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="605f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="605f6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="605f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="605f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="605f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="605f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="605f6-107">Perfil de implantação de piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="605f6-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="605f6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="605f6-108">Methods</span></span>
|<span data-ttu-id="605f6-109">Método</span><span class="sxs-lookup"><span data-stu-id="605f6-109">Method</span></span>|<span data-ttu-id="605f6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="605f6-110">Return Type</span></span>|<span data-ttu-id="605f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="605f6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="605f6-112">Obter windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="605f6-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="605f6-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="605f6-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="605f6-114">Leia as propriedades e os relacionamentos do objeto [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="605f6-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="605f6-115">Ação assign</span><span class="sxs-lookup"><span data-stu-id="605f6-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="605f6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="605f6-116">None</span></span>|<span data-ttu-id="605f6-117">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="605f6-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="605f6-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="605f6-118">Properties</span></span>
|<span data-ttu-id="605f6-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="605f6-119">Property</span></span>|<span data-ttu-id="605f6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="605f6-120">Type</span></span>|<span data-ttu-id="605f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="605f6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="605f6-122">id</span><span class="sxs-lookup"><span data-stu-id="605f6-122">id</span></span>|<span data-ttu-id="605f6-123">String</span><span class="sxs-lookup"><span data-stu-id="605f6-123">String</span></span>|<span data-ttu-id="605f6-124">Chave de perfil</span><span class="sxs-lookup"><span data-stu-id="605f6-124">Profile Key</span></span>|
|<span data-ttu-id="605f6-125">displayName</span><span class="sxs-lookup"><span data-stu-id="605f6-125">displayName</span></span>|<span data-ttu-id="605f6-126">String</span><span class="sxs-lookup"><span data-stu-id="605f6-126">String</span></span>|<span data-ttu-id="605f6-127">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="605f6-127">Name of the profile</span></span>|
|<span data-ttu-id="605f6-128">description</span><span class="sxs-lookup"><span data-stu-id="605f6-128">description</span></span>|<span data-ttu-id="605f6-129">String</span><span class="sxs-lookup"><span data-stu-id="605f6-129">String</span></span>|<span data-ttu-id="605f6-130">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="605f6-130">Description of the profile</span></span>|
|<span data-ttu-id="605f6-131">idioma</span><span class="sxs-lookup"><span data-stu-id="605f6-131">language</span></span>|<span data-ttu-id="605f6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="605f6-132">String</span></span>|<span data-ttu-id="605f6-133">Idioma configurado no dispositivo</span><span class="sxs-lookup"><span data-stu-id="605f6-133">Language configured on the device</span></span>|
|<span data-ttu-id="605f6-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="605f6-134">createdDateTime</span></span>|<span data-ttu-id="605f6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="605f6-135">DateTimeOffset</span></span>|<span data-ttu-id="605f6-136">Hora da criação de perfil</span><span class="sxs-lookup"><span data-stu-id="605f6-136">Profile creation time</span></span>|
|<span data-ttu-id="605f6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="605f6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="605f6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="605f6-138">DateTimeOffset</span></span>|<span data-ttu-id="605f6-139">Hora da última modificação da perfil</span><span class="sxs-lookup"><span data-stu-id="605f6-139">Profile last modified time</span></span>|
|<span data-ttu-id="605f6-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="605f6-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="605f6-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="605f6-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="605f6-142">Configuração inicial pelo usuário configuração</span><span class="sxs-lookup"><span data-stu-id="605f6-142">Out of box experience setting</span></span>|
|<span data-ttu-id="605f6-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="605f6-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="605f6-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="605f6-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="605f6-145">Configuração de tela do status de inscrição</span><span class="sxs-lookup"><span data-stu-id="605f6-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="605f6-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="605f6-146">extractHardwareHash</span></span>|<span data-ttu-id="605f6-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="605f6-147">Boolean</span></span>|<span data-ttu-id="605f6-148">Extração de HardwareHash para o perfil</span><span class="sxs-lookup"><span data-stu-id="605f6-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="605f6-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="605f6-149">deviceNameTemplate</span></span>|<span data-ttu-id="605f6-150">String</span><span class="sxs-lookup"><span data-stu-id="605f6-150">String</span></span>|<span data-ttu-id="605f6-151">O modelo usado para nomear o dispositivo piloto automático.</span><span class="sxs-lookup"><span data-stu-id="605f6-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="605f6-152">Isso pode ser um texto personalizado e também pode conter o número de série do dispositivo, ou um número gerado aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="605f6-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="605f6-153">O comprimento total do texto gerado pelo modelo pode ser mais do que 15 caracteres.</span><span class="sxs-lookup"><span data-stu-id="605f6-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="605f6-154">Relações</span><span class="sxs-lookup"><span data-stu-id="605f6-154">Relationships</span></span>
|<span data-ttu-id="605f6-155">Relação</span><span class="sxs-lookup"><span data-stu-id="605f6-155">Relationship</span></span>|<span data-ttu-id="605f6-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="605f6-156">Type</span></span>|<span data-ttu-id="605f6-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="605f6-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="605f6-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="605f6-158">assignedDevices</span></span>|<span data-ttu-id="605f6-159">coleção [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="605f6-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="605f6-160">A lista de dispositivos atribuídos para o perfil.</span><span class="sxs-lookup"><span data-stu-id="605f6-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="605f6-161">assignments</span><span class="sxs-lookup"><span data-stu-id="605f6-161">assignments</span></span>|<span data-ttu-id="605f6-162">coleção [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="605f6-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="605f6-163">A lista de atribuições de grupo para o perfil.</span><span class="sxs-lookup"><span data-stu-id="605f6-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="605f6-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="605f6-164">JSON Representation</span></span>
<span data-ttu-id="605f6-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="605f6-165">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```





