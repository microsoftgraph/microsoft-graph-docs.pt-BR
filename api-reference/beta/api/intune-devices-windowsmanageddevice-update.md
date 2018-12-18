---
title: Atualizar windowsManagedDevice
description: Atualize as propriedades de um objeto windowsManagedDevice.
author: tfitzmac
ms.openlocfilehash: d1aa637a513d45ad33a1a5990399cf35f4cb21ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347632"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="440fc-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="440fc-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="440fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="440fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="440fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="440fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="440fc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="440fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="440fc-107">Atualize as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="440fc-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="440fc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="440fc-108">Prerequisites</span></span>
<span data-ttu-id="440fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="440fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="440fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="440fc-111">Permission type</span></span>|<span data-ttu-id="440fc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="440fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="440fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="440fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="440fc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="440fc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="440fc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="440fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="440fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="440fc-116">Not supported.</span></span>|
|<span data-ttu-id="440fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="440fc-117">Application</span></span>|<span data-ttu-id="440fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="440fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="440fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="440fc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="440fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="440fc-120">Request headers</span></span>
|<span data-ttu-id="440fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="440fc-121">Header</span></span>|<span data-ttu-id="440fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="440fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="440fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="440fc-123">Authorization</span></span>|<span data-ttu-id="440fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="440fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="440fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="440fc-125">Accept</span></span>|<span data-ttu-id="440fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="440fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="440fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="440fc-127">Request body</span></span>
<span data-ttu-id="440fc-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="440fc-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="440fc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="440fc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="440fc-130">Property</span></span>|<span data-ttu-id="440fc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="440fc-131">Type</span></span>|<span data-ttu-id="440fc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="440fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="440fc-133">id</span><span class="sxs-lookup"><span data-stu-id="440fc-133">id</span></span>|<span data-ttu-id="440fc-134">String</span><span class="sxs-lookup"><span data-stu-id="440fc-134">String</span></span>|<span data-ttu-id="440fc-135">Identificador exclusivo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-136">userId</span><span class="sxs-lookup"><span data-stu-id="440fc-136">userId</span></span>|<span data-ttu-id="440fc-137">String</span><span class="sxs-lookup"><span data-stu-id="440fc-137">String</span></span>|<span data-ttu-id="440fc-138">Identificador exclusivo para o usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="440fc-139">deviceName</span></span>|<span data-ttu-id="440fc-140">String</span><span class="sxs-lookup"><span data-stu-id="440fc-140">String</span></span>|<span data-ttu-id="440fc-141">Nome do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="440fc-142">hardwareInformation</span></span>|[<span data-ttu-id="440fc-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="440fc-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="440fc-144">Os detalhes de hardware do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-144">The hardward details for the device.</span></span>  <span data-ttu-id="440fc-145">Inclui informações como o espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="440fc-146">ownerType</span></span>|[<span data-ttu-id="440fc-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="440fc-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="440fc-148">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-148">Ownership of the device.</span></span> <span data-ttu-id="440fc-149">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="440fc-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="440fc-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="440fc-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="440fc-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="440fc-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="440fc-153">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-153">Ownership of the device.</span></span> <span data-ttu-id="440fc-154">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-155">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="440fc-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="440fc-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="440fc-156">deviceActionResults</span></span>|<span data-ttu-id="440fc-157">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="440fc-158">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="440fc-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="440fc-159">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-160">managementState</span><span class="sxs-lookup"><span data-stu-id="440fc-160">managementState</span></span>|[<span data-ttu-id="440fc-161">managementState</span><span class="sxs-lookup"><span data-stu-id="440fc-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="440fc-162">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-162">Management state of the device.</span></span> <span data-ttu-id="440fc-163">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-164">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="440fc-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="440fc-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="440fc-165">enrolledDateTime</span></span>|<span data-ttu-id="440fc-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-166">DateTimeOffset</span></span>|<span data-ttu-id="440fc-167">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-167">Enrollment time of the device.</span></span> <span data-ttu-id="440fc-168">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="440fc-169">lastSyncDateTime</span></span>|<span data-ttu-id="440fc-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-170">DateTimeOffset</span></span>|<span data-ttu-id="440fc-171">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="440fc-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="440fc-172">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="440fc-173">chassisType</span></span>|[<span data-ttu-id="440fc-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="440fc-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="440fc-175">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-175">Chassis type of the device.</span></span> <span data-ttu-id="440fc-176">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-177">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="440fc-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="440fc-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="440fc-178">operatingSystem</span></span>|<span data-ttu-id="440fc-179">String</span><span class="sxs-lookup"><span data-stu-id="440fc-179">String</span></span>|<span data-ttu-id="440fc-180">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-180">Operating system of the device.</span></span> <span data-ttu-id="440fc-181">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="440fc-182">deviceType</span></span>|[<span data-ttu-id="440fc-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="440fc-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="440fc-184">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-184">Platform of the device.</span></span> <span data-ttu-id="440fc-185">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-186">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="440fc-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="440fc-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="440fc-187">complianceState</span></span>|[<span data-ttu-id="440fc-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="440fc-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="440fc-189">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-189">Compliance state of the device.</span></span> <span data-ttu-id="440fc-190">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-191">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="440fc-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="440fc-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="440fc-192">jailBroken</span></span>|<span data-ttu-id="440fc-193">String</span><span class="sxs-lookup"><span data-stu-id="440fc-193">String</span></span>|<span data-ttu-id="440fc-194">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="440fc-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="440fc-195">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="440fc-196">managementAgent</span></span>|[<span data-ttu-id="440fc-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="440fc-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="440fc-198">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-198">Management channel of the device.</span></span> <span data-ttu-id="440fc-199">Intune, EAS, etc. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-200">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="440fc-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="440fc-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="440fc-201">osVersion</span></span>|<span data-ttu-id="440fc-202">String</span><span class="sxs-lookup"><span data-stu-id="440fc-202">String</span></span>|<span data-ttu-id="440fc-203">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-203">Operating system version of the device.</span></span> <span data-ttu-id="440fc-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="440fc-205">easActivated</span></span>|<span data-ttu-id="440fc-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-206">Boolean</span></span>|<span data-ttu-id="440fc-207">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="440fc-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="440fc-208">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="440fc-209">easDeviceId</span></span>|<span data-ttu-id="440fc-210">String</span><span class="sxs-lookup"><span data-stu-id="440fc-210">String</span></span>|<span data-ttu-id="440fc-211">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="440fc-212">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="440fc-213">easActivationDateTime</span></span>|<span data-ttu-id="440fc-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-214">DateTimeOffset</span></span>|<span data-ttu-id="440fc-215">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="440fc-216">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="440fc-217">aadRegistered</span></span>|<span data-ttu-id="440fc-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-218">Boolean</span></span>|<span data-ttu-id="440fc-219">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="440fc-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="440fc-220">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="440fc-221">azureADRegistered</span></span>|<span data-ttu-id="440fc-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-222">Boolean</span></span>|<span data-ttu-id="440fc-223">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="440fc-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="440fc-224">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="440fc-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="440fc-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="440fc-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="440fc-227">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-227">Enrollment type of the device.</span></span> <span data-ttu-id="440fc-228">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-229">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="440fc-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="440fc-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="440fc-230">lostModeState</span></span>|[<span data-ttu-id="440fc-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="440fc-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="440fc-232">Indica se o modo perdido está habilitado ou desabilitada Inherited em [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-233">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="440fc-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="440fc-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="440fc-234">activationLockBypassCode</span></span>|<span data-ttu-id="440fc-235">String</span><span class="sxs-lookup"><span data-stu-id="440fc-235">String</span></span>|<span data-ttu-id="440fc-236">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="440fc-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="440fc-237">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="440fc-238">emailAddress</span></span>|<span data-ttu-id="440fc-239">String</span><span class="sxs-lookup"><span data-stu-id="440fc-239">String</span></span>|<span data-ttu-id="440fc-240">O usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md) email(s)</span><span class="sxs-lookup"><span data-stu-id="440fc-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="440fc-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="440fc-242">String</span><span class="sxs-lookup"><span data-stu-id="440fc-242">String</span></span>|<span data-ttu-id="440fc-243">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="440fc-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="440fc-244">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="440fc-244">Read only.</span></span> <span data-ttu-id="440fc-245">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="440fc-246">azureADDeviceId</span></span>|<span data-ttu-id="440fc-247">String</span><span class="sxs-lookup"><span data-stu-id="440fc-247">String</span></span>|<span data-ttu-id="440fc-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="440fc-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="440fc-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="440fc-249">Read only.</span></span> <span data-ttu-id="440fc-250">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="440fc-251">deviceRegistrationState</span></span>|[<span data-ttu-id="440fc-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="440fc-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="440fc-253">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-253">Device registration state.</span></span> <span data-ttu-id="440fc-254">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-255">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="440fc-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="440fc-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="440fc-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="440fc-257">String</span><span class="sxs-lookup"><span data-stu-id="440fc-257">String</span></span>|<span data-ttu-id="440fc-258">Nome de exibição de categoria dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="440fc-259">isSupervised</span></span>|<span data-ttu-id="440fc-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-260">Boolean</span></span>|<span data-ttu-id="440fc-261">Status do dispositivo supervisionado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="440fc-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="440fc-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-263">DateTimeOffset</span></span>|<span data-ttu-id="440fc-264">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="440fc-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="440fc-265">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="440fc-266">exchangeAccessState</span></span>|[<span data-ttu-id="440fc-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="440fc-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="440fc-268">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="440fc-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="440fc-269">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-270">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="440fc-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="440fc-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="440fc-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="440fc-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="440fc-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="440fc-273">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="440fc-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="440fc-274">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-275">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="440fc-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="440fc-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="440fc-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="440fc-277">String</span><span class="sxs-lookup"><span data-stu-id="440fc-277">String</span></span>|<span data-ttu-id="440fc-278">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="440fc-279">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="440fc-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="440fc-281">String</span><span class="sxs-lookup"><span data-stu-id="440fc-281">String</span></span>|<span data-ttu-id="440fc-282">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="440fc-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="440fc-283">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="440fc-284">isEncrypted</span></span>|<span data-ttu-id="440fc-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-285">Boolean</span></span>|<span data-ttu-id="440fc-286">Status de criptografia do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="440fc-287">userPrincipalName</span></span>|<span data-ttu-id="440fc-288">String</span><span class="sxs-lookup"><span data-stu-id="440fc-288">String</span></span>|<span data-ttu-id="440fc-289">Dispositivo nome principal de usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-290">modelo</span><span class="sxs-lookup"><span data-stu-id="440fc-290">model</span></span>|<span data-ttu-id="440fc-291">String</span><span class="sxs-lookup"><span data-stu-id="440fc-291">String</span></span>|<span data-ttu-id="440fc-292">Modelo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-293">fabricante</span><span class="sxs-lookup"><span data-stu-id="440fc-293">manufacturer</span></span>|<span data-ttu-id="440fc-294">String</span><span class="sxs-lookup"><span data-stu-id="440fc-294">String</span></span>|<span data-ttu-id="440fc-295">Fabricante do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-296">imei</span><span class="sxs-lookup"><span data-stu-id="440fc-296">imei</span></span>|<span data-ttu-id="440fc-297">String</span><span class="sxs-lookup"><span data-stu-id="440fc-297">String</span></span>|<span data-ttu-id="440fc-298">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="440fc-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="440fc-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-300">DateTimeOffset</span></span>|<span data-ttu-id="440fc-301">A data e hora quando o período de carência de conformidade do dispositivo expiram Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="440fc-302">serialNumber</span></span>|<span data-ttu-id="440fc-303">String</span><span class="sxs-lookup"><span data-stu-id="440fc-303">String</span></span>|<span data-ttu-id="440fc-304">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="440fc-305">phoneNumber</span></span>|<span data-ttu-id="440fc-306">String</span><span class="sxs-lookup"><span data-stu-id="440fc-306">String</span></span>|<span data-ttu-id="440fc-307">Número de telefone do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="440fc-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="440fc-309">String</span><span class="sxs-lookup"><span data-stu-id="440fc-309">String</span></span>|<span data-ttu-id="440fc-310">Nível de patch de segurança Android Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="440fc-311">userDisplayName</span></span>|<span data-ttu-id="440fc-312">String</span><span class="sxs-lookup"><span data-stu-id="440fc-312">String</span></span>|<span data-ttu-id="440fc-313">Nome de exibição do usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="440fc-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="440fc-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="440fc-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="440fc-316">Cliente de ConfigrMgr habilitado recursos Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="440fc-317">wiFiMacAddress</span></span>|<span data-ttu-id="440fc-318">String</span><span class="sxs-lookup"><span data-stu-id="440fc-318">String</span></span>|<span data-ttu-id="440fc-319">Wi-Fi MAC herdada do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="440fc-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="440fc-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="440fc-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="440fc-322">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-322">The device health attestation state.</span></span> <span data-ttu-id="440fc-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="440fc-324">subscriberCarrier</span></span>|<span data-ttu-id="440fc-325">String</span><span class="sxs-lookup"><span data-stu-id="440fc-325">String</span></span>|<span data-ttu-id="440fc-326">Herdado de operadora de assinante de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-327">meid</span><span class="sxs-lookup"><span data-stu-id="440fc-327">meid</span></span>|<span data-ttu-id="440fc-328">String</span><span class="sxs-lookup"><span data-stu-id="440fc-328">String</span></span>|<span data-ttu-id="440fc-329">MEID herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="440fc-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="440fc-331">Int64</span><span class="sxs-lookup"><span data-stu-id="440fc-331">Int64</span></span>|<span data-ttu-id="440fc-332">Armazenamento total em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="440fc-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="440fc-334">Int64</span><span class="sxs-lookup"><span data-stu-id="440fc-334">Int64</span></span>|<span data-ttu-id="440fc-335">Armazenamento gratuito em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="440fc-336">managedDeviceName</span></span>|<span data-ttu-id="440fc-337">String</span><span class="sxs-lookup"><span data-stu-id="440fc-337">String</span></span>|<span data-ttu-id="440fc-338">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="440fc-339">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="440fc-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="440fc-340">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="440fc-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="440fc-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="440fc-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="440fc-343">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="440fc-344">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="440fc-344">Read Only.</span></span> <span data-ttu-id="440fc-345">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="440fc-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="440fc-346">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="440fc-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="440fc-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="440fc-347">usersLoggedOn</span></span>|<span data-ttu-id="440fc-348">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="440fc-349">Indica o último logon usuários de um dispositivo Inherited da [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="440fc-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="440fc-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-351">DateTimeOffset</span></span>|<span data-ttu-id="440fc-352">Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="440fc-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="440fc-353">Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="440fc-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="440fc-354">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="440fc-354">Read Only.</span></span> <span data-ttu-id="440fc-355">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="440fc-356">autopilotEnrolled</span></span>|<span data-ttu-id="440fc-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-357">Boolean</span></span>|<span data-ttu-id="440fc-358">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="440fc-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="440fc-359">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="440fc-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="440fc-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="440fc-361">Boolean</span></span>|<span data-ttu-id="440fc-362">Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="440fc-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="440fc-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="440fc-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="440fc-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="440fc-365">DateTimeOffset</span></span>|<span data-ttu-id="440fc-366">Relatórios de dispositivo gerenciamento data de validade certificado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-367">iccid</span><span class="sxs-lookup"><span data-stu-id="440fc-367">iccid</span></span>|<span data-ttu-id="440fc-368">String</span><span class="sxs-lookup"><span data-stu-id="440fc-368">String</span></span>|<span data-ttu-id="440fc-369">Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM.</span><span class="sxs-lookup"><span data-stu-id="440fc-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="440fc-370">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-371">UDID</span><span class="sxs-lookup"><span data-stu-id="440fc-371">udid</span></span>|<span data-ttu-id="440fc-372">String</span><span class="sxs-lookup"><span data-stu-id="440fc-372">String</span></span>|<span data-ttu-id="440fc-373">Identificador exclusivo do dispositivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="440fc-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="440fc-374">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="440fc-375">roleScopeTagIds</span></span>|<span data-ttu-id="440fc-376">String collection</span><span class="sxs-lookup"><span data-stu-id="440fc-376">String collection</span></span>|<span data-ttu-id="440fc-377">Lista de IDs de marca de escopo para essa instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="440fc-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="440fc-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="440fc-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="440fc-380">Int32</span><span class="sxs-lookup"><span data-stu-id="440fc-380">Int32</span></span>|<span data-ttu-id="440fc-381">Contagem de malware ativos para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="440fc-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="440fc-383">Int32</span><span class="sxs-lookup"><span data-stu-id="440fc-383">Int32</span></span>|<span data-ttu-id="440fc-384">Contagem de malware remediados por teste para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-385">Observações</span><span class="sxs-lookup"><span data-stu-id="440fc-385">notes</span></span>|<span data-ttu-id="440fc-386">String</span><span class="sxs-lookup"><span data-stu-id="440fc-386">String</span></span>|<span data-ttu-id="440fc-387">Anotações no dispositivo criados pelo administrador de TI herdadas a partir do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="440fc-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="440fc-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="440fc-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="440fc-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="440fc-390">Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados pelo MDM/ConfigMgr herdadas de agente do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="440fc-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="440fc-391">Resposta</span><span class="sxs-lookup"><span data-stu-id="440fc-391">Response</span></span>
<span data-ttu-id="440fc-392">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="440fc-392">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="440fc-393">Exemplo</span><span class="sxs-lookup"><span data-stu-id="440fc-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="440fc-394">Solicitação</span><span class="sxs-lookup"><span data-stu-id="440fc-394">Request</span></span>
<span data-ttu-id="440fc-395">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="440fc-395">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="440fc-396">Resposta</span><span class="sxs-lookup"><span data-stu-id="440fc-396">Response</span></span>
<span data-ttu-id="440fc-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="440fc-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





