---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af0b6c6f63df6c0575ce5d3901f3e77720d7943b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159686"
---
# <a name="update-manageddevice"></a><span data-ttu-id="45c3a-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="45c3a-103">Update managedDevice</span></span>

<span data-ttu-id="45c3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45c3a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45c3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45c3a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45c3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45c3a-107">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="45c3a-107">Update the properties of a [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45c3a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45c3a-108">Prerequisites</span></span>
<span data-ttu-id="45c3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c3a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45c3a-111">Permission type</span></span>|<span data-ttu-id="45c3a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45c3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45c3a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45c3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45c3a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c3a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="45c3a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45c3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45c3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45c3a-116">Not supported.</span></span>|
|<span data-ttu-id="45c3a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45c3a-117">Application</span></span>|<span data-ttu-id="45c3a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c3a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45c3a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45c3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/comanagedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="45c3a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45c3a-120">Request headers</span></span>
|<span data-ttu-id="45c3a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45c3a-121">Header</span></span>|<span data-ttu-id="45c3a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45c3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45c3a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45c3a-123">Authorization</span></span>|<span data-ttu-id="45c3a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45c3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45c3a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45c3a-125">Accept</span></span>|<span data-ttu-id="45c3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45c3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45c3a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45c3a-127">Request body</span></span>
<span data-ttu-id="45c3a-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="45c3a-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

<span data-ttu-id="45c3a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="45c3a-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-shared-manageddevice.md).</span></span>

