---
title: Criar windowsManagedDevice
description: Crie um novo objeto de windowsManagedDevice.
ms.openlocfilehash: 79db6b0f2d5f8e918b42fb9b1c5a40b05983edae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036915"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="6a70a-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="6a70a-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="6a70a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a70a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a70a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a70a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a70a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a70a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a70a-107">Crie um novo objeto de [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="6a70a-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a70a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a70a-108">Prerequisites</span></span>
<span data-ttu-id="6a70a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a70a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a70a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a70a-111">Permission type</span></span>|<span data-ttu-id="6a70a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a70a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a70a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a70a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a70a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a70a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6a70a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a70a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a70a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a70a-116">Not supported.</span></span>|
|<span data-ttu-id="6a70a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a70a-117">Application</span></span>|<span data-ttu-id="6a70a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a70a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a70a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a70a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="6a70a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a70a-120">Request headers</span></span>
|<span data-ttu-id="6a70a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a70a-121">Header</span></span>|<span data-ttu-id="6a70a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a70a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a70a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a70a-123">Authorization</span></span>|<span data-ttu-id="6a70a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a70a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a70a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a70a-125">Accept</span></span>|<span data-ttu-id="6a70a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a70a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a70a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a70a-127">Request body</span></span>
<span data-ttu-id="6a70a-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="6a70a-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="6a70a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="6a70a-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="6a70a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a70a-130">Property</span></span>|<span data-ttu-id="6a70a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a70a-131">Type</span></span>|<span data-ttu-id="6a70a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a70a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a70a-133">id</span><span class="sxs-lookup"><span data-stu-id="6a70a-133">id</span></span>|<span data-ttu-id="6a70a-134">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-134">String</span></span>|<span data-ttu-id="6a70a-135">Identificador exclusivo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-136">userId</span><span class="sxs-lookup"><span data-stu-id="6a70a-136">userId</span></span>|<span data-ttu-id="6a70a-137">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-137">String</span></span>|<span data-ttu-id="6a70a-138">Identificador exclusivo para o usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="6a70a-139">deviceName</span></span>|<span data-ttu-id="6a70a-140">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-140">String</span></span>|<span data-ttu-id="6a70a-141">Nome do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="6a70a-142">hardwareInformation</span></span>|[<span data-ttu-id="6a70a-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="6a70a-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="6a70a-144">Os detalhes de hardware do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-144">The hardward details for the device.</span></span>  <span data-ttu-id="6a70a-145">Inclui informações como o espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="6a70a-146">ownerType</span></span>|[<span data-ttu-id="6a70a-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="6a70a-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="6a70a-148">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-148">Ownership of the device.</span></span> <span data-ttu-id="6a70a-149">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="6a70a-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="6a70a-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="6a70a-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="6a70a-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="6a70a-153">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-153">Ownership of the device.</span></span> <span data-ttu-id="6a70a-154">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-155">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="6a70a-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="6a70a-156">deviceActionResults</span></span>|<span data-ttu-id="6a70a-157">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="6a70a-158">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="6a70a-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="6a70a-159">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-160">managementState</span><span class="sxs-lookup"><span data-stu-id="6a70a-160">managementState</span></span>|[<span data-ttu-id="6a70a-161">managementState</span><span class="sxs-lookup"><span data-stu-id="6a70a-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="6a70a-162">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-162">Management state of the device.</span></span> <span data-ttu-id="6a70a-163">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-164">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="6a70a-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="6a70a-165">enrolledDateTime</span></span>|<span data-ttu-id="6a70a-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-166">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-167">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-167">Enrollment time of the device.</span></span> <span data-ttu-id="6a70a-168">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6a70a-169">lastSyncDateTime</span></span>|<span data-ttu-id="6a70a-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-170">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-171">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="6a70a-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="6a70a-172">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="6a70a-173">chassisType</span></span>|[<span data-ttu-id="6a70a-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="6a70a-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="6a70a-175">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-175">Chassis type of the device.</span></span> <span data-ttu-id="6a70a-176">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-177">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="6a70a-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a70a-178">operatingSystem</span></span>|<span data-ttu-id="6a70a-179">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-179">String</span></span>|<span data-ttu-id="6a70a-180">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-180">Operating system of the device.</span></span> <span data-ttu-id="6a70a-181">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="6a70a-182">deviceType</span></span>|[<span data-ttu-id="6a70a-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="6a70a-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6a70a-184">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-184">Platform of the device.</span></span> <span data-ttu-id="6a70a-185">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-186">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6a70a-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="6a70a-187">complianceState</span></span>|[<span data-ttu-id="6a70a-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="6a70a-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="6a70a-189">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-189">Compliance state of the device.</span></span> <span data-ttu-id="6a70a-190">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-191">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="6a70a-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="6a70a-192">jailBroken</span></span>|<span data-ttu-id="6a70a-193">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-193">String</span></span>|<span data-ttu-id="6a70a-194">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="6a70a-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="6a70a-195">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="6a70a-196">managementAgent</span></span>|[<span data-ttu-id="6a70a-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="6a70a-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="6a70a-198">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-198">Management channel of the device.</span></span> <span data-ttu-id="6a70a-199">Intune, EAS, etc. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-200">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="6a70a-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="6a70a-201">osVersion</span></span>|<span data-ttu-id="6a70a-202">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-202">String</span></span>|<span data-ttu-id="6a70a-203">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-203">Operating system version of the device.</span></span> <span data-ttu-id="6a70a-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="6a70a-205">easActivated</span></span>|<span data-ttu-id="6a70a-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-206">Boolean</span></span>|<span data-ttu-id="6a70a-207">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="6a70a-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="6a70a-208">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="6a70a-209">easDeviceId</span></span>|<span data-ttu-id="6a70a-210">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-210">String</span></span>|<span data-ttu-id="6a70a-211">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="6a70a-212">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="6a70a-213">easActivationDateTime</span></span>|<span data-ttu-id="6a70a-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-214">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-215">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="6a70a-216">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="6a70a-217">aadRegistered</span></span>|<span data-ttu-id="6a70a-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-218">Boolean</span></span>|<span data-ttu-id="6a70a-219">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a70a-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="6a70a-220">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="6a70a-221">azureADRegistered</span></span>|<span data-ttu-id="6a70a-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-222">Boolean</span></span>|<span data-ttu-id="6a70a-223">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a70a-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="6a70a-224">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="6a70a-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="6a70a-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="6a70a-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="6a70a-227">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-227">Enrollment type of the device.</span></span> <span data-ttu-id="6a70a-228">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-229">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="6a70a-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="6a70a-230">lostModeState</span></span>|[<span data-ttu-id="6a70a-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="6a70a-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="6a70a-232">Indica se o modo perdido está habilitado ou desabilitada Inherited em [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-233">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="6a70a-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="6a70a-234">activationLockBypassCode</span></span>|<span data-ttu-id="6a70a-235">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-235">String</span></span>|<span data-ttu-id="6a70a-236">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="6a70a-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="6a70a-237">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6a70a-238">emailAddress</span></span>|<span data-ttu-id="6a70a-239">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-239">String</span></span>|<span data-ttu-id="6a70a-240">O usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md) email(s)</span><span class="sxs-lookup"><span data-stu-id="6a70a-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="6a70a-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="6a70a-242">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-242">String</span></span>|<span data-ttu-id="6a70a-243">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a70a-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="6a70a-244">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a70a-244">Read only.</span></span> <span data-ttu-id="6a70a-245">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="6a70a-246">azureADDeviceId</span></span>|<span data-ttu-id="6a70a-247">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-247">String</span></span>|<span data-ttu-id="6a70a-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a70a-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="6a70a-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a70a-249">Read only.</span></span> <span data-ttu-id="6a70a-250">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6a70a-251">deviceRegistrationState</span></span>|[<span data-ttu-id="6a70a-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="6a70a-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="6a70a-253">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-253">Device registration state.</span></span> <span data-ttu-id="6a70a-254">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-255">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="6a70a-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a70a-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="6a70a-257">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-257">String</span></span>|<span data-ttu-id="6a70a-258">Nome de exibição de categoria dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="6a70a-259">isSupervised</span></span>|<span data-ttu-id="6a70a-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-260">Boolean</span></span>|<span data-ttu-id="6a70a-261">Status do dispositivo supervisionado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6a70a-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="6a70a-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-263">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-264">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a70a-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="6a70a-265">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="6a70a-266">exchangeAccessState</span></span>|[<span data-ttu-id="6a70a-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="6a70a-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="6a70a-268">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a70a-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="6a70a-269">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-270">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="6a70a-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="6a70a-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="6a70a-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="6a70a-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="6a70a-273">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a70a-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="6a70a-274">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-275">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="6a70a-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="6a70a-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="6a70a-277">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-277">String</span></span>|<span data-ttu-id="6a70a-278">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="6a70a-279">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="6a70a-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="6a70a-281">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-281">String</span></span>|<span data-ttu-id="6a70a-282">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="6a70a-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="6a70a-283">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="6a70a-284">isEncrypted</span></span>|<span data-ttu-id="6a70a-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-285">Boolean</span></span>|<span data-ttu-id="6a70a-286">Status de criptografia do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a70a-287">userPrincipalName</span></span>|<span data-ttu-id="6a70a-288">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-288">String</span></span>|<span data-ttu-id="6a70a-289">Dispositivo nome principal de usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-290">modelo</span><span class="sxs-lookup"><span data-stu-id="6a70a-290">model</span></span>|<span data-ttu-id="6a70a-291">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-291">String</span></span>|<span data-ttu-id="6a70a-292">Modelo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-293">fabricante</span><span class="sxs-lookup"><span data-stu-id="6a70a-293">manufacturer</span></span>|<span data-ttu-id="6a70a-294">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-294">String</span></span>|<span data-ttu-id="6a70a-295">Fabricante do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-296">imei</span><span class="sxs-lookup"><span data-stu-id="6a70a-296">imei</span></span>|<span data-ttu-id="6a70a-297">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-297">String</span></span>|<span data-ttu-id="6a70a-298">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6a70a-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6a70a-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-300">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-301">A data e hora quando o período de carência de conformidade do dispositivo expiram Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6a70a-302">serialNumber</span></span>|<span data-ttu-id="6a70a-303">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-303">String</span></span>|<span data-ttu-id="6a70a-304">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="6a70a-305">phoneNumber</span></span>|<span data-ttu-id="6a70a-306">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-306">String</span></span>|<span data-ttu-id="6a70a-307">Número de telefone do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6a70a-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="6a70a-309">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-309">String</span></span>|<span data-ttu-id="6a70a-310">Nível de patch de segurança Android Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a70a-311">userDisplayName</span></span>|<span data-ttu-id="6a70a-312">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-312">String</span></span>|<span data-ttu-id="6a70a-313">Nome de exibição do usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="6a70a-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="6a70a-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="6a70a-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="6a70a-316">Cliente de ConfigrMgr habilitado recursos Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="6a70a-317">wiFiMacAddress</span></span>|<span data-ttu-id="6a70a-318">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-318">String</span></span>|<span data-ttu-id="6a70a-319">Wi-Fi MAC herdada do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="6a70a-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="6a70a-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="6a70a-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="6a70a-322">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-322">The device health attestation state.</span></span> <span data-ttu-id="6a70a-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="6a70a-324">subscriberCarrier</span></span>|<span data-ttu-id="6a70a-325">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-325">String</span></span>|<span data-ttu-id="6a70a-326">Herdado de operadora de assinante de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-327">meid</span><span class="sxs-lookup"><span data-stu-id="6a70a-327">meid</span></span>|<span data-ttu-id="6a70a-328">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-328">String</span></span>|<span data-ttu-id="6a70a-329">MEID herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="6a70a-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="6a70a-331">Int64</span><span class="sxs-lookup"><span data-stu-id="6a70a-331">Int64</span></span>|<span data-ttu-id="6a70a-332">Armazenamento total em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="6a70a-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="6a70a-334">Int64</span><span class="sxs-lookup"><span data-stu-id="6a70a-334">Int64</span></span>|<span data-ttu-id="6a70a-335">Armazenamento gratuito em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="6a70a-336">managedDeviceName</span></span>|<span data-ttu-id="6a70a-337">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-337">String</span></span>|<span data-ttu-id="6a70a-338">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="6a70a-339">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="6a70a-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="6a70a-340">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="6a70a-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="6a70a-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="6a70a-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="6a70a-343">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="6a70a-344">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a70a-344">Read Only.</span></span> <span data-ttu-id="6a70a-345">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="6a70a-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="6a70a-346">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="6a70a-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="6a70a-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="6a70a-347">usersLoggedOn</span></span>|<span data-ttu-id="6a70a-348">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="6a70a-349">Indica o último logon usuários de um dispositivo Inherited da [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a70a-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="6a70a-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-351">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-352">Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="6a70a-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="6a70a-353">Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="6a70a-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="6a70a-354">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a70a-354">Read Only.</span></span> <span data-ttu-id="6a70a-355">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="6a70a-356">autopilotEnrolled</span></span>|<span data-ttu-id="6a70a-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-357">Boolean</span></span>|<span data-ttu-id="6a70a-358">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="6a70a-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="6a70a-359">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="6a70a-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="6a70a-361">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a70a-361">Boolean</span></span>|<span data-ttu-id="6a70a-362">Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="6a70a-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="6a70a-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6a70a-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="6a70a-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a70a-365">DateTimeOffset</span></span>|<span data-ttu-id="6a70a-366">Relatórios de dispositivo gerenciamento data de validade certificado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-367">iccid</span><span class="sxs-lookup"><span data-stu-id="6a70a-367">iccid</span></span>|<span data-ttu-id="6a70a-368">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-368">String</span></span>|<span data-ttu-id="6a70a-369">Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM.</span><span class="sxs-lookup"><span data-stu-id="6a70a-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="6a70a-370">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-371">UDID</span><span class="sxs-lookup"><span data-stu-id="6a70a-371">udid</span></span>|<span data-ttu-id="6a70a-372">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-372">String</span></span>|<span data-ttu-id="6a70a-373">Identificador exclusivo do dispositivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="6a70a-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="6a70a-374">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a70a-375">roleScopeTagIds</span></span>|<span data-ttu-id="6a70a-376">String collection</span><span class="sxs-lookup"><span data-stu-id="6a70a-376">String collection</span></span>|<span data-ttu-id="6a70a-377">Lista de IDs de marca de escopo para essa instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a70a-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="6a70a-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="6a70a-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="6a70a-380">Int32</span><span class="sxs-lookup"><span data-stu-id="6a70a-380">Int32</span></span>|<span data-ttu-id="6a70a-381">Contagem de malware ativos para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="6a70a-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="6a70a-383">Int32</span><span class="sxs-lookup"><span data-stu-id="6a70a-383">Int32</span></span>|<span data-ttu-id="6a70a-384">Contagem de malware remediados por teste para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-385">Observações</span><span class="sxs-lookup"><span data-stu-id="6a70a-385">notes</span></span>|<span data-ttu-id="6a70a-386">String</span><span class="sxs-lookup"><span data-stu-id="6a70a-386">String</span></span>|<span data-ttu-id="6a70a-387">Anotações no dispositivo criados pelo administrador de TI herdadas a partir do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="6a70a-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="6a70a-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="6a70a-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="6a70a-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="6a70a-390">Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados pelo MDM/ConfigMgr herdadas de agente do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="6a70a-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6a70a-391">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a70a-391">Response</span></span>
<span data-ttu-id="6a70a-392">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a70a-392">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a70a-393">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a70a-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a70a-394">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a70a-394">Request</span></span>
<span data-ttu-id="6a70a-395">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a70a-395">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7173

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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

### <a name="response"></a><span data-ttu-id="6a70a-396">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a70a-396">Response</span></span>
<span data-ttu-id="6a70a-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a70a-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7222

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
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





