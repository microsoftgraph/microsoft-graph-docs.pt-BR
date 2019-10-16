---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a51ae80b13e1b6a0a571e1213c0c7638d945f3c5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37528238"
---
# <a name="update-manageddevice"></a><span data-ttu-id="ab134-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="ab134-103">Update managedDevice</span></span>

> <span data-ttu-id="ab134-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab134-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab134-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab134-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab134-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab134-107">Prerequisites</span></span>
<span data-ttu-id="ab134-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab134-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab134-110">Permission type</span></span>|<span data-ttu-id="ab134-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab134-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab134-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab134-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab134-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab134-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab134-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab134-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab134-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab134-115">Not supported.</span></span>|
|<span data-ttu-id="ab134-116">Application</span><span class="sxs-lookup"><span data-stu-id="ab134-116">Application</span></span>|<span data-ttu-id="ab134-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab134-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab134-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab134-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ab134-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab134-119">Request headers</span></span>
|<span data-ttu-id="ab134-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab134-120">Header</span></span>|<span data-ttu-id="ab134-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ab134-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab134-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab134-122">Authorization</span></span>|<span data-ttu-id="ab134-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab134-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab134-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab134-124">Accept</span></span>|<span data-ttu-id="ab134-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab134-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab134-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab134-126">Request body</span></span>
<span data-ttu-id="ab134-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab134-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="ab134-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ab134-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="ab134-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab134-129">Property</span></span>|<span data-ttu-id="ab134-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab134-130">Type</span></span>|<span data-ttu-id="ab134-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab134-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab134-132">id</span><span class="sxs-lookup"><span data-stu-id="ab134-132">id</span></span>|<span data-ttu-id="ab134-133">String</span><span class="sxs-lookup"><span data-stu-id="ab134-133">String</span></span>|<span data-ttu-id="ab134-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-134">Unique Identifier for the device.</span></span> <span data-ttu-id="ab134-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-135">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-136">userId</span><span class="sxs-lookup"><span data-stu-id="ab134-136">userId</span></span>|<span data-ttu-id="ab134-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-137">String</span></span>|<span data-ttu-id="ab134-138">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="ab134-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-139">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="ab134-140">deviceName</span></span>|<span data-ttu-id="ab134-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-141">String</span></span>|<span data-ttu-id="ab134-142">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-142">Name of the device.</span></span> <span data-ttu-id="ab134-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-143">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-144">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ab134-144">hardwareInformation</span></span>|[<span data-ttu-id="ab134-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ab134-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="ab134-146">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-146">The hardward details for the device.</span></span>  <span data-ttu-id="ab134-147">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="ab134-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="ab134-148">ownerType</span></span>|[<span data-ttu-id="ab134-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="ab134-149">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="ab134-150">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-150">Ownership of the device.</span></span> <span data-ttu-id="ab134-151">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="ab134-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ab134-152">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ab134-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ab134-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ab134-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ab134-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ab134-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="ab134-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-155">Ownership of the device.</span></span> <span data-ttu-id="ab134-156">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="ab134-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ab134-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ab134-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ab134-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ab134-158">deviceActionResults</span></span>|<span data-ttu-id="ab134-159">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ab134-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ab134-160">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="ab134-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="ab134-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-161">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-162">ManagementState</span><span class="sxs-lookup"><span data-stu-id="ab134-162">managementState</span></span>|[<span data-ttu-id="ab134-163">ManagementState</span><span class="sxs-lookup"><span data-stu-id="ab134-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="ab134-164">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-164">Management state of the device.</span></span> <span data-ttu-id="ab134-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-165">This property is read-only.</span></span> <span data-ttu-id="ab134-166">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="ab134-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="ab134-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-167">enrolledDateTime</span></span>|<span data-ttu-id="ab134-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-168">DateTimeOffset</span></span>|<span data-ttu-id="ab134-169">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-169">Enrollment time of the device.</span></span> <span data-ttu-id="ab134-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-170">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-171">lastSyncDateTime</span></span>|<span data-ttu-id="ab134-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-172">DateTimeOffset</span></span>|<span data-ttu-id="ab134-173">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="ab134-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="ab134-174">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-174">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-175">chassisType</span><span class="sxs-lookup"><span data-stu-id="ab134-175">chassisType</span></span>|[<span data-ttu-id="ab134-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="ab134-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="ab134-177">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-177">Chassis type of the device.</span></span> <span data-ttu-id="ab134-178">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-178">This property is read-only.</span></span> <span data-ttu-id="ab134-179">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="ab134-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="ab134-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ab134-180">operatingSystem</span></span>|<span data-ttu-id="ab134-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-181">String</span></span>|<span data-ttu-id="ab134-182">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-182">Operating system of the device.</span></span> <span data-ttu-id="ab134-183">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="ab134-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="ab134-184">deviceType</span></span>|[<span data-ttu-id="ab134-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="ab134-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="ab134-186">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-186">Platform of the device.</span></span> <span data-ttu-id="ab134-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-187">This property is read-only.</span></span> <span data-ttu-id="ab134-188">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ab134-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="ab134-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="ab134-189">complianceState</span></span>|[<span data-ttu-id="ab134-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="ab134-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ab134-191">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-191">Compliance state of the device.</span></span> <span data-ttu-id="ab134-192">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-192">This property is read-only.</span></span> <span data-ttu-id="ab134-193">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ab134-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ab134-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ab134-194">jailBroken</span></span>|<span data-ttu-id="ab134-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-195">String</span></span>|<span data-ttu-id="ab134-196">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="ab134-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="ab134-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-197">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ab134-198">managementAgent</span></span>|[<span data-ttu-id="ab134-199">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ab134-199">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="ab134-200">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-200">Management channel of the device.</span></span> <span data-ttu-id="ab134-201">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="ab134-202">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="ab134-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="ab134-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="ab134-203">osVersion</span></span>|<span data-ttu-id="ab134-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-204">String</span></span>|<span data-ttu-id="ab134-205">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-205">Operating system version of the device.</span></span> <span data-ttu-id="ab134-206">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-206">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="ab134-207">easActivated</span></span>|<span data-ttu-id="ab134-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab134-208">Boolean</span></span>|<span data-ttu-id="ab134-209">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ab134-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="ab134-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-210">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab134-211">easDeviceId</span></span>|<span data-ttu-id="ab134-212">String</span><span class="sxs-lookup"><span data-stu-id="ab134-212">String</span></span>|<span data-ttu-id="ab134-213">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="ab134-214">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-214">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-215">easActivationDateTime</span></span>|<span data-ttu-id="ab134-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-216">DateTimeOffset</span></span>|<span data-ttu-id="ab134-217">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="ab134-218">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-218">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-219">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="ab134-219">aadRegistered</span></span>|<span data-ttu-id="ab134-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab134-220">Boolean</span></span>|<span data-ttu-id="ab134-221">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab134-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="ab134-222">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-222">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ab134-223">azureADRegistered</span></span>|<span data-ttu-id="ab134-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab134-224">Boolean</span></span>|<span data-ttu-id="ab134-225">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab134-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="ab134-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-226">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ab134-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="ab134-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ab134-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="ab134-229">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-229">Enrollment type of the device.</span></span> <span data-ttu-id="ab134-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-230">This property is read-only.</span></span> <span data-ttu-id="ab134-231">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="ab134-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="ab134-232">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ab134-232">lostModeState</span></span>|[<span data-ttu-id="ab134-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ab134-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="ab134-234">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="ab134-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="ab134-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-235">This property is read-only.</span></span> <span data-ttu-id="ab134-236">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="ab134-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="ab134-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ab134-237">activationLockBypassCode</span></span>|<span data-ttu-id="ab134-238">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-238">String</span></span>|<span data-ttu-id="ab134-239">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="ab134-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="ab134-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-240">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ab134-241">emailAddress</span></span>|<span data-ttu-id="ab134-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-242">String</span></span>|<span data-ttu-id="ab134-243">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="ab134-244">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-244">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-245">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab134-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="ab134-246">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-246">String</span></span>|<span data-ttu-id="ab134-247">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab134-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ab134-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-248">Read only.</span></span> <span data-ttu-id="ab134-249">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-249">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ab134-250">azureADDeviceId</span></span>|<span data-ttu-id="ab134-251">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-251">String</span></span>|<span data-ttu-id="ab134-252">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab134-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ab134-253">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-253">Read only.</span></span> <span data-ttu-id="ab134-254">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-254">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ab134-255">deviceRegistrationState</span></span>|[<span data-ttu-id="ab134-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ab134-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ab134-257">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-257">Device registration state.</span></span> <span data-ttu-id="ab134-258">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-258">This property is read-only.</span></span> <span data-ttu-id="ab134-259">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ab134-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ab134-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab134-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ab134-261">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-261">String</span></span>|<span data-ttu-id="ab134-262">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-262">Device category display name.</span></span> <span data-ttu-id="ab134-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-263">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ab134-264">isSupervised</span></span>|<span data-ttu-id="ab134-265">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab134-265">Boolean</span></span>|<span data-ttu-id="ab134-266">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-266">Device supervised status.</span></span> <span data-ttu-id="ab134-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-267">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ab134-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-269">DateTimeOffset</span></span>|<span data-ttu-id="ab134-270">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab134-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="ab134-271">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-271">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ab134-272">exchangeAccessState</span></span>|[<span data-ttu-id="ab134-273">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ab134-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ab134-274">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab134-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ab134-275">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-275">This property is read-only.</span></span> <span data-ttu-id="ab134-276">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="ab134-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ab134-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ab134-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ab134-278">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ab134-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ab134-279">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab134-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ab134-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-280">This property is read-only.</span></span> <span data-ttu-id="ab134-281">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="ab134-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ab134-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ab134-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ab134-283">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-283">String</span></span>|<span data-ttu-id="ab134-284">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="ab134-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-285">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ab134-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ab134-287">String</span><span class="sxs-lookup"><span data-stu-id="ab134-287">String</span></span>|<span data-ttu-id="ab134-288">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="ab134-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="ab134-289">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-289">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ab134-290">isEncrypted</span></span>|<span data-ttu-id="ab134-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab134-291">Boolean</span></span>|<span data-ttu-id="ab134-292">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-292">Device encryption status.</span></span> <span data-ttu-id="ab134-293">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-293">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ab134-294">userPrincipalName</span></span>|<span data-ttu-id="ab134-295">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-295">String</span></span>|<span data-ttu-id="ab134-296">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-296">Device user principal name.</span></span> <span data-ttu-id="ab134-297">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-297">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-298">modelo</span><span class="sxs-lookup"><span data-stu-id="ab134-298">model</span></span>|<span data-ttu-id="ab134-299">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-299">String</span></span>|<span data-ttu-id="ab134-300">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-300">Model of the device.</span></span> <span data-ttu-id="ab134-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-301">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-302">fabricante</span><span class="sxs-lookup"><span data-stu-id="ab134-302">manufacturer</span></span>|<span data-ttu-id="ab134-303">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-303">String</span></span>|<span data-ttu-id="ab134-304">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-304">Manufacturer of the device.</span></span> <span data-ttu-id="ab134-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-305">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-306">imei</span><span class="sxs-lookup"><span data-stu-id="ab134-306">imei</span></span>|<span data-ttu-id="ab134-307">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-307">String</span></span>|<span data-ttu-id="ab134-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="ab134-308">IMEI.</span></span> <span data-ttu-id="ab134-309">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-309">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ab134-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-311">DateTimeOffset</span></span>|<span data-ttu-id="ab134-312">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="ab134-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="ab134-313">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-313">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ab134-314">serialNumber</span></span>|<span data-ttu-id="ab134-315">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-315">String</span></span>|<span data-ttu-id="ab134-316">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="ab134-316">SerialNumber.</span></span> <span data-ttu-id="ab134-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-317">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ab134-318">phoneNumber</span></span>|<span data-ttu-id="ab134-319">String</span><span class="sxs-lookup"><span data-stu-id="ab134-319">String</span></span>|<span data-ttu-id="ab134-320">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-320">Phone number of the device.</span></span> <span data-ttu-id="ab134-321">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-321">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ab134-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ab134-323">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-323">String</span></span>|<span data-ttu-id="ab134-324">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="ab134-324">Android security patch level.</span></span> <span data-ttu-id="ab134-325">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-325">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab134-326">userDisplayName</span></span>|<span data-ttu-id="ab134-327">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-327">String</span></span>|<span data-ttu-id="ab134-328">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab134-328">User display name.</span></span> <span data-ttu-id="ab134-329">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-329">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ab134-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ab134-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ab134-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ab134-332">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="ab134-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="ab134-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-333">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ab134-334">wiFiMacAddress</span></span>|<span data-ttu-id="ab134-335">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-335">String</span></span>|<span data-ttu-id="ab134-336">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ab134-336">Wi-Fi MAC.</span></span> <span data-ttu-id="ab134-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-337">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ab134-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ab134-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ab134-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ab134-340">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-340">The device health attestation state.</span></span> <span data-ttu-id="ab134-341">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-341">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ab134-342">subscriberCarrier</span></span>|<span data-ttu-id="ab134-343">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-343">String</span></span>|<span data-ttu-id="ab134-344">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="ab134-344">Subscriber Carrier.</span></span> <span data-ttu-id="ab134-345">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-345">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-346">meid</span><span class="sxs-lookup"><span data-stu-id="ab134-346">meid</span></span>|<span data-ttu-id="ab134-347">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-347">String</span></span>|<span data-ttu-id="ab134-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="ab134-348">MEID.</span></span> <span data-ttu-id="ab134-349">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-349">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ab134-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ab134-351">Int64</span><span class="sxs-lookup"><span data-stu-id="ab134-351">Int64</span></span>|<span data-ttu-id="ab134-352">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="ab134-352">Total Storage in Bytes.</span></span> <span data-ttu-id="ab134-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-353">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ab134-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ab134-355">Int64</span><span class="sxs-lookup"><span data-stu-id="ab134-355">Int64</span></span>|<span data-ttu-id="ab134-356">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="ab134-356">Free Storage in Bytes.</span></span> <span data-ttu-id="ab134-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-357">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ab134-358">managedDeviceName</span></span>|<span data-ttu-id="ab134-359">String</span><span class="sxs-lookup"><span data-stu-id="ab134-359">String</span></span>|<span data-ttu-id="ab134-360">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ab134-361">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ab134-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="ab134-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ab134-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="ab134-363">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="ab134-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ab134-364">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ab134-365">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-365">Read Only.</span></span> <span data-ttu-id="ab134-366">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-366">This property is read-only.</span></span> <span data-ttu-id="ab134-367">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="ab134-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="ab134-368">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-368">retireAfterDateTime</span></span>|<span data-ttu-id="ab134-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-369">DateTimeOffset</span></span>|<span data-ttu-id="ab134-370">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="ab134-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="ab134-371">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-371">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-372">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="ab134-372">usersLoggedOn</span></span>|<span data-ttu-id="ab134-373">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="ab134-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="ab134-374">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="ab134-375">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-375">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-376">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab134-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="ab134-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-377">DateTimeOffset</span></span>|<span data-ttu-id="ab134-378">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="ab134-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="ab134-379">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="ab134-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="ab134-380">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-380">Read Only.</span></span> <span data-ttu-id="ab134-381">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-381">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-382">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="ab134-382">autopilotEnrolled</span></span>|<span data-ttu-id="ab134-383">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab134-383">Boolean</span></span>|<span data-ttu-id="ab134-384">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="ab134-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="ab134-385">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-385">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-386">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="ab134-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="ab134-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab134-387">Boolean</span></span>|<span data-ttu-id="ab134-388">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab134-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="ab134-389">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-389">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="ab134-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="ab134-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab134-391">DateTimeOffset</span></span>|<span data-ttu-id="ab134-392">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ab134-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="ab134-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-393">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-394">iccid</span><span class="sxs-lookup"><span data-stu-id="ab134-394">iccid</span></span>|<span data-ttu-id="ab134-395">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-395">String</span></span>|<span data-ttu-id="ab134-396">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="ab134-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="ab134-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-397">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-398">udid</span><span class="sxs-lookup"><span data-stu-id="ab134-398">udid</span></span>|<span data-ttu-id="ab134-399">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-399">String</span></span>|<span data-ttu-id="ab134-400">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="ab134-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="ab134-401">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-401">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab134-402">roleScopeTagIds</span></span>|<span data-ttu-id="ab134-403">String collection</span><span class="sxs-lookup"><span data-stu-id="ab134-403">String collection</span></span>|<span data-ttu-id="ab134-404">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab134-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="ab134-405">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ab134-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="ab134-406">Int32</span><span class="sxs-lookup"><span data-stu-id="ab134-406">Int32</span></span>|<span data-ttu-id="ab134-407">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="ab134-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="ab134-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-408">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-409">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ab134-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="ab134-410">Int32</span><span class="sxs-lookup"><span data-stu-id="ab134-410">Int32</span></span>|<span data-ttu-id="ab134-411">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="ab134-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="ab134-412">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab134-412">This property is read-only.</span></span>|
|<span data-ttu-id="ab134-413">notes</span><span class="sxs-lookup"><span data-stu-id="ab134-413">notes</span></span>|<span data-ttu-id="ab134-414">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab134-414">String</span></span>|<span data-ttu-id="ab134-415">Observações sobre o dispositivo criado pelo administrador de ti</span><span class="sxs-lookup"><span data-stu-id="ab134-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="ab134-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ab134-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="ab134-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ab134-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="ab134-418">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="ab134-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="ab134-419">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="ab134-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="ab134-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="ab134-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="ab134-421">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="ab134-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="ab134-422">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab134-422">Response</span></span>
<span data-ttu-id="ab134-423">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab134-423">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab134-424">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab134-424">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab134-425">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab134-425">Request</span></span>
<span data-ttu-id="ab134-426">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab134-426">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7513

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
    "clientIdentifier": "Client Identifier value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ab134-427">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab134-427">Response</span></span>
<span data-ttu-id="ab134-p167">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab134-p167">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7562

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
    "clientIdentifier": "Client Identifier value"
  }
}
```