|<span data-ttu-id="45c3a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45c3a-130">Property</span></span>|<span data-ttu-id="45c3a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45c3a-131">Type</span></span>|<span data-ttu-id="45c3a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45c3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45c3a-133">id</span><span class="sxs-lookup"><span data-stu-id="45c3a-133">id</span></span>|<span data-ttu-id="45c3a-134">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-134">String</span></span>|<span data-ttu-id="45c3a-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-135">Unique Identifier for the device.</span></span> <span data-ttu-id="45c3a-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-136">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-137">userId</span><span class="sxs-lookup"><span data-stu-id="45c3a-137">userId</span></span>|<span data-ttu-id="45c3a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45c3a-138">String</span></span>|<span data-ttu-id="45c3a-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="45c3a-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-140">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="45c3a-141">deviceName</span></span>|<span data-ttu-id="45c3a-142">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-142">String</span></span>|<span data-ttu-id="45c3a-143">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-143">Name of the device.</span></span> <span data-ttu-id="45c3a-144">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-144">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="45c3a-145">hardwareInformation</span></span>|[<span data-ttu-id="45c3a-146">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="45c3a-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="45c3a-147">Os detalhes rígidos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-147">The hardward details for the device.</span></span>  <span data-ttu-id="45c3a-148">Inclui informações como espaço de armazenamento, fabricante, número de série etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="45c3a-149">ownerType</span></span>|[<span data-ttu-id="45c3a-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="45c3a-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="45c3a-151">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-151">Ownership of the device.</span></span> <span data-ttu-id="45c3a-152">Pode ser 'empresa' ou 'pessoal'.</span><span class="sxs-lookup"><span data-stu-id="45c3a-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="45c3a-153">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="45c3a-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="45c3a-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="45c3a-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="45c3a-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="45c3a-156">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-156">Ownership of the device.</span></span> <span data-ttu-id="45c3a-157">Pode ser 'empresa' ou 'pessoal'.</span><span class="sxs-lookup"><span data-stu-id="45c3a-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="45c3a-158">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="45c3a-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="45c3a-159">deviceActionResults</span></span>|<span data-ttu-id="45c3a-160">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="45c3a-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="45c3a-161">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="45c3a-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="45c3a-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-162">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-163">managementState</span><span class="sxs-lookup"><span data-stu-id="45c3a-163">managementState</span></span>|[<span data-ttu-id="45c3a-164">managementState</span><span class="sxs-lookup"><span data-stu-id="45c3a-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="45c3a-165">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-165">Management state of the device.</span></span> <span data-ttu-id="45c3a-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-166">This property is read-only.</span></span> <span data-ttu-id="45c3a-167">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="45c3a-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-168">enrolledDateTime</span></span>|<span data-ttu-id="45c3a-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-169">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-170">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-170">Enrollment time of the device.</span></span> <span data-ttu-id="45c3a-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-171">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-172">lastSyncDateTime</span></span>|<span data-ttu-id="45c3a-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-173">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-174">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="45c3a-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="45c3a-175">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-175">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="45c3a-176">chassisType</span></span>|[<span data-ttu-id="45c3a-177">chassisType</span><span class="sxs-lookup"><span data-stu-id="45c3a-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="45c3a-178">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-178">Chassis type of the device.</span></span> <span data-ttu-id="45c3a-179">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-179">This property is read-only.</span></span> <span data-ttu-id="45c3a-180">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="45c3a-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="45c3a-181">operatingSystem</span></span>|<span data-ttu-id="45c3a-182">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-182">String</span></span>|<span data-ttu-id="45c3a-183">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-183">Operating system of the device.</span></span> <span data-ttu-id="45c3a-184">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="45c3a-185">deviceType</span></span>|[<span data-ttu-id="45c3a-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="45c3a-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="45c3a-187">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-187">Platform of the device.</span></span> <span data-ttu-id="45c3a-188">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-188">This property is read-only.</span></span> <span data-ttu-id="45c3a-189">Os valores possíveis `desktop` são: `windowsRT` , , , , , , , `winMO6` `nokia` , , `windowsPhone` `mac` , , `winCE` , `winEmbedded` , `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` .</span><span class="sxs-lookup"><span data-stu-id="45c3a-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="45c3a-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="45c3a-190">complianceState</span></span>|[<span data-ttu-id="45c3a-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="45c3a-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="45c3a-192">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-192">Compliance state of the device.</span></span> <span data-ttu-id="45c3a-193">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-193">This property is read-only.</span></span> <span data-ttu-id="45c3a-194">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="45c3a-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="45c3a-195">jailBroken</span></span>|<span data-ttu-id="45c3a-196">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-196">String</span></span>|<span data-ttu-id="45c3a-197">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="45c3a-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="45c3a-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-198">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="45c3a-199">managementAgent</span></span>|[<span data-ttu-id="45c3a-200">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="45c3a-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="45c3a-201">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-201">Management channel of the device.</span></span> <span data-ttu-id="45c3a-202">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="45c3a-203">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="45c3a-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="45c3a-204">osVersion</span></span>|<span data-ttu-id="45c3a-205">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-205">String</span></span>|<span data-ttu-id="45c3a-206">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-206">Operating system version of the device.</span></span> <span data-ttu-id="45c3a-207">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-207">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="45c3a-208">easActivated</span></span>|<span data-ttu-id="45c3a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-209">Boolean</span></span>|<span data-ttu-id="45c3a-210">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="45c3a-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="45c3a-211">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-211">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="45c3a-212">easDeviceId</span></span>|<span data-ttu-id="45c3a-213">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-213">String</span></span>|<span data-ttu-id="45c3a-214">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="45c3a-215">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-215">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-216">easActivationDateTime</span></span>|<span data-ttu-id="45c3a-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-217">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-218">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="45c3a-219">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-219">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-220">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="45c3a-220">aadRegistered</span></span>|<span data-ttu-id="45c3a-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-221">Boolean</span></span>|<span data-ttu-id="45c3a-222">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="45c3a-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="45c3a-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-223">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="45c3a-224">azureADRegistered</span></span>|<span data-ttu-id="45c3a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-225">Boolean</span></span>|<span data-ttu-id="45c3a-226">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="45c3a-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="45c3a-227">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-227">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="45c3a-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="45c3a-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="45c3a-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="45c3a-230">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-230">Enrollment type of the device.</span></span> <span data-ttu-id="45c3a-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-231">This property is read-only.</span></span> <span data-ttu-id="45c3a-232">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="45c3a-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="45c3a-233">lostModeState</span></span>|[<span data-ttu-id="45c3a-234">lostModeState</span><span class="sxs-lookup"><span data-stu-id="45c3a-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="45c3a-235">Indica se o modo Perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="45c3a-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="45c3a-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-236">This property is read-only.</span></span> <span data-ttu-id="45c3a-237">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="45c3a-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="45c3a-238">activationLockBypassCode</span></span>|<span data-ttu-id="45c3a-239">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-239">String</span></span>|<span data-ttu-id="45c3a-240">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="45c3a-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="45c3a-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-241">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="45c3a-242">emailAddress</span></span>|<span data-ttu-id="45c3a-243">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-243">String</span></span>|<span data-ttu-id="45c3a-244">Email(s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="45c3a-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-245">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-246">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="45c3a-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="45c3a-247">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-247">String</span></span>|<span data-ttu-id="45c3a-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="45c3a-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="45c3a-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-249">Read only.</span></span> <span data-ttu-id="45c3a-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-250">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="45c3a-251">azureADDeviceId</span></span>|<span data-ttu-id="45c3a-252">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-252">String</span></span>|<span data-ttu-id="45c3a-253">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="45c3a-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="45c3a-254">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-254">Read only.</span></span> <span data-ttu-id="45c3a-255">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-255">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="45c3a-256">deviceRegistrationState</span></span>|[<span data-ttu-id="45c3a-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="45c3a-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="45c3a-258">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-258">Device registration state.</span></span> <span data-ttu-id="45c3a-259">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-259">This property is read-only.</span></span> <span data-ttu-id="45c3a-260">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="45c3a-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="45c3a-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="45c3a-262">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-262">String</span></span>|<span data-ttu-id="45c3a-263">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-263">Device category display name.</span></span> <span data-ttu-id="45c3a-264">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-264">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="45c3a-265">isSupervised</span></span>|<span data-ttu-id="45c3a-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-266">Boolean</span></span>|<span data-ttu-id="45c3a-267">Status supervisionado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-267">Device supervised status.</span></span> <span data-ttu-id="45c3a-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-268">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="45c3a-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-270">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-271">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="45c3a-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="45c3a-272">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-272">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="45c3a-273">exchangeAccessState</span></span>|[<span data-ttu-id="45c3a-274">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="45c3a-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="45c3a-275">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="45c3a-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="45c3a-276">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-276">This property is read-only.</span></span> <span data-ttu-id="45c3a-277">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="45c3a-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="45c3a-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="45c3a-279">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="45c3a-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="45c3a-280">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="45c3a-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="45c3a-281">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-281">This property is read-only.</span></span> <span data-ttu-id="45c3a-282">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="45c3a-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="45c3a-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="45c3a-284">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-284">String</span></span>|<span data-ttu-id="45c3a-285">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="45c3a-286">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-286">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="45c3a-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="45c3a-288">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-288">String</span></span>|<span data-ttu-id="45c3a-289">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="45c3a-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="45c3a-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-290">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="45c3a-291">isEncrypted</span></span>|<span data-ttu-id="45c3a-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-292">Boolean</span></span>|<span data-ttu-id="45c3a-293">Status da criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-293">Device encryption status.</span></span> <span data-ttu-id="45c3a-294">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-294">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="45c3a-295">userPrincipalName</span></span>|<span data-ttu-id="45c3a-296">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-296">String</span></span>|<span data-ttu-id="45c3a-297">Nome principal do usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-297">Device user principal name.</span></span> <span data-ttu-id="45c3a-298">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-298">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-299">modelo</span><span class="sxs-lookup"><span data-stu-id="45c3a-299">model</span></span>|<span data-ttu-id="45c3a-300">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-300">String</span></span>|<span data-ttu-id="45c3a-301">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-301">Model of the device.</span></span> <span data-ttu-id="45c3a-302">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-302">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-303">fabricante</span><span class="sxs-lookup"><span data-stu-id="45c3a-303">manufacturer</span></span>|<span data-ttu-id="45c3a-304">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-304">String</span></span>|<span data-ttu-id="45c3a-305">Fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-305">Manufacturer of the device.</span></span> <span data-ttu-id="45c3a-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-306">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-307">imei</span><span class="sxs-lookup"><span data-stu-id="45c3a-307">imei</span></span>|<span data-ttu-id="45c3a-308">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-308">String</span></span>|<span data-ttu-id="45c3a-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="45c3a-309">IMEI.</span></span> <span data-ttu-id="45c3a-310">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-310">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="45c3a-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-312">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-313">DateTime quando o período de carência de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="45c3a-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="45c3a-314">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-314">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="45c3a-315">serialNumber</span></span>|<span data-ttu-id="45c3a-316">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-316">String</span></span>|<span data-ttu-id="45c3a-317">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="45c3a-317">SerialNumber.</span></span> <span data-ttu-id="45c3a-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-318">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="45c3a-319">phoneNumber</span></span>|<span data-ttu-id="45c3a-320">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-320">String</span></span>|<span data-ttu-id="45c3a-321">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-321">Phone number of the device.</span></span> <span data-ttu-id="45c3a-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-322">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="45c3a-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="45c3a-324">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-324">String</span></span>|<span data-ttu-id="45c3a-325">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="45c3a-325">Android security patch level.</span></span> <span data-ttu-id="45c3a-326">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-326">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="45c3a-327">userDisplayName</span></span>|<span data-ttu-id="45c3a-328">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45c3a-328">String</span></span>|<span data-ttu-id="45c3a-329">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="45c3a-329">User display name.</span></span> <span data-ttu-id="45c3a-330">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-330">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="45c3a-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="45c3a-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="45c3a-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="45c3a-333">Recursos habilitados para o cliente ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="45c3a-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="45c3a-334">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-334">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="45c3a-335">wiFiMacAddress</span></span>|<span data-ttu-id="45c3a-336">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-336">String</span></span>|<span data-ttu-id="45c3a-337">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="45c3a-337">Wi-Fi MAC.</span></span> <span data-ttu-id="45c3a-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-338">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="45c3a-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="45c3a-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="45c3a-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="45c3a-341">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-341">The device health attestation state.</span></span> <span data-ttu-id="45c3a-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-342">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="45c3a-343">subscriberCarrier</span></span>|<span data-ttu-id="45c3a-344">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-344">String</span></span>|<span data-ttu-id="45c3a-345">Transportadora assinante.</span><span class="sxs-lookup"><span data-stu-id="45c3a-345">Subscriber Carrier.</span></span> <span data-ttu-id="45c3a-346">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-346">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-347">meid</span><span class="sxs-lookup"><span data-stu-id="45c3a-347">meid</span></span>|<span data-ttu-id="45c3a-348">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-348">String</span></span>|<span data-ttu-id="45c3a-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="45c3a-349">MEID.</span></span> <span data-ttu-id="45c3a-350">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-350">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="45c3a-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="45c3a-352">Int64</span><span class="sxs-lookup"><span data-stu-id="45c3a-352">Int64</span></span>|<span data-ttu-id="45c3a-353">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="45c3a-353">Total Storage in Bytes.</span></span> <span data-ttu-id="45c3a-354">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-354">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="45c3a-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="45c3a-356">Int64</span><span class="sxs-lookup"><span data-stu-id="45c3a-356">Int64</span></span>|<span data-ttu-id="45c3a-357">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="45c3a-357">Free Storage in Bytes.</span></span> <span data-ttu-id="45c3a-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-358">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="45c3a-359">managedDeviceName</span></span>|<span data-ttu-id="45c3a-360">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-360">String</span></span>|<span data-ttu-id="45c3a-361">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="45c3a-362">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="45c3a-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="45c3a-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="45c3a-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="45c3a-364">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="45c3a-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="45c3a-365">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="45c3a-366">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-366">Read Only.</span></span> <span data-ttu-id="45c3a-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-367">This property is read-only.</span></span> <span data-ttu-id="45c3a-368">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="45c3a-369">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-369">retireAfterDateTime</span></span>|<span data-ttu-id="45c3a-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-370">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-371">Indica o tempo após o momento em que um dispositivo será automaticamente retirado devido a uma ação agendada.</span><span class="sxs-lookup"><span data-stu-id="45c3a-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="45c3a-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-372">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-373">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="45c3a-373">usersLoggedOn</span></span>|<span data-ttu-id="45c3a-374">[coleção loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="45c3a-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="45c3a-375">Indica os últimos usuários conectados de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="45c3a-376">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-376">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-377">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="45c3a-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="45c3a-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-378">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-379">Relata a DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="45c3a-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="45c3a-380">Quando definidas, as configurações do MDM do Intune substituirão as configurações da Política de Grupo se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="45c3a-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="45c3a-381">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-381">Read Only.</span></span> <span data-ttu-id="45c3a-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-382">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-383">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="45c3a-383">autopilotEnrolled</span></span>|<span data-ttu-id="45c3a-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-384">Boolean</span></span>|<span data-ttu-id="45c3a-385">Relata se o dispositivo gerenciado está inscrito por meio do piloto automático.</span><span class="sxs-lookup"><span data-stu-id="45c3a-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="45c3a-386">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-386">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="45c3a-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="45c3a-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="45c3a-388">Boolean</span></span>|<span data-ttu-id="45c3a-389">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="45c3a-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="45c3a-390">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-390">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="45c3a-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="45c3a-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c3a-392">DateTimeOffset</span></span>|<span data-ttu-id="45c3a-393">Relata a data de expiração do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="45c3a-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="45c3a-394">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-394">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-395">iccid</span><span class="sxs-lookup"><span data-stu-id="45c3a-395">iccid</span></span>|<span data-ttu-id="45c3a-396">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-396">String</span></span>|<span data-ttu-id="45c3a-397">Identificador de Placa de Circuito Integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="45c3a-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="45c3a-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-398">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-399">udid</span><span class="sxs-lookup"><span data-stu-id="45c3a-399">udid</span></span>|<span data-ttu-id="45c3a-400">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-400">String</span></span>|<span data-ttu-id="45c3a-401">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="45c3a-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="45c3a-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-402">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45c3a-403">roleScopeTagIds</span></span>|<span data-ttu-id="45c3a-404">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45c3a-404">String collection</span></span>|<span data-ttu-id="45c3a-405">Lista de IDs de Marca de Escopo para esta instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="45c3a-406">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="45c3a-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="45c3a-407">Int32</span><span class="sxs-lookup"><span data-stu-id="45c3a-407">Int32</span></span>|<span data-ttu-id="45c3a-408">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="45c3a-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="45c3a-409">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-409">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-410">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="45c3a-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="45c3a-411">Int32</span><span class="sxs-lookup"><span data-stu-id="45c3a-411">Int32</span></span>|<span data-ttu-id="45c3a-412">Contagem de malware remediado para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="45c3a-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="45c3a-413">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-413">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-414">notes</span><span class="sxs-lookup"><span data-stu-id="45c3a-414">notes</span></span>|<span data-ttu-id="45c3a-415">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-415">String</span></span>|<span data-ttu-id="45c3a-416">Observações sobre o dispositivo criado pelo administrador de IT</span><span class="sxs-lookup"><span data-stu-id="45c3a-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="45c3a-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="45c3a-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="45c3a-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="45c3a-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="45c3a-419">Estado de saúde do cliente do Gerenciador de Configurações, válido somente para dispositivos gerenciados pelo MDM/ConfigMgr Agent</span><span class="sxs-lookup"><span data-stu-id="45c3a-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="45c3a-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="45c3a-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="45c3a-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="45c3a-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="45c3a-422">Informações do cliente do Gerenciador de Configurações, válidas somente para dispositivos gerenciados, gerenciados por grupo ou gerenciados por três via ConfigMgr Agent</span><span class="sxs-lookup"><span data-stu-id="45c3a-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="45c3a-423">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="45c3a-423">ethernetMacAddress</span></span>|<span data-ttu-id="45c3a-424">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-424">String</span></span>|<span data-ttu-id="45c3a-425">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="45c3a-425">Ethernet MAC.</span></span> <span data-ttu-id="45c3a-426">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-426">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-427">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="45c3a-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="45c3a-428">Int64</span><span class="sxs-lookup"><span data-stu-id="45c3a-428">Int64</span></span>|<span data-ttu-id="45c3a-429">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="45c3a-429">Total Memory in Bytes.</span></span> <span data-ttu-id="45c3a-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-430">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-431">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="45c3a-431">processorArchitecture</span></span>|[<span data-ttu-id="45c3a-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="45c3a-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="45c3a-433">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="45c3a-433">Processor architecture.</span></span> <span data-ttu-id="45c3a-434">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-434">This property is read-only.</span></span> <span data-ttu-id="45c3a-435">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="45c3a-436">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="45c3a-436">specificationVersion</span></span>|<span data-ttu-id="45c3a-437">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-437">String</span></span>|<span data-ttu-id="45c3a-438">Versão da especificação.</span><span class="sxs-lookup"><span data-stu-id="45c3a-438">Specification version.</span></span> <span data-ttu-id="45c3a-439">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-439">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-440">joinType</span><span class="sxs-lookup"><span data-stu-id="45c3a-440">joinType</span></span>|[<span data-ttu-id="45c3a-441">joinType</span><span class="sxs-lookup"><span data-stu-id="45c3a-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="45c3a-442">Tipo de junção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45c3a-442">Device join type.</span></span> <span data-ttu-id="45c3a-443">Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="45c3a-444">skuFamily</span><span class="sxs-lookup"><span data-stu-id="45c3a-444">skuFamily</span></span>|<span data-ttu-id="45c3a-445">String</span><span class="sxs-lookup"><span data-stu-id="45c3a-445">String</span></span>|<span data-ttu-id="45c3a-446">Família de skus de dispositivos</span><span class="sxs-lookup"><span data-stu-id="45c3a-446">Device sku family</span></span>|
|<span data-ttu-id="45c3a-447">skuNumber</span><span class="sxs-lookup"><span data-stu-id="45c3a-447">skuNumber</span></span>|<span data-ttu-id="45c3a-448">Int32</span><span class="sxs-lookup"><span data-stu-id="45c3a-448">Int32</span></span>|<span data-ttu-id="45c3a-449">Número sku do dispositivo, consulte também: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="45c3a-449">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="45c3a-450">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="45c3a-450">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="45c3a-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45c3a-451">This property is read-only.</span></span>|
|<span data-ttu-id="45c3a-452">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="45c3a-452">managementFeatures</span></span>|[<span data-ttu-id="45c3a-453">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="45c3a-453">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="45c3a-454">Recursos de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="45c3a-454">Device management features.</span></span> <span data-ttu-id="45c3a-455">Os valores possíveis são: `none` e `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="45c3a-455">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="45c3a-456">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c3a-456">Response</span></span>
<span data-ttu-id="45c3a-457">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-shared-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45c3a-457">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c3a-458">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45c3a-458">Example</span></span>

### <a name="request"></a><span data-ttu-id="45c3a-459">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45c3a-459">Request</span></span>
<span data-ttu-id="45c3a-460">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45c3a-460">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8108

{
  "@odata.type": "#microsoft.graph.managedDevice",
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
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value"
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a><span data-ttu-id="45c3a-461">Resposta</span><span class="sxs-lookup"><span data-stu-id="45c3a-461">Response</span></span>
<span data-ttu-id="45c3a-p174">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45c3a-p174">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8157

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
    "batterySerialNumber": "Battery Serial Number value",
    "batteryHealthPercentage": 7,
    "batteryChargeCycles": 3,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10,
    "ipAddressV4": "Ip Address V4 value",
    "subnetAddress": "Subnet Address value"
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86",
  "specificationVersion": "Specification Version value",
  "joinType": "azureADJoined",
  "skuFamily": "Sku Family value",
  "skuNumber": 9,
  "managementFeatures": "microsoftManagedDesktop"
}
```




