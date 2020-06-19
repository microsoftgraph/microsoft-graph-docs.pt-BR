---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 36c81bfb08c6656c3c5d314a60f8b0cf56e2ab46
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792153"
---
# <a name="update-manageddevice"></a><span data-ttu-id="25d5b-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="25d5b-103">Update managedDevice</span></span>

<span data-ttu-id="25d5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25d5b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25d5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25d5b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25d5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25d5b-107">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25d5b-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25d5b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25d5b-108">Prerequisites</span></span>
<span data-ttu-id="25d5b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="25d5b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="25d5b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25d5b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d5b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25d5b-111">Permission type</span></span>|<span data-ttu-id="25d5b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25d5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25d5b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25d5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25d5b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d5b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="25d5b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25d5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25d5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25d5b-116">Not supported.</span></span>|
|<span data-ttu-id="25d5b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25d5b-117">Application</span></span>|<span data-ttu-id="25d5b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d5b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25d5b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25d5b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="25d5b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25d5b-120">Request headers</span></span>
|<span data-ttu-id="25d5b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25d5b-121">Header</span></span>|<span data-ttu-id="25d5b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="25d5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25d5b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="25d5b-123">Authorization</span></span>|<span data-ttu-id="25d5b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25d5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25d5b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="25d5b-125">Accept</span></span>|<span data-ttu-id="25d5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25d5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25d5b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25d5b-127">Request body</span></span>
<span data-ttu-id="25d5b-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25d5b-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="25d5b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="25d5b-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="25d5b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25d5b-130">Property</span></span>|<span data-ttu-id="25d5b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="25d5b-131">Type</span></span>|<span data-ttu-id="25d5b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="25d5b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d5b-133">id</span><span class="sxs-lookup"><span data-stu-id="25d5b-133">id</span></span>|<span data-ttu-id="25d5b-134">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-134">String</span></span>|<span data-ttu-id="25d5b-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-135">Unique Identifier for the device.</span></span> <span data-ttu-id="25d5b-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-136">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-137">userId</span><span class="sxs-lookup"><span data-stu-id="25d5b-137">userId</span></span>|<span data-ttu-id="25d5b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d5b-138">String</span></span>|<span data-ttu-id="25d5b-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="25d5b-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-140">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="25d5b-141">deviceName</span></span>|<span data-ttu-id="25d5b-142">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-142">String</span></span>|<span data-ttu-id="25d5b-143">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-143">Name of the device.</span></span> <span data-ttu-id="25d5b-144">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-144">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="25d5b-145">hardwareInformation</span></span>|[<span data-ttu-id="25d5b-146">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="25d5b-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="25d5b-147">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-147">The hardward details for the device.</span></span>  <span data-ttu-id="25d5b-148">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="25d5b-149">ownerType</span></span>|[<span data-ttu-id="25d5b-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="25d5b-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="25d5b-151">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-151">Ownership of the device.</span></span> <span data-ttu-id="25d5b-152">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="25d5b-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="25d5b-153">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="25d5b-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="25d5b-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="25d5b-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="25d5b-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="25d5b-156">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-156">Ownership of the device.</span></span> <span data-ttu-id="25d5b-157">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="25d5b-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="25d5b-158">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="25d5b-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="25d5b-159">deviceActionResults</span></span>|<span data-ttu-id="25d5b-160">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="25d5b-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="25d5b-161">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="25d5b-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="25d5b-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-162">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-163">ManagementState</span><span class="sxs-lookup"><span data-stu-id="25d5b-163">managementState</span></span>|[<span data-ttu-id="25d5b-164">ManagementState</span><span class="sxs-lookup"><span data-stu-id="25d5b-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="25d5b-165">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-165">Management state of the device.</span></span> <span data-ttu-id="25d5b-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-166">This property is read-only.</span></span> <span data-ttu-id="25d5b-167">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="25d5b-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-168">enrolledDateTime</span></span>|<span data-ttu-id="25d5b-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-169">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-170">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-170">Enrollment time of the device.</span></span> <span data-ttu-id="25d5b-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-171">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-172">lastSyncDateTime</span></span>|<span data-ttu-id="25d5b-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-173">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-174">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="25d5b-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="25d5b-175">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-175">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="25d5b-176">chassisType</span></span>|[<span data-ttu-id="25d5b-177">chassisType</span><span class="sxs-lookup"><span data-stu-id="25d5b-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="25d5b-178">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-178">Chassis type of the device.</span></span> <span data-ttu-id="25d5b-179">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-179">This property is read-only.</span></span> <span data-ttu-id="25d5b-180">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="25d5b-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="25d5b-181">operatingSystem</span></span>|<span data-ttu-id="25d5b-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d5b-182">String</span></span>|<span data-ttu-id="25d5b-183">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-183">Operating system of the device.</span></span> <span data-ttu-id="25d5b-184">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="25d5b-185">deviceType</span></span>|[<span data-ttu-id="25d5b-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="25d5b-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="25d5b-187">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-187">Platform of the device.</span></span> <span data-ttu-id="25d5b-188">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-188">This property is read-only.</span></span> <span data-ttu-id="25d5b-189">Os valores possíveis são:,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` , `holoLens` , `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="25d5b-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="25d5b-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="25d5b-190">complianceState</span></span>|[<span data-ttu-id="25d5b-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="25d5b-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="25d5b-192">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-192">Compliance state of the device.</span></span> <span data-ttu-id="25d5b-193">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-193">This property is read-only.</span></span> <span data-ttu-id="25d5b-194">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="25d5b-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="25d5b-195">jailBroken</span></span>|<span data-ttu-id="25d5b-196">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-196">String</span></span>|<span data-ttu-id="25d5b-197">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="25d5b-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="25d5b-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-198">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="25d5b-199">managementAgent</span></span>|[<span data-ttu-id="25d5b-200">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="25d5b-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="25d5b-201">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-201">Management channel of the device.</span></span> <span data-ttu-id="25d5b-202">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="25d5b-203">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="25d5b-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="25d5b-204">osVersion</span></span>|<span data-ttu-id="25d5b-205">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-205">String</span></span>|<span data-ttu-id="25d5b-206">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-206">Operating system version of the device.</span></span> <span data-ttu-id="25d5b-207">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-207">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="25d5b-208">easActivated</span></span>|<span data-ttu-id="25d5b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-209">Boolean</span></span>|<span data-ttu-id="25d5b-210">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="25d5b-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="25d5b-211">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-211">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="25d5b-212">easDeviceId</span></span>|<span data-ttu-id="25d5b-213">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-213">String</span></span>|<span data-ttu-id="25d5b-214">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="25d5b-215">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-215">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-216">easActivationDateTime</span></span>|<span data-ttu-id="25d5b-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-217">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-218">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="25d5b-219">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-219">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-220">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="25d5b-220">aadRegistered</span></span>|<span data-ttu-id="25d5b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-221">Boolean</span></span>|<span data-ttu-id="25d5b-222">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25d5b-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="25d5b-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-223">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="25d5b-224">azureADRegistered</span></span>|<span data-ttu-id="25d5b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-225">Boolean</span></span>|<span data-ttu-id="25d5b-226">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25d5b-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="25d5b-227">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-227">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="25d5b-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="25d5b-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="25d5b-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="25d5b-230">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-230">Enrollment type of the device.</span></span> <span data-ttu-id="25d5b-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-231">This property is read-only.</span></span> <span data-ttu-id="25d5b-232">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="25d5b-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="25d5b-233">lostModeState</span></span>|[<span data-ttu-id="25d5b-234">lostModeState</span><span class="sxs-lookup"><span data-stu-id="25d5b-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="25d5b-235">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="25d5b-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="25d5b-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-236">This property is read-only.</span></span> <span data-ttu-id="25d5b-237">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="25d5b-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="25d5b-238">activationLockBypassCode</span></span>|<span data-ttu-id="25d5b-239">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-239">String</span></span>|<span data-ttu-id="25d5b-240">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="25d5b-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="25d5b-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-241">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="25d5b-242">emailAddress</span></span>|<span data-ttu-id="25d5b-243">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-243">String</span></span>|<span data-ttu-id="25d5b-244">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="25d5b-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-245">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-246">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="25d5b-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="25d5b-247">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-247">String</span></span>|<span data-ttu-id="25d5b-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25d5b-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="25d5b-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-249">Read only.</span></span> <span data-ttu-id="25d5b-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-250">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="25d5b-251">azureADDeviceId</span></span>|<span data-ttu-id="25d5b-252">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-252">String</span></span>|<span data-ttu-id="25d5b-253">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="25d5b-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="25d5b-254">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-254">Read only.</span></span> <span data-ttu-id="25d5b-255">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-255">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="25d5b-256">deviceRegistrationState</span></span>|[<span data-ttu-id="25d5b-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="25d5b-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="25d5b-258">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-258">Device registration state.</span></span> <span data-ttu-id="25d5b-259">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-259">This property is read-only.</span></span> <span data-ttu-id="25d5b-260">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="25d5b-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="25d5b-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="25d5b-262">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-262">String</span></span>|<span data-ttu-id="25d5b-263">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-263">Device category display name.</span></span> <span data-ttu-id="25d5b-264">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-264">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="25d5b-265">isSupervised</span></span>|<span data-ttu-id="25d5b-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-266">Boolean</span></span>|<span data-ttu-id="25d5b-267">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-267">Device supervised status.</span></span> <span data-ttu-id="25d5b-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-268">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="25d5b-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-270">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-271">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d5b-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="25d5b-272">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-272">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="25d5b-273">exchangeAccessState</span></span>|[<span data-ttu-id="25d5b-274">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="25d5b-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="25d5b-275">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d5b-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="25d5b-276">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-276">This property is read-only.</span></span> <span data-ttu-id="25d5b-277">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="25d5b-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="25d5b-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="25d5b-279">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="25d5b-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="25d5b-280">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="25d5b-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="25d5b-281">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-281">This property is read-only.</span></span> <span data-ttu-id="25d5b-282">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="25d5b-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="25d5b-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="25d5b-284">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-284">String</span></span>|<span data-ttu-id="25d5b-285">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="25d5b-286">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-286">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="25d5b-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="25d5b-288">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-288">String</span></span>|<span data-ttu-id="25d5b-289">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="25d5b-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="25d5b-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-290">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="25d5b-291">isEncrypted</span></span>|<span data-ttu-id="25d5b-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-292">Boolean</span></span>|<span data-ttu-id="25d5b-293">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-293">Device encryption status.</span></span> <span data-ttu-id="25d5b-294">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-294">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="25d5b-295">userPrincipalName</span></span>|<span data-ttu-id="25d5b-296">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-296">String</span></span>|<span data-ttu-id="25d5b-297">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-297">Device user principal name.</span></span> <span data-ttu-id="25d5b-298">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-298">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-299">modelo</span><span class="sxs-lookup"><span data-stu-id="25d5b-299">model</span></span>|<span data-ttu-id="25d5b-300">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-300">String</span></span>|<span data-ttu-id="25d5b-301">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-301">Model of the device.</span></span> <span data-ttu-id="25d5b-302">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-302">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-303">fabricante</span><span class="sxs-lookup"><span data-stu-id="25d5b-303">manufacturer</span></span>|<span data-ttu-id="25d5b-304">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-304">String</span></span>|<span data-ttu-id="25d5b-305">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-305">Manufacturer of the device.</span></span> <span data-ttu-id="25d5b-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-306">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-307">imei</span><span class="sxs-lookup"><span data-stu-id="25d5b-307">imei</span></span>|<span data-ttu-id="25d5b-308">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-308">String</span></span>|<span data-ttu-id="25d5b-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="25d5b-309">IMEI.</span></span> <span data-ttu-id="25d5b-310">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-310">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="25d5b-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-312">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-313">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="25d5b-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="25d5b-314">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-314">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="25d5b-315">serialNumber</span></span>|<span data-ttu-id="25d5b-316">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d5b-316">String</span></span>|<span data-ttu-id="25d5b-317">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="25d5b-317">SerialNumber.</span></span> <span data-ttu-id="25d5b-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-318">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="25d5b-319">phoneNumber</span></span>|<span data-ttu-id="25d5b-320">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-320">String</span></span>|<span data-ttu-id="25d5b-321">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-321">Phone number of the device.</span></span> <span data-ttu-id="25d5b-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-322">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="25d5b-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="25d5b-324">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-324">String</span></span>|<span data-ttu-id="25d5b-325">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="25d5b-325">Android security patch level.</span></span> <span data-ttu-id="25d5b-326">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-326">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="25d5b-327">userDisplayName</span></span>|<span data-ttu-id="25d5b-328">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d5b-328">String</span></span>|<span data-ttu-id="25d5b-329">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="25d5b-329">User display name.</span></span> <span data-ttu-id="25d5b-330">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-330">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="25d5b-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="25d5b-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="25d5b-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="25d5b-333">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="25d5b-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="25d5b-334">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-334">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="25d5b-335">wiFiMacAddress</span></span>|<span data-ttu-id="25d5b-336">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-336">String</span></span>|<span data-ttu-id="25d5b-337">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="25d5b-337">Wi-Fi MAC.</span></span> <span data-ttu-id="25d5b-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-338">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="25d5b-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="25d5b-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="25d5b-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="25d5b-341">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-341">The device health attestation state.</span></span> <span data-ttu-id="25d5b-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-342">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="25d5b-343">subscriberCarrier</span></span>|<span data-ttu-id="25d5b-344">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-344">String</span></span>|<span data-ttu-id="25d5b-345">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="25d5b-345">Subscriber Carrier.</span></span> <span data-ttu-id="25d5b-346">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-346">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-347">meid</span><span class="sxs-lookup"><span data-stu-id="25d5b-347">meid</span></span>|<span data-ttu-id="25d5b-348">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-348">String</span></span>|<span data-ttu-id="25d5b-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="25d5b-349">MEID.</span></span> <span data-ttu-id="25d5b-350">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-350">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="25d5b-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="25d5b-352">Int64</span><span class="sxs-lookup"><span data-stu-id="25d5b-352">Int64</span></span>|<span data-ttu-id="25d5b-353">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="25d5b-353">Total Storage in Bytes.</span></span> <span data-ttu-id="25d5b-354">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-354">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="25d5b-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="25d5b-356">Int64</span><span class="sxs-lookup"><span data-stu-id="25d5b-356">Int64</span></span>|<span data-ttu-id="25d5b-357">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="25d5b-357">Free Storage in Bytes.</span></span> <span data-ttu-id="25d5b-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-358">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="25d5b-359">managedDeviceName</span></span>|<span data-ttu-id="25d5b-360">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-360">String</span></span>|<span data-ttu-id="25d5b-361">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="25d5b-362">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="25d5b-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="25d5b-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="25d5b-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="25d5b-364">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="25d5b-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="25d5b-365">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="25d5b-366">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-366">Read Only.</span></span> <span data-ttu-id="25d5b-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-367">This property is read-only.</span></span> <span data-ttu-id="25d5b-368">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="25d5b-369">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-369">retireAfterDateTime</span></span>|<span data-ttu-id="25d5b-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-370">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-371">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="25d5b-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="25d5b-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-372">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-373">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="25d5b-373">usersLoggedOn</span></span>|<span data-ttu-id="25d5b-374">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="25d5b-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="25d5b-375">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="25d5b-376">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-376">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-377">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="25d5b-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="25d5b-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-378">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-379">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="25d5b-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="25d5b-380">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="25d5b-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="25d5b-381">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-381">Read Only.</span></span> <span data-ttu-id="25d5b-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-382">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-383">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="25d5b-383">autopilotEnrolled</span></span>|<span data-ttu-id="25d5b-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-384">Boolean</span></span>|<span data-ttu-id="25d5b-385">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="25d5b-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="25d5b-386">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-386">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="25d5b-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="25d5b-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="25d5b-388">Boolean</span></span>|<span data-ttu-id="25d5b-389">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="25d5b-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="25d5b-390">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-390">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="25d5b-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="25d5b-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25d5b-392">DateTimeOffset</span></span>|<span data-ttu-id="25d5b-393">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="25d5b-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="25d5b-394">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-394">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-395">iccid</span><span class="sxs-lookup"><span data-stu-id="25d5b-395">iccid</span></span>|<span data-ttu-id="25d5b-396">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-396">String</span></span>|<span data-ttu-id="25d5b-397">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="25d5b-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="25d5b-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-398">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-399">udid</span><span class="sxs-lookup"><span data-stu-id="25d5b-399">udid</span></span>|<span data-ttu-id="25d5b-400">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-400">String</span></span>|<span data-ttu-id="25d5b-401">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="25d5b-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="25d5b-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-402">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25d5b-403">roleScopeTagIds</span></span>|<span data-ttu-id="25d5b-404">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d5b-404">String collection</span></span>|<span data-ttu-id="25d5b-405">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="25d5b-406">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="25d5b-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="25d5b-407">Int32</span><span class="sxs-lookup"><span data-stu-id="25d5b-407">Int32</span></span>|<span data-ttu-id="25d5b-408">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="25d5b-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="25d5b-409">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-409">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-410">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="25d5b-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="25d5b-411">Int32</span><span class="sxs-lookup"><span data-stu-id="25d5b-411">Int32</span></span>|<span data-ttu-id="25d5b-412">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="25d5b-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="25d5b-413">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-413">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-414">notes</span><span class="sxs-lookup"><span data-stu-id="25d5b-414">notes</span></span>|<span data-ttu-id="25d5b-415">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25d5b-415">String</span></span>|<span data-ttu-id="25d5b-416">Observações sobre o dispositivo criado pelo administrador de ti</span><span class="sxs-lookup"><span data-stu-id="25d5b-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="25d5b-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="25d5b-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="25d5b-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="25d5b-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="25d5b-419">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="25d5b-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="25d5b-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="25d5b-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="25d5b-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="25d5b-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="25d5b-422">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="25d5b-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="25d5b-423">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="25d5b-423">ethernetMacAddress</span></span>|<span data-ttu-id="25d5b-424">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-424">String</span></span>|<span data-ttu-id="25d5b-425">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="25d5b-425">Ethernet MAC.</span></span> <span data-ttu-id="25d5b-426">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-426">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-427">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="25d5b-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="25d5b-428">Int64</span><span class="sxs-lookup"><span data-stu-id="25d5b-428">Int64</span></span>|<span data-ttu-id="25d5b-429">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="25d5b-429">Total Memory in Bytes.</span></span> <span data-ttu-id="25d5b-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-430">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-431">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="25d5b-431">processorArchitecture</span></span>|[<span data-ttu-id="25d5b-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="25d5b-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="25d5b-433">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="25d5b-433">Processor architecture.</span></span> <span data-ttu-id="25d5b-434">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-434">This property is read-only.</span></span> <span data-ttu-id="25d5b-435">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="25d5b-436">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="25d5b-436">specificationVersion</span></span>|<span data-ttu-id="25d5b-437">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-437">String</span></span>|<span data-ttu-id="25d5b-438">Versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="25d5b-438">Specification version.</span></span> <span data-ttu-id="25d5b-439">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25d5b-439">This property is read-only.</span></span>|
|<span data-ttu-id="25d5b-440">joinType</span><span class="sxs-lookup"><span data-stu-id="25d5b-440">joinType</span></span>|[<span data-ttu-id="25d5b-441">joinType</span><span class="sxs-lookup"><span data-stu-id="25d5b-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="25d5b-442">Tipo de ingresso de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25d5b-442">Device join type.</span></span> <span data-ttu-id="25d5b-443">Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="25d5b-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="25d5b-444">skuFamily</span><span class="sxs-lookup"><span data-stu-id="25d5b-444">skuFamily</span></span>|<span data-ttu-id="25d5b-445">String</span><span class="sxs-lookup"><span data-stu-id="25d5b-445">String</span></span>|<span data-ttu-id="25d5b-446">Família de SKU do dispositivo</span><span class="sxs-lookup"><span data-stu-id="25d5b-446">Device sku family</span></span>|



## <a name="response"></a><span data-ttu-id="25d5b-447">Resposta</span><span class="sxs-lookup"><span data-stu-id="25d5b-447">Response</span></span>
<span data-ttu-id="25d5b-448">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25d5b-448">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25d5b-449">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25d5b-449">Example</span></span>

### <a name="request"></a><span data-ttu-id="25d5b-450">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25d5b-450">Request</span></span>
<span data-ttu-id="25d5b-451">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25d5b-451">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7823

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
    "operatingSystemProductType": 10
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
  "skuFamily": "Sku Family value"
}
```

### <a name="response"></a><span data-ttu-id="25d5b-452">Resposta</span><span class="sxs-lookup"><span data-stu-id="25d5b-452">Response</span></span>
<span data-ttu-id="25d5b-453">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="25d5b-453">Here is an example of the response.</span></span> <span data-ttu-id="25d5b-454">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="25d5b-454">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="25d5b-455">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="25d5b-455">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7872

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
    "osBuildNumber": "Os Build Number value",
    "operatingSystemProductType": 10
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
  "skuFamily": "Sku Family value"
}
```



