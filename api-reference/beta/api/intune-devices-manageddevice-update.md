---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d4cdc3242c176c92c595573de0509d151261941
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42774299"
---
# <a name="update-manageddevice"></a><span data-ttu-id="8e3bf-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="8e3bf-103">Update managedDevice</span></span>

> <span data-ttu-id="8e3bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e3bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e3bf-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="8e3bf-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e3bf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e3bf-107">Prerequisites</span></span>
<span data-ttu-id="8e3bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e3bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e3bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e3bf-110">Permission type</span></span>|<span data-ttu-id="8e3bf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e3bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e3bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e3bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e3bf-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3bf-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e3bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e3bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e3bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-115">Not supported.</span></span>|
|<span data-ttu-id="8e3bf-116">Application</span><span class="sxs-lookup"><span data-stu-id="8e3bf-116">Application</span></span>|<span data-ttu-id="8e3bf-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e3bf-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e3bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="8e3bf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3bf-119">Request headers</span></span>
|<span data-ttu-id="8e3bf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e3bf-120">Header</span></span>|<span data-ttu-id="8e3bf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e3bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e3bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e3bf-122">Authorization</span></span>|<span data-ttu-id="8e3bf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e3bf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e3bf-124">Accept</span></span>|<span data-ttu-id="8e3bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e3bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e3bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3bf-126">Request body</span></span>
<span data-ttu-id="8e3bf-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="8e3bf-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="8e3bf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="8e3bf-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="8e3bf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e3bf-129">Property</span></span>|<span data-ttu-id="8e3bf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e3bf-130">Type</span></span>|<span data-ttu-id="8e3bf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3bf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3bf-132">id</span><span class="sxs-lookup"><span data-stu-id="8e3bf-132">id</span></span>|<span data-ttu-id="8e3bf-133">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-133">String</span></span>|<span data-ttu-id="8e3bf-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-134">Unique Identifier for the device.</span></span> <span data-ttu-id="8e3bf-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-135">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-136">userId</span><span class="sxs-lookup"><span data-stu-id="8e3bf-136">userId</span></span>|<span data-ttu-id="8e3bf-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3bf-137">String</span></span>|<span data-ttu-id="8e3bf-138">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="8e3bf-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-139">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="8e3bf-140">deviceName</span></span>|<span data-ttu-id="8e3bf-141">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-141">String</span></span>|<span data-ttu-id="8e3bf-142">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-142">Name of the device.</span></span> <span data-ttu-id="8e3bf-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-143">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-144">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="8e3bf-144">hardwareInformation</span></span>|[<span data-ttu-id="8e3bf-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="8e3bf-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="8e3bf-146">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-146">The hardward details for the device.</span></span>  <span data-ttu-id="8e3bf-147">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-148">ownerType</span></span>|[<span data-ttu-id="8e3bf-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-149">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="8e3bf-150">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-150">Ownership of the device.</span></span> <span data-ttu-id="8e3bf-151">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="8e3bf-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="8e3bf-152">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="8e3bf-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="8e3bf-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="8e3bf-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-155">Ownership of the device.</span></span> <span data-ttu-id="8e3bf-156">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="8e3bf-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="8e3bf-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="8e3bf-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="8e3bf-158">deviceActionResults</span></span>|<span data-ttu-id="8e3bf-159">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e3bf-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="8e3bf-160">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="8e3bf-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-161">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-162">ManagementState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-162">managementState</span></span>|[<span data-ttu-id="8e3bf-163">ManagementState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="8e3bf-164">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-164">Management state of the device.</span></span> <span data-ttu-id="8e3bf-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-165">This property is read-only.</span></span> <span data-ttu-id="8e3bf-166">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="8e3bf-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-167">enrolledDateTime</span></span>|<span data-ttu-id="8e3bf-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-168">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-169">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-169">Enrollment time of the device.</span></span> <span data-ttu-id="8e3bf-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-170">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-171">lastSyncDateTime</span></span>|<span data-ttu-id="8e3bf-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-172">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-173">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="8e3bf-174">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-174">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-175">chassisType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-175">chassisType</span></span>|[<span data-ttu-id="8e3bf-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="8e3bf-177">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-177">Chassis type of the device.</span></span> <span data-ttu-id="8e3bf-178">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-178">This property is read-only.</span></span> <span data-ttu-id="8e3bf-179">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="8e3bf-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e3bf-180">operatingSystem</span></span>|<span data-ttu-id="8e3bf-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3bf-181">String</span></span>|<span data-ttu-id="8e3bf-182">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-182">Operating system of the device.</span></span> <span data-ttu-id="8e3bf-183">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-184">deviceType</span></span>|[<span data-ttu-id="8e3bf-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="8e3bf-186">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-186">Platform of the device.</span></span> <span data-ttu-id="8e3bf-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-187">This property is read-only.</span></span> <span data-ttu-id="8e3bf-188">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="8e3bf-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-189">complianceState</span></span>|[<span data-ttu-id="8e3bf-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="8e3bf-191">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-191">Compliance state of the device.</span></span> <span data-ttu-id="8e3bf-192">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-192">This property is read-only.</span></span> <span data-ttu-id="8e3bf-193">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="8e3bf-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="8e3bf-194">jailBroken</span></span>|<span data-ttu-id="8e3bf-195">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-195">String</span></span>|<span data-ttu-id="8e3bf-196">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="8e3bf-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-197">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="8e3bf-198">managementAgent</span></span>|[<span data-ttu-id="8e3bf-199">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-199">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="8e3bf-200">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-200">Management channel of the device.</span></span> <span data-ttu-id="8e3bf-201">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="8e3bf-202">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="8e3bf-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="8e3bf-203">osVersion</span></span>|<span data-ttu-id="8e3bf-204">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-204">String</span></span>|<span data-ttu-id="8e3bf-205">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-205">Operating system version of the device.</span></span> <span data-ttu-id="8e3bf-206">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-206">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="8e3bf-207">easActivated</span></span>|<span data-ttu-id="8e3bf-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-208">Boolean</span></span>|<span data-ttu-id="8e3bf-209">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="8e3bf-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-210">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="8e3bf-211">easDeviceId</span></span>|<span data-ttu-id="8e3bf-212">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-212">String</span></span>|<span data-ttu-id="8e3bf-213">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="8e3bf-214">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-214">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-215">easActivationDateTime</span></span>|<span data-ttu-id="8e3bf-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-216">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-217">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="8e3bf-218">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-218">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-219">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="8e3bf-219">aadRegistered</span></span>|<span data-ttu-id="8e3bf-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-220">Boolean</span></span>|<span data-ttu-id="8e3bf-221">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="8e3bf-222">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-222">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="8e3bf-223">azureADRegistered</span></span>|<span data-ttu-id="8e3bf-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-224">Boolean</span></span>|<span data-ttu-id="8e3bf-225">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="8e3bf-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-226">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="8e3bf-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8e3bf-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="8e3bf-229">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-229">Enrollment type of the device.</span></span> <span data-ttu-id="8e3bf-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-230">This property is read-only.</span></span> <span data-ttu-id="8e3bf-231">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="8e3bf-232">lostModeState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-232">lostModeState</span></span>|[<span data-ttu-id="8e3bf-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="8e3bf-234">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="8e3bf-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-235">This property is read-only.</span></span> <span data-ttu-id="8e3bf-236">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="8e3bf-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="8e3bf-237">activationLockBypassCode</span></span>|<span data-ttu-id="8e3bf-238">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-238">String</span></span>|<span data-ttu-id="8e3bf-239">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="8e3bf-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-240">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8e3bf-241">emailAddress</span></span>|<span data-ttu-id="8e3bf-242">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-242">String</span></span>|<span data-ttu-id="8e3bf-243">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="8e3bf-244">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-244">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-245">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="8e3bf-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="8e3bf-246">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-246">String</span></span>|<span data-ttu-id="8e3bf-247">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="8e3bf-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-248">Read only.</span></span> <span data-ttu-id="8e3bf-249">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-249">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="8e3bf-250">azureADDeviceId</span></span>|<span data-ttu-id="8e3bf-251">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-251">String</span></span>|<span data-ttu-id="8e3bf-252">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="8e3bf-253">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-253">Read only.</span></span> <span data-ttu-id="8e3bf-254">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-254">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-255">deviceRegistrationState</span></span>|[<span data-ttu-id="8e3bf-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="8e3bf-257">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-257">Device registration state.</span></span> <span data-ttu-id="8e3bf-258">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-258">This property is read-only.</span></span> <span data-ttu-id="8e3bf-259">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="8e3bf-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="8e3bf-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="8e3bf-261">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-261">String</span></span>|<span data-ttu-id="8e3bf-262">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-262">Device category display name.</span></span> <span data-ttu-id="8e3bf-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-263">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="8e3bf-264">isSupervised</span></span>|<span data-ttu-id="8e3bf-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-265">Boolean</span></span>|<span data-ttu-id="8e3bf-266">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-266">Device supervised status.</span></span> <span data-ttu-id="8e3bf-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-267">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="8e3bf-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-269">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-270">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="8e3bf-271">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-271">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-272">exchangeAccessState</span></span>|[<span data-ttu-id="8e3bf-273">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="8e3bf-274">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="8e3bf-275">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-275">This property is read-only.</span></span> <span data-ttu-id="8e3bf-276">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="8e3bf-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="8e3bf-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="8e3bf-278">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="8e3bf-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="8e3bf-279">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="8e3bf-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-280">This property is read-only.</span></span> <span data-ttu-id="8e3bf-281">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="8e3bf-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="8e3bf-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="8e3bf-283">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-283">String</span></span>|<span data-ttu-id="8e3bf-284">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="8e3bf-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-285">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8e3bf-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="8e3bf-287">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-287">String</span></span>|<span data-ttu-id="8e3bf-288">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="8e3bf-289">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-289">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="8e3bf-290">isEncrypted</span></span>|<span data-ttu-id="8e3bf-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-291">Boolean</span></span>|<span data-ttu-id="8e3bf-292">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-292">Device encryption status.</span></span> <span data-ttu-id="8e3bf-293">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-293">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e3bf-294">userPrincipalName</span></span>|<span data-ttu-id="8e3bf-295">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-295">String</span></span>|<span data-ttu-id="8e3bf-296">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-296">Device user principal name.</span></span> <span data-ttu-id="8e3bf-297">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-297">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-298">modelo</span><span class="sxs-lookup"><span data-stu-id="8e3bf-298">model</span></span>|<span data-ttu-id="8e3bf-299">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-299">String</span></span>|<span data-ttu-id="8e3bf-300">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-300">Model of the device.</span></span> <span data-ttu-id="8e3bf-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-301">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-302">fabricante</span><span class="sxs-lookup"><span data-stu-id="8e3bf-302">manufacturer</span></span>|<span data-ttu-id="8e3bf-303">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-303">String</span></span>|<span data-ttu-id="8e3bf-304">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-304">Manufacturer of the device.</span></span> <span data-ttu-id="8e3bf-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-305">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-306">imei</span><span class="sxs-lookup"><span data-stu-id="8e3bf-306">imei</span></span>|<span data-ttu-id="8e3bf-307">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-307">String</span></span>|<span data-ttu-id="8e3bf-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-308">IMEI.</span></span> <span data-ttu-id="8e3bf-309">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-309">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8e3bf-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-311">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-312">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="8e3bf-313">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-313">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="8e3bf-314">serialNumber</span></span>|<span data-ttu-id="8e3bf-315">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3bf-315">String</span></span>|<span data-ttu-id="8e3bf-316">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-316">SerialNumber.</span></span> <span data-ttu-id="8e3bf-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-317">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="8e3bf-318">phoneNumber</span></span>|<span data-ttu-id="8e3bf-319">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-319">String</span></span>|<span data-ttu-id="8e3bf-320">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-320">Phone number of the device.</span></span> <span data-ttu-id="8e3bf-321">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-321">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="8e3bf-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="8e3bf-323">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-323">String</span></span>|<span data-ttu-id="8e3bf-324">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-324">Android security patch level.</span></span> <span data-ttu-id="8e3bf-325">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-325">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8e3bf-326">userDisplayName</span></span>|<span data-ttu-id="8e3bf-327">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3bf-327">String</span></span>|<span data-ttu-id="8e3bf-328">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-328">User display name.</span></span> <span data-ttu-id="8e3bf-329">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-329">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="8e3bf-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="8e3bf-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="8e3bf-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="8e3bf-332">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="8e3bf-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-333">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="8e3bf-334">wiFiMacAddress</span></span>|<span data-ttu-id="8e3bf-335">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-335">String</span></span>|<span data-ttu-id="8e3bf-336">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-336">Wi-Fi MAC.</span></span> <span data-ttu-id="8e3bf-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-337">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="8e3bf-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="8e3bf-340">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-340">The device health attestation state.</span></span> <span data-ttu-id="8e3bf-341">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-341">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="8e3bf-342">subscriberCarrier</span></span>|<span data-ttu-id="8e3bf-343">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-343">String</span></span>|<span data-ttu-id="8e3bf-344">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-344">Subscriber Carrier.</span></span> <span data-ttu-id="8e3bf-345">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-345">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-346">meid</span><span class="sxs-lookup"><span data-stu-id="8e3bf-346">meid</span></span>|<span data-ttu-id="8e3bf-347">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-347">String</span></span>|<span data-ttu-id="8e3bf-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-348">MEID.</span></span> <span data-ttu-id="8e3bf-349">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-349">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="8e3bf-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="8e3bf-351">Int64</span><span class="sxs-lookup"><span data-stu-id="8e3bf-351">Int64</span></span>|<span data-ttu-id="8e3bf-352">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-352">Total Storage in Bytes.</span></span> <span data-ttu-id="8e3bf-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-353">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="8e3bf-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="8e3bf-355">Int64</span><span class="sxs-lookup"><span data-stu-id="8e3bf-355">Int64</span></span>|<span data-ttu-id="8e3bf-356">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-356">Free Storage in Bytes.</span></span> <span data-ttu-id="8e3bf-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-357">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="8e3bf-358">managedDeviceName</span></span>|<span data-ttu-id="8e3bf-359">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-359">String</span></span>|<span data-ttu-id="8e3bf-360">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="8e3bf-361">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="8e3bf-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="8e3bf-363">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="8e3bf-364">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="8e3bf-365">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-365">Read Only.</span></span> <span data-ttu-id="8e3bf-366">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-366">This property is read-only.</span></span> <span data-ttu-id="8e3bf-367">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="8e3bf-368">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-368">retireAfterDateTime</span></span>|<span data-ttu-id="8e3bf-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-369">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-370">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="8e3bf-371">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-371">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-372">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="8e3bf-372">usersLoggedOn</span></span>|<span data-ttu-id="8e3bf-373">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="8e3bf-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="8e3bf-374">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="8e3bf-375">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-375">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-376">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e3bf-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="8e3bf-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-377">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-378">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="8e3bf-379">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="8e3bf-380">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-380">Read Only.</span></span> <span data-ttu-id="8e3bf-381">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-381">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-382">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="8e3bf-382">autopilotEnrolled</span></span>|<span data-ttu-id="8e3bf-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-383">Boolean</span></span>|<span data-ttu-id="8e3bf-384">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="8e3bf-385">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-385">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-386">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="8e3bf-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="8e3bf-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e3bf-387">Boolean</span></span>|<span data-ttu-id="8e3bf-388">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="8e3bf-389">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-389">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="8e3bf-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="8e3bf-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3bf-391">DateTimeOffset</span></span>|<span data-ttu-id="8e3bf-392">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="8e3bf-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-393">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-394">iccid</span><span class="sxs-lookup"><span data-stu-id="8e3bf-394">iccid</span></span>|<span data-ttu-id="8e3bf-395">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-395">String</span></span>|<span data-ttu-id="8e3bf-396">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="8e3bf-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-397">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-398">udid</span><span class="sxs-lookup"><span data-stu-id="8e3bf-398">udid</span></span>|<span data-ttu-id="8e3bf-399">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-399">String</span></span>|<span data-ttu-id="8e3bf-400">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="8e3bf-401">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-401">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e3bf-402">roleScopeTagIds</span></span>|<span data-ttu-id="8e3bf-403">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3bf-403">String collection</span></span>|<span data-ttu-id="8e3bf-404">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="8e3bf-405">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="8e3bf-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="8e3bf-406">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3bf-406">Int32</span></span>|<span data-ttu-id="8e3bf-407">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="8e3bf-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-408">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-409">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="8e3bf-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="8e3bf-410">Int32</span><span class="sxs-lookup"><span data-stu-id="8e3bf-410">Int32</span></span>|<span data-ttu-id="8e3bf-411">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="8e3bf-412">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-412">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-413">notes</span><span class="sxs-lookup"><span data-stu-id="8e3bf-413">notes</span></span>|<span data-ttu-id="8e3bf-414">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3bf-414">String</span></span>|<span data-ttu-id="8e3bf-415">Observações sobre o dispositivo criado pelo administrador de ti</span><span class="sxs-lookup"><span data-stu-id="8e3bf-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="8e3bf-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="8e3bf-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="8e3bf-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="8e3bf-418">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="8e3bf-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="8e3bf-419">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="8e3bf-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="8e3bf-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="8e3bf-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="8e3bf-421">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="8e3bf-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="8e3bf-422">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="8e3bf-422">ethernetMacAddress</span></span>|<span data-ttu-id="8e3bf-423">String</span><span class="sxs-lookup"><span data-stu-id="8e3bf-423">String</span></span>|<span data-ttu-id="8e3bf-424">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-424">Ethernet MAC.</span></span> <span data-ttu-id="8e3bf-425">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-425">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-426">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="8e3bf-426">physicalMemoryInBytes</span></span>|<span data-ttu-id="8e3bf-427">Int64</span><span class="sxs-lookup"><span data-stu-id="8e3bf-427">Int64</span></span>|<span data-ttu-id="8e3bf-428">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-428">Total Memory in Bytes.</span></span> <span data-ttu-id="8e3bf-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-429">This property is read-only.</span></span>|
|<span data-ttu-id="8e3bf-430">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="8e3bf-430">processorArchitecture</span></span>|[<span data-ttu-id="8e3bf-431">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="8e3bf-431">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="8e3bf-432">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-432">Processor architecture.</span></span> <span data-ttu-id="8e3bf-433">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-433">This property is read-only.</span></span> <span data-ttu-id="8e3bf-434">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-434">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="8e3bf-435">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3bf-435">Response</span></span>
<span data-ttu-id="8e3bf-436">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-436">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e3bf-437">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e3bf-437">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e3bf-438">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3bf-438">Request</span></span>
<span data-ttu-id="8e3bf-439">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-439">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7658

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
    "osBuildNumber": "Os Build Number value"
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
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="8e3bf-440">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3bf-440">Response</span></span>
<span data-ttu-id="8e3bf-p170">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e3bf-p170">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7707

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
    "osBuildNumber": "Os Build Number value"
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
  "processorArchitecture": "x86"
}
```




