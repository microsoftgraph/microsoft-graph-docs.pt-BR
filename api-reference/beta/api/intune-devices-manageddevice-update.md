---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
ms.openlocfilehash: fa831967b7c091e8f698de4acef70cfec7119435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035814"
---
# <a name="update-manageddevice"></a><span data-ttu-id="00d8b-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="00d8b-103">Update managedDevice</span></span>

> <span data-ttu-id="00d8b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="00d8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00d8b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00d8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00d8b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="00d8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00d8b-107">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="00d8b-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00d8b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00d8b-108">Prerequisites</span></span>
<span data-ttu-id="00d8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00d8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00d8b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00d8b-111">Permission type</span></span>|<span data-ttu-id="00d8b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00d8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00d8b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00d8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00d8b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00d8b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="00d8b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00d8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00d8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00d8b-116">Not supported.</span></span>|
|<span data-ttu-id="00d8b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00d8b-117">Application</span></span>|<span data-ttu-id="00d8b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00d8b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00d8b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00d8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="00d8b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00d8b-120">Request headers</span></span>
|<span data-ttu-id="00d8b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00d8b-121">Header</span></span>|<span data-ttu-id="00d8b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="00d8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00d8b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="00d8b-123">Authorization</span></span>|<span data-ttu-id="00d8b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00d8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00d8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00d8b-125">Accept</span></span>|<span data-ttu-id="00d8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00d8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00d8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00d8b-127">Request body</span></span>
<span data-ttu-id="00d8b-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="00d8b-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="00d8b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="00d8b-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="00d8b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00d8b-130">Property</span></span>|<span data-ttu-id="00d8b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00d8b-131">Type</span></span>|<span data-ttu-id="00d8b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00d8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00d8b-133">id</span><span class="sxs-lookup"><span data-stu-id="00d8b-133">id</span></span>|<span data-ttu-id="00d8b-134">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-134">String</span></span>|<span data-ttu-id="00d8b-135">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-135">Unique Identifier for the device</span></span>|
|<span data-ttu-id="00d8b-136">userId</span><span class="sxs-lookup"><span data-stu-id="00d8b-136">userId</span></span>|<span data-ttu-id="00d8b-137">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-137">String</span></span>|<span data-ttu-id="00d8b-138">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-138">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="00d8b-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="00d8b-139">deviceName</span></span>|<span data-ttu-id="00d8b-140">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-140">String</span></span>|<span data-ttu-id="00d8b-141">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-141">Name of the device</span></span>|
|<span data-ttu-id="00d8b-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="00d8b-142">hardwareInformation</span></span>|[<span data-ttu-id="00d8b-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="00d8b-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="00d8b-144">Os detalhes de hardware do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-144">The hardward details for the device.</span></span>  <span data-ttu-id="00d8b-145">Inclui informações como o espaço de armazenamento, fabricante, número de série, etc.</span><span class="sxs-lookup"><span data-stu-id="00d8b-145">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="00d8b-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="00d8b-146">ownerType</span></span>|[<span data-ttu-id="00d8b-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="00d8b-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="00d8b-148">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-148">Ownership of the device.</span></span> <span data-ttu-id="00d8b-149">Pode ser 'empresa' ou 'pessoal'.</span><span class="sxs-lookup"><span data-stu-id="00d8b-149">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="00d8b-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="00d8b-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="00d8b-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="00d8b-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="00d8b-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="00d8b-153">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-153">Ownership of the device.</span></span> <span data-ttu-id="00d8b-154">Pode ser 'empresa' ou 'pessoal'.</span><span class="sxs-lookup"><span data-stu-id="00d8b-154">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="00d8b-155">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="00d8b-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="00d8b-156">deviceActionResults</span></span>|<span data-ttu-id="00d8b-157">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="00d8b-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="00d8b-158">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="00d8b-158">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="00d8b-159">managementState</span><span class="sxs-lookup"><span data-stu-id="00d8b-159">managementState</span></span>|[<span data-ttu-id="00d8b-160">managementState</span><span class="sxs-lookup"><span data-stu-id="00d8b-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="00d8b-161">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-161">Management state of the device.</span></span> <span data-ttu-id="00d8b-162">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-162">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="00d8b-163">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="00d8b-163">enrolledDateTime</span></span>|<span data-ttu-id="00d8b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-164">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-165">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-165">Enrollment time of the device.</span></span>|
|<span data-ttu-id="00d8b-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="00d8b-166">lastSyncDateTime</span></span>|<span data-ttu-id="00d8b-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-167">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-168">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="00d8b-168">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="00d8b-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="00d8b-169">chassisType</span></span>|[<span data-ttu-id="00d8b-170">chassisType</span><span class="sxs-lookup"><span data-stu-id="00d8b-170">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="00d8b-171">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-171">Chassis type of the device.</span></span> <span data-ttu-id="00d8b-172">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-172">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="00d8b-173">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="00d8b-173">operatingSystem</span></span>|<span data-ttu-id="00d8b-174">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-174">String</span></span>|<span data-ttu-id="00d8b-175">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-175">Operating system of the device.</span></span> <span data-ttu-id="00d8b-176">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="00d8b-176">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="00d8b-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="00d8b-177">deviceType</span></span>|[<span data-ttu-id="00d8b-178">deviceType</span><span class="sxs-lookup"><span data-stu-id="00d8b-178">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="00d8b-179">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-179">Platform of the device.</span></span> <span data-ttu-id="00d8b-180">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-180">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="00d8b-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="00d8b-181">complianceState</span></span>|[<span data-ttu-id="00d8b-182">complianceState</span><span class="sxs-lookup"><span data-stu-id="00d8b-182">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="00d8b-183">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-183">Compliance state of the device.</span></span> <span data-ttu-id="00d8b-184">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-184">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="00d8b-185">jailBroken</span><span class="sxs-lookup"><span data-stu-id="00d8b-185">jailBroken</span></span>|<span data-ttu-id="00d8b-186">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-186">String</span></span>|<span data-ttu-id="00d8b-187">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="00d8b-187">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="00d8b-188">managementAgent</span><span class="sxs-lookup"><span data-stu-id="00d8b-188">managementAgent</span></span>|[<span data-ttu-id="00d8b-189">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="00d8b-189">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="00d8b-190">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-190">Management channel of the device.</span></span> <span data-ttu-id="00d8b-191">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-191">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="00d8b-192">osVersion</span><span class="sxs-lookup"><span data-stu-id="00d8b-192">osVersion</span></span>|<span data-ttu-id="00d8b-193">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-193">String</span></span>|<span data-ttu-id="00d8b-194">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-194">Operating system version of the device.</span></span>|
|<span data-ttu-id="00d8b-195">easActivated</span><span class="sxs-lookup"><span data-stu-id="00d8b-195">easActivated</span></span>|<span data-ttu-id="00d8b-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-196">Boolean</span></span>|<span data-ttu-id="00d8b-197">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="00d8b-197">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="00d8b-198">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="00d8b-198">easDeviceId</span></span>|<span data-ttu-id="00d8b-199">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-199">String</span></span>|<span data-ttu-id="00d8b-200">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-200">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="00d8b-201">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="00d8b-201">easActivationDateTime</span></span>|<span data-ttu-id="00d8b-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-202">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-203">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-203">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="00d8b-204">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="00d8b-204">aadRegistered</span></span>|<span data-ttu-id="00d8b-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-205">Boolean</span></span>|<span data-ttu-id="00d8b-206">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00d8b-206">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="00d8b-207">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="00d8b-207">azureADRegistered</span></span>|<span data-ttu-id="00d8b-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-208">Boolean</span></span>|<span data-ttu-id="00d8b-209">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00d8b-209">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="00d8b-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="00d8b-210">deviceEnrollmentType</span></span>|[<span data-ttu-id="00d8b-211">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="00d8b-211">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="00d8b-212">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-212">Enrollment type of the device.</span></span> <span data-ttu-id="00d8b-213">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-213">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="00d8b-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="00d8b-214">lostModeState</span></span>|[<span data-ttu-id="00d8b-215">lostModeState</span><span class="sxs-lookup"><span data-stu-id="00d8b-215">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="00d8b-216">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="00d8b-216">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="00d8b-217">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-217">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="00d8b-218">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="00d8b-218">activationLockBypassCode</span></span>|<span data-ttu-id="00d8b-219">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-219">String</span></span>|<span data-ttu-id="00d8b-220">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="00d8b-220">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="00d8b-221">emailAddress</span><span class="sxs-lookup"><span data-stu-id="00d8b-221">emailAddress</span></span>|<span data-ttu-id="00d8b-222">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-222">String</span></span>|<span data-ttu-id="00d8b-223">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-223">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="00d8b-224">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="00d8b-224">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="00d8b-225">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-225">String</span></span>|<span data-ttu-id="00d8b-226">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00d8b-226">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="00d8b-227">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00d8b-227">Read only.</span></span>|
|<span data-ttu-id="00d8b-228">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="00d8b-228">azureADDeviceId</span></span>|<span data-ttu-id="00d8b-229">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-229">String</span></span>|<span data-ttu-id="00d8b-230">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00d8b-230">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="00d8b-231">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00d8b-231">Read only.</span></span>|
|<span data-ttu-id="00d8b-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="00d8b-232">deviceRegistrationState</span></span>|[<span data-ttu-id="00d8b-233">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="00d8b-233">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="00d8b-234">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-234">Device registration state.</span></span> <span data-ttu-id="00d8b-235">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-235">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="00d8b-236">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="00d8b-236">deviceCategoryDisplayName</span></span>|<span data-ttu-id="00d8b-237">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-237">String</span></span>|<span data-ttu-id="00d8b-238">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-238">Device category display name</span></span>|
|<span data-ttu-id="00d8b-239">isSupervised</span><span class="sxs-lookup"><span data-stu-id="00d8b-239">isSupervised</span></span>|<span data-ttu-id="00d8b-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-240">Boolean</span></span>|<span data-ttu-id="00d8b-241">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-241">Device supervised status</span></span>|
|<span data-ttu-id="00d8b-242">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="00d8b-242">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="00d8b-243">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-243">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-244">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="00d8b-244">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="00d8b-245">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="00d8b-245">exchangeAccessState</span></span>|[<span data-ttu-id="00d8b-246">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="00d8b-246">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="00d8b-247">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="00d8b-247">The Access State of the device in Exchange.</span></span> <span data-ttu-id="00d8b-248">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-248">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="00d8b-249">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="00d8b-249">exchangeAccessStateReason</span></span>|[<span data-ttu-id="00d8b-250">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="00d8b-250">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="00d8b-251">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="00d8b-251">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="00d8b-252">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-252">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="00d8b-253">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="00d8b-253">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="00d8b-254">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-254">String</span></span>|<span data-ttu-id="00d8b-255">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-255">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="00d8b-256">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="00d8b-256">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="00d8b-257">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-257">String</span></span>|<span data-ttu-id="00d8b-258">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="00d8b-258">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="00d8b-259">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="00d8b-259">isEncrypted</span></span>|<span data-ttu-id="00d8b-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-260">Boolean</span></span>|<span data-ttu-id="00d8b-261">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-261">Device encryption status</span></span>|
|<span data-ttu-id="00d8b-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00d8b-262">userPrincipalName</span></span>|<span data-ttu-id="00d8b-263">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-263">String</span></span>|<span data-ttu-id="00d8b-264">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-264">Device user principal name</span></span>|
|<span data-ttu-id="00d8b-265">modelo</span><span class="sxs-lookup"><span data-stu-id="00d8b-265">model</span></span>|<span data-ttu-id="00d8b-266">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-266">String</span></span>|<span data-ttu-id="00d8b-267">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-267">Model of the device</span></span>|
|<span data-ttu-id="00d8b-268">fabricante</span><span class="sxs-lookup"><span data-stu-id="00d8b-268">manufacturer</span></span>|<span data-ttu-id="00d8b-269">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-269">String</span></span>|<span data-ttu-id="00d8b-270">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-270">Manufacturer of the device</span></span>|
|<span data-ttu-id="00d8b-271">imei</span><span class="sxs-lookup"><span data-stu-id="00d8b-271">imei</span></span>|<span data-ttu-id="00d8b-272">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-272">String</span></span>|<span data-ttu-id="00d8b-273">IMEI</span><span class="sxs-lookup"><span data-stu-id="00d8b-273">IMEI</span></span>|
|<span data-ttu-id="00d8b-274">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="00d8b-274">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="00d8b-275">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-275">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-276">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="00d8b-276">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="00d8b-277">serialNumber</span><span class="sxs-lookup"><span data-stu-id="00d8b-277">serialNumber</span></span>|<span data-ttu-id="00d8b-278">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-278">String</span></span>|<span data-ttu-id="00d8b-279">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="00d8b-279">SerialNumber</span></span>|
|<span data-ttu-id="00d8b-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="00d8b-280">phoneNumber</span></span>|<span data-ttu-id="00d8b-281">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-281">String</span></span>|<span data-ttu-id="00d8b-282">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-282">Phone number of the device</span></span>|
|<span data-ttu-id="00d8b-283">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="00d8b-283">androidSecurityPatchLevel</span></span>|<span data-ttu-id="00d8b-284">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-284">String</span></span>|<span data-ttu-id="00d8b-285">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="00d8b-285">Android security patch level</span></span>|
|<span data-ttu-id="00d8b-286">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="00d8b-286">userDisplayName</span></span>|<span data-ttu-id="00d8b-287">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-287">String</span></span>|<span data-ttu-id="00d8b-288">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="00d8b-288">User display name</span></span>|
|<span data-ttu-id="00d8b-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="00d8b-289">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="00d8b-290">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="00d8b-290">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="00d8b-291">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="00d8b-291">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="00d8b-292">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="00d8b-292">wiFiMacAddress</span></span>|<span data-ttu-id="00d8b-293">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-293">String</span></span>|<span data-ttu-id="00d8b-294">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="00d8b-294">Wi-Fi MAC</span></span>|
|<span data-ttu-id="00d8b-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="00d8b-295">deviceHealthAttestationState</span></span>|[<span data-ttu-id="00d8b-296">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="00d8b-296">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="00d8b-297">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-297">The device health attestation state.</span></span>|
|<span data-ttu-id="00d8b-298">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="00d8b-298">subscriberCarrier</span></span>|<span data-ttu-id="00d8b-299">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-299">String</span></span>|<span data-ttu-id="00d8b-300">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="00d8b-300">Subscriber Carrier</span></span>|
|<span data-ttu-id="00d8b-301">meid</span><span class="sxs-lookup"><span data-stu-id="00d8b-301">meid</span></span>|<span data-ttu-id="00d8b-302">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-302">String</span></span>|<span data-ttu-id="00d8b-303">MEID</span><span class="sxs-lookup"><span data-stu-id="00d8b-303">MEID</span></span>|
|<span data-ttu-id="00d8b-304">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="00d8b-304">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="00d8b-305">Int64</span><span class="sxs-lookup"><span data-stu-id="00d8b-305">Int64</span></span>|<span data-ttu-id="00d8b-306">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="00d8b-306">Total Storage in Bytes</span></span>|
|<span data-ttu-id="00d8b-307">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="00d8b-307">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="00d8b-308">Int64</span><span class="sxs-lookup"><span data-stu-id="00d8b-308">Int64</span></span>|<span data-ttu-id="00d8b-309">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="00d8b-309">Free Storage in Bytes</span></span>|
|<span data-ttu-id="00d8b-310">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="00d8b-310">managedDeviceName</span></span>|<span data-ttu-id="00d8b-311">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-311">String</span></span>|<span data-ttu-id="00d8b-312">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-312">Automatically generated name to identify a device.</span></span> <span data-ttu-id="00d8b-313">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="00d8b-313">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="00d8b-314">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="00d8b-314">partnerReportedThreatState</span></span>|[<span data-ttu-id="00d8b-315">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="00d8b-315">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="00d8b-316">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-316">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="00d8b-317">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00d8b-317">Read Only.</span></span> <span data-ttu-id="00d8b-318">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="00d8b-318">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="00d8b-319">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="00d8b-319">usersLoggedOn</span></span>|<span data-ttu-id="00d8b-320">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="00d8b-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="00d8b-321">Indica o último logon usuários de um dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-321">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="00d8b-322">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="00d8b-322">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="00d8b-323">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-323">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-324">Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="00d8b-324">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="00d8b-325">Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="00d8b-325">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="00d8b-326">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00d8b-326">Read Only.</span></span>|
|<span data-ttu-id="00d8b-327">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="00d8b-327">autopilotEnrolled</span></span>|<span data-ttu-id="00d8b-328">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-328">Boolean</span></span>|<span data-ttu-id="00d8b-329">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="00d8b-329">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="00d8b-330">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="00d8b-330">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="00d8b-331">Booliano</span><span class="sxs-lookup"><span data-stu-id="00d8b-331">Boolean</span></span>|<span data-ttu-id="00d8b-332">Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="00d8b-332">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="00d8b-333">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="00d8b-333">managementCertificateExpirationDate</span></span>|<span data-ttu-id="00d8b-334">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d8b-334">DateTimeOffset</span></span>|<span data-ttu-id="00d8b-335">Relata a data de validade do certificado de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="00d8b-335">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="00d8b-336">iccid</span><span class="sxs-lookup"><span data-stu-id="00d8b-336">iccid</span></span>|<span data-ttu-id="00d8b-337">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-337">String</span></span>|<span data-ttu-id="00d8b-338">Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM.</span><span class="sxs-lookup"><span data-stu-id="00d8b-338">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="00d8b-339">UDID</span><span class="sxs-lookup"><span data-stu-id="00d8b-339">udid</span></span>|<span data-ttu-id="00d8b-340">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-340">String</span></span>|<span data-ttu-id="00d8b-341">Identificador exclusivo do dispositivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="00d8b-341">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="00d8b-342">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00d8b-342">roleScopeTagIds</span></span>|<span data-ttu-id="00d8b-343">String collection</span><span class="sxs-lookup"><span data-stu-id="00d8b-343">String collection</span></span>|<span data-ttu-id="00d8b-344">Lista de IDs de marca de escopo para essa instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00d8b-344">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="00d8b-345">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="00d8b-345">windowsActiveMalwareCount</span></span>|<span data-ttu-id="00d8b-346">Int32</span><span class="sxs-lookup"><span data-stu-id="00d8b-346">Int32</span></span>|<span data-ttu-id="00d8b-347">Contagem de malware ativos para este dispositivo do windows</span><span class="sxs-lookup"><span data-stu-id="00d8b-347">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="00d8b-348">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="00d8b-348">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="00d8b-349">Int32</span><span class="sxs-lookup"><span data-stu-id="00d8b-349">Int32</span></span>|<span data-ttu-id="00d8b-350">Contagem de malware remediados por teste para este dispositivo do windows</span><span class="sxs-lookup"><span data-stu-id="00d8b-350">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="00d8b-351">Observações</span><span class="sxs-lookup"><span data-stu-id="00d8b-351">notes</span></span>|<span data-ttu-id="00d8b-352">String</span><span class="sxs-lookup"><span data-stu-id="00d8b-352">String</span></span>|<span data-ttu-id="00d8b-353">Anotações no dispositivo criado pelo administrador de TI</span><span class="sxs-lookup"><span data-stu-id="00d8b-353">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="00d8b-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="00d8b-354">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="00d8b-355">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="00d8b-355">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="00d8b-356">Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados por agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="00d8b-356">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="00d8b-357">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d8b-357">Response</span></span>
<span data-ttu-id="00d8b-358">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00d8b-358">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00d8b-359">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00d8b-359">Example</span></span>
### <a name="request"></a><span data-ttu-id="00d8b-360">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00d8b-360">Request</span></span>
<span data-ttu-id="00d8b-361">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00d8b-361">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7114

{
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a><span data-ttu-id="00d8b-362">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d8b-362">Response</span></span>
<span data-ttu-id="00d8b-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00d8b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7215

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```





