---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 035c6501fe91398dc8f7d723ffdf5648689acb1d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162089"
---
# <a name="update-manageddevice"></a><span data-ttu-id="66162-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="66162-103">Update managedDevice</span></span>

> <span data-ttu-id="66162-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66162-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66162-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66162-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66162-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="66162-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66162-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66162-107">Prerequisites</span></span>
<span data-ttu-id="66162-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66162-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66162-110">Permission type</span></span>|<span data-ttu-id="66162-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66162-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66162-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66162-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66162-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66162-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="66162-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66162-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66162-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66162-115">Not supported.</span></span>|
|<span data-ttu-id="66162-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66162-116">Application</span></span>|<span data-ttu-id="66162-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66162-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66162-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66162-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="66162-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66162-119">Request headers</span></span>
|<span data-ttu-id="66162-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66162-120">Header</span></span>|<span data-ttu-id="66162-121">Valor</span><span class="sxs-lookup"><span data-stu-id="66162-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66162-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66162-122">Authorization</span></span>|<span data-ttu-id="66162-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66162-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66162-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66162-124">Accept</span></span>|<span data-ttu-id="66162-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66162-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66162-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66162-126">Request body</span></span>
<span data-ttu-id="66162-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="66162-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="66162-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="66162-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="66162-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66162-129">Property</span></span>|<span data-ttu-id="66162-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="66162-130">Type</span></span>|<span data-ttu-id="66162-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="66162-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66162-132">id</span><span class="sxs-lookup"><span data-stu-id="66162-132">id</span></span>|<span data-ttu-id="66162-133">String</span><span class="sxs-lookup"><span data-stu-id="66162-133">String</span></span>|<span data-ttu-id="66162-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-134">Unique Identifier for the device.</span></span> <span data-ttu-id="66162-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-135">This property is read-only.</span></span>|
|<span data-ttu-id="66162-136">userId</span><span class="sxs-lookup"><span data-stu-id="66162-136">userId</span></span>|<span data-ttu-id="66162-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66162-137">String</span></span>|<span data-ttu-id="66162-138">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="66162-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-139">This property is read-only.</span></span>|
|<span data-ttu-id="66162-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="66162-140">deviceName</span></span>|<span data-ttu-id="66162-141">String</span><span class="sxs-lookup"><span data-stu-id="66162-141">String</span></span>|<span data-ttu-id="66162-142">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-142">Name of the device.</span></span> <span data-ttu-id="66162-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-143">This property is read-only.</span></span>|
|<span data-ttu-id="66162-144">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="66162-144">hardwareInformation</span></span>|[<span data-ttu-id="66162-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="66162-145">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="66162-146">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-146">The hardward details for the device.</span></span>  <span data-ttu-id="66162-147">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-147">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="66162-148">ownerType</span><span class="sxs-lookup"><span data-stu-id="66162-148">ownerType</span></span>|[<span data-ttu-id="66162-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="66162-149">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="66162-150">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-150">Ownership of the device.</span></span> <span data-ttu-id="66162-151">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="66162-151">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="66162-152">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="66162-152">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="66162-153">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="66162-153">managedDeviceOwnerType</span></span>|[<span data-ttu-id="66162-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="66162-154">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="66162-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-155">Ownership of the device.</span></span> <span data-ttu-id="66162-156">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="66162-156">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="66162-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="66162-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="66162-158">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="66162-158">deviceActionResults</span></span>|<span data-ttu-id="66162-159">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="66162-159">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="66162-160">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="66162-160">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="66162-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-161">This property is read-only.</span></span>|
|<span data-ttu-id="66162-162">ManagementState</span><span class="sxs-lookup"><span data-stu-id="66162-162">managementState</span></span>|[<span data-ttu-id="66162-163">ManagementState</span><span class="sxs-lookup"><span data-stu-id="66162-163">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="66162-164">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-164">Management state of the device.</span></span> <span data-ttu-id="66162-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-165">This property is read-only.</span></span> <span data-ttu-id="66162-166">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="66162-166">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="66162-167">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-167">enrolledDateTime</span></span>|<span data-ttu-id="66162-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-168">DateTimeOffset</span></span>|<span data-ttu-id="66162-169">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-169">Enrollment time of the device.</span></span> <span data-ttu-id="66162-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-170">This property is read-only.</span></span>|
|<span data-ttu-id="66162-171">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-171">lastSyncDateTime</span></span>|<span data-ttu-id="66162-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-172">DateTimeOffset</span></span>|<span data-ttu-id="66162-173">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="66162-173">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="66162-174">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-174">This property is read-only.</span></span>|
|<span data-ttu-id="66162-175">chassisType</span><span class="sxs-lookup"><span data-stu-id="66162-175">chassisType</span></span>|[<span data-ttu-id="66162-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="66162-176">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="66162-177">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-177">Chassis type of the device.</span></span> <span data-ttu-id="66162-178">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-178">This property is read-only.</span></span> <span data-ttu-id="66162-179">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="66162-179">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="66162-180">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="66162-180">operatingSystem</span></span>|<span data-ttu-id="66162-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66162-181">String</span></span>|<span data-ttu-id="66162-182">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-182">Operating system of the device.</span></span> <span data-ttu-id="66162-183">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-183">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="66162-184">deviceType</span><span class="sxs-lookup"><span data-stu-id="66162-184">deviceType</span></span>|[<span data-ttu-id="66162-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="66162-185">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="66162-186">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-186">Platform of the device.</span></span> <span data-ttu-id="66162-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-187">This property is read-only.</span></span> <span data-ttu-id="66162-188">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="66162-188">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="66162-189">complianceState</span><span class="sxs-lookup"><span data-stu-id="66162-189">complianceState</span></span>|[<span data-ttu-id="66162-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="66162-190">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="66162-191">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-191">Compliance state of the device.</span></span> <span data-ttu-id="66162-192">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-192">This property is read-only.</span></span> <span data-ttu-id="66162-193">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="66162-193">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="66162-194">jailBroken</span><span class="sxs-lookup"><span data-stu-id="66162-194">jailBroken</span></span>|<span data-ttu-id="66162-195">String</span><span class="sxs-lookup"><span data-stu-id="66162-195">String</span></span>|<span data-ttu-id="66162-196">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="66162-196">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="66162-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-197">This property is read-only.</span></span>|
|<span data-ttu-id="66162-198">managementAgent</span><span class="sxs-lookup"><span data-stu-id="66162-198">managementAgent</span></span>|[<span data-ttu-id="66162-199">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="66162-199">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="66162-200">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-200">Management channel of the device.</span></span> <span data-ttu-id="66162-201">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-201">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="66162-202">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="66162-202">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="66162-203">osVersion</span><span class="sxs-lookup"><span data-stu-id="66162-203">osVersion</span></span>|<span data-ttu-id="66162-204">String</span><span class="sxs-lookup"><span data-stu-id="66162-204">String</span></span>|<span data-ttu-id="66162-205">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-205">Operating system version of the device.</span></span> <span data-ttu-id="66162-206">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-206">This property is read-only.</span></span>|
|<span data-ttu-id="66162-207">easActivated</span><span class="sxs-lookup"><span data-stu-id="66162-207">easActivated</span></span>|<span data-ttu-id="66162-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="66162-208">Boolean</span></span>|<span data-ttu-id="66162-209">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="66162-209">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="66162-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-210">This property is read-only.</span></span>|
|<span data-ttu-id="66162-211">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="66162-211">easDeviceId</span></span>|<span data-ttu-id="66162-212">String</span><span class="sxs-lookup"><span data-stu-id="66162-212">String</span></span>|<span data-ttu-id="66162-213">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-213">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="66162-214">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-214">This property is read-only.</span></span>|
|<span data-ttu-id="66162-215">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-215">easActivationDateTime</span></span>|<span data-ttu-id="66162-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-216">DateTimeOffset</span></span>|<span data-ttu-id="66162-217">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-217">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="66162-218">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-218">This property is read-only.</span></span>|
|<span data-ttu-id="66162-219">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="66162-219">aadRegistered</span></span>|<span data-ttu-id="66162-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="66162-220">Boolean</span></span>|<span data-ttu-id="66162-221">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66162-221">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="66162-222">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-222">This property is read-only.</span></span>|
|<span data-ttu-id="66162-223">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="66162-223">azureADRegistered</span></span>|<span data-ttu-id="66162-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="66162-224">Boolean</span></span>|<span data-ttu-id="66162-225">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66162-225">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="66162-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-226">This property is read-only.</span></span>|
|<span data-ttu-id="66162-227">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="66162-227">deviceEnrollmentType</span></span>|[<span data-ttu-id="66162-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="66162-228">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="66162-229">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-229">Enrollment type of the device.</span></span> <span data-ttu-id="66162-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-230">This property is read-only.</span></span> <span data-ttu-id="66162-231">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="66162-231">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="66162-232">lostModeState</span><span class="sxs-lookup"><span data-stu-id="66162-232">lostModeState</span></span>|[<span data-ttu-id="66162-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="66162-233">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="66162-234">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="66162-234">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="66162-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-235">This property is read-only.</span></span> <span data-ttu-id="66162-236">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="66162-236">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="66162-237">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="66162-237">activationLockBypassCode</span></span>|<span data-ttu-id="66162-238">String</span><span class="sxs-lookup"><span data-stu-id="66162-238">String</span></span>|<span data-ttu-id="66162-239">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="66162-239">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="66162-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-240">This property is read-only.</span></span>|
|<span data-ttu-id="66162-241">emailAddress</span><span class="sxs-lookup"><span data-stu-id="66162-241">emailAddress</span></span>|<span data-ttu-id="66162-242">String</span><span class="sxs-lookup"><span data-stu-id="66162-242">String</span></span>|<span data-ttu-id="66162-243">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-243">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="66162-244">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-244">This property is read-only.</span></span>|
|<span data-ttu-id="66162-245">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="66162-245">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="66162-246">String</span><span class="sxs-lookup"><span data-stu-id="66162-246">String</span></span>|<span data-ttu-id="66162-247">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66162-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="66162-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-248">Read only.</span></span> <span data-ttu-id="66162-249">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-249">This property is read-only.</span></span>|
|<span data-ttu-id="66162-250">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="66162-250">azureADDeviceId</span></span>|<span data-ttu-id="66162-251">String</span><span class="sxs-lookup"><span data-stu-id="66162-251">String</span></span>|<span data-ttu-id="66162-252">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66162-252">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="66162-253">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-253">Read only.</span></span> <span data-ttu-id="66162-254">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-254">This property is read-only.</span></span>|
|<span data-ttu-id="66162-255">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="66162-255">deviceRegistrationState</span></span>|[<span data-ttu-id="66162-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="66162-256">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="66162-257">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-257">Device registration state.</span></span> <span data-ttu-id="66162-258">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-258">This property is read-only.</span></span> <span data-ttu-id="66162-259">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="66162-259">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="66162-260">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="66162-260">deviceCategoryDisplayName</span></span>|<span data-ttu-id="66162-261">String</span><span class="sxs-lookup"><span data-stu-id="66162-261">String</span></span>|<span data-ttu-id="66162-262">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-262">Device category display name.</span></span> <span data-ttu-id="66162-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-263">This property is read-only.</span></span>|
|<span data-ttu-id="66162-264">isSupervised</span><span class="sxs-lookup"><span data-stu-id="66162-264">isSupervised</span></span>|<span data-ttu-id="66162-265">Booliano</span><span class="sxs-lookup"><span data-stu-id="66162-265">Boolean</span></span>|<span data-ttu-id="66162-266">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-266">Device supervised status.</span></span> <span data-ttu-id="66162-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-267">This property is read-only.</span></span>|
|<span data-ttu-id="66162-268">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-268">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="66162-269">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-269">DateTimeOffset</span></span>|<span data-ttu-id="66162-270">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="66162-270">Last time the device contacted Exchange.</span></span> <span data-ttu-id="66162-271">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-271">This property is read-only.</span></span>|
|<span data-ttu-id="66162-272">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="66162-272">exchangeAccessState</span></span>|[<span data-ttu-id="66162-273">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="66162-273">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="66162-274">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="66162-274">The Access State of the device in Exchange.</span></span> <span data-ttu-id="66162-275">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-275">This property is read-only.</span></span> <span data-ttu-id="66162-276">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="66162-276">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="66162-277">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="66162-277">exchangeAccessStateReason</span></span>|[<span data-ttu-id="66162-278">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="66162-278">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="66162-279">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="66162-279">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="66162-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-280">This property is read-only.</span></span> <span data-ttu-id="66162-281">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="66162-281">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="66162-282">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="66162-282">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="66162-283">String</span><span class="sxs-lookup"><span data-stu-id="66162-283">String</span></span>|<span data-ttu-id="66162-284">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-284">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="66162-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-285">This property is read-only.</span></span>|
|<span data-ttu-id="66162-286">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="66162-286">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="66162-287">String</span><span class="sxs-lookup"><span data-stu-id="66162-287">String</span></span>|<span data-ttu-id="66162-288">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="66162-288">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="66162-289">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-289">This property is read-only.</span></span>|
|<span data-ttu-id="66162-290">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="66162-290">isEncrypted</span></span>|<span data-ttu-id="66162-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="66162-291">Boolean</span></span>|<span data-ttu-id="66162-292">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-292">Device encryption status.</span></span> <span data-ttu-id="66162-293">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-293">This property is read-only.</span></span>|
|<span data-ttu-id="66162-294">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="66162-294">userPrincipalName</span></span>|<span data-ttu-id="66162-295">String</span><span class="sxs-lookup"><span data-stu-id="66162-295">String</span></span>|<span data-ttu-id="66162-296">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-296">Device user principal name.</span></span> <span data-ttu-id="66162-297">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-297">This property is read-only.</span></span>|
|<span data-ttu-id="66162-298">modelo</span><span class="sxs-lookup"><span data-stu-id="66162-298">model</span></span>|<span data-ttu-id="66162-299">String</span><span class="sxs-lookup"><span data-stu-id="66162-299">String</span></span>|<span data-ttu-id="66162-300">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-300">Model of the device.</span></span> <span data-ttu-id="66162-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-301">This property is read-only.</span></span>|
|<span data-ttu-id="66162-302">fabricante</span><span class="sxs-lookup"><span data-stu-id="66162-302">manufacturer</span></span>|<span data-ttu-id="66162-303">String</span><span class="sxs-lookup"><span data-stu-id="66162-303">String</span></span>|<span data-ttu-id="66162-304">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-304">Manufacturer of the device.</span></span> <span data-ttu-id="66162-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-305">This property is read-only.</span></span>|
|<span data-ttu-id="66162-306">imei</span><span class="sxs-lookup"><span data-stu-id="66162-306">imei</span></span>|<span data-ttu-id="66162-307">String</span><span class="sxs-lookup"><span data-stu-id="66162-307">String</span></span>|<span data-ttu-id="66162-308">IMEI.</span><span class="sxs-lookup"><span data-stu-id="66162-308">IMEI.</span></span> <span data-ttu-id="66162-309">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-309">This property is read-only.</span></span>|
|<span data-ttu-id="66162-310">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-310">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="66162-311">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-311">DateTimeOffset</span></span>|<span data-ttu-id="66162-312">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="66162-312">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="66162-313">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-313">This property is read-only.</span></span>|
|<span data-ttu-id="66162-314">serialNumber</span><span class="sxs-lookup"><span data-stu-id="66162-314">serialNumber</span></span>|<span data-ttu-id="66162-315">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66162-315">String</span></span>|<span data-ttu-id="66162-316">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="66162-316">SerialNumber.</span></span> <span data-ttu-id="66162-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-317">This property is read-only.</span></span>|
|<span data-ttu-id="66162-318">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="66162-318">phoneNumber</span></span>|<span data-ttu-id="66162-319">String</span><span class="sxs-lookup"><span data-stu-id="66162-319">String</span></span>|<span data-ttu-id="66162-320">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-320">Phone number of the device.</span></span> <span data-ttu-id="66162-321">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-321">This property is read-only.</span></span>|
|<span data-ttu-id="66162-322">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="66162-322">androidSecurityPatchLevel</span></span>|<span data-ttu-id="66162-323">String</span><span class="sxs-lookup"><span data-stu-id="66162-323">String</span></span>|<span data-ttu-id="66162-324">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="66162-324">Android security patch level.</span></span> <span data-ttu-id="66162-325">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-325">This property is read-only.</span></span>|
|<span data-ttu-id="66162-326">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="66162-326">userDisplayName</span></span>|<span data-ttu-id="66162-327">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66162-327">String</span></span>|<span data-ttu-id="66162-328">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="66162-328">User display name.</span></span> <span data-ttu-id="66162-329">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-329">This property is read-only.</span></span>|
|<span data-ttu-id="66162-330">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="66162-330">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="66162-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="66162-331">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="66162-332">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="66162-332">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="66162-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-333">This property is read-only.</span></span>|
|<span data-ttu-id="66162-334">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="66162-334">wiFiMacAddress</span></span>|<span data-ttu-id="66162-335">String</span><span class="sxs-lookup"><span data-stu-id="66162-335">String</span></span>|<span data-ttu-id="66162-336">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="66162-336">Wi-Fi MAC.</span></span> <span data-ttu-id="66162-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-337">This property is read-only.</span></span>|
|<span data-ttu-id="66162-338">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="66162-338">deviceHealthAttestationState</span></span>|[<span data-ttu-id="66162-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="66162-339">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="66162-340">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-340">The device health attestation state.</span></span> <span data-ttu-id="66162-341">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-341">This property is read-only.</span></span>|
|<span data-ttu-id="66162-342">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="66162-342">subscriberCarrier</span></span>|<span data-ttu-id="66162-343">String</span><span class="sxs-lookup"><span data-stu-id="66162-343">String</span></span>|<span data-ttu-id="66162-344">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="66162-344">Subscriber Carrier.</span></span> <span data-ttu-id="66162-345">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-345">This property is read-only.</span></span>|
|<span data-ttu-id="66162-346">meid</span><span class="sxs-lookup"><span data-stu-id="66162-346">meid</span></span>|<span data-ttu-id="66162-347">String</span><span class="sxs-lookup"><span data-stu-id="66162-347">String</span></span>|<span data-ttu-id="66162-348">MEID.</span><span class="sxs-lookup"><span data-stu-id="66162-348">MEID.</span></span> <span data-ttu-id="66162-349">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-349">This property is read-only.</span></span>|
|<span data-ttu-id="66162-350">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="66162-350">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="66162-351">Int64</span><span class="sxs-lookup"><span data-stu-id="66162-351">Int64</span></span>|<span data-ttu-id="66162-352">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="66162-352">Total Storage in Bytes.</span></span> <span data-ttu-id="66162-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-353">This property is read-only.</span></span>|
|<span data-ttu-id="66162-354">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="66162-354">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="66162-355">Int64</span><span class="sxs-lookup"><span data-stu-id="66162-355">Int64</span></span>|<span data-ttu-id="66162-356">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="66162-356">Free Storage in Bytes.</span></span> <span data-ttu-id="66162-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-357">This property is read-only.</span></span>|
|<span data-ttu-id="66162-358">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="66162-358">managedDeviceName</span></span>|<span data-ttu-id="66162-359">String</span><span class="sxs-lookup"><span data-stu-id="66162-359">String</span></span>|<span data-ttu-id="66162-360">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-360">Automatically generated name to identify a device.</span></span> <span data-ttu-id="66162-361">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="66162-361">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="66162-362">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="66162-362">partnerReportedThreatState</span></span>|[<span data-ttu-id="66162-363">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="66162-363">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="66162-364">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-364">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="66162-365">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-365">Read Only.</span></span> <span data-ttu-id="66162-366">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-366">This property is read-only.</span></span> <span data-ttu-id="66162-367">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="66162-367">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="66162-368">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-368">retireAfterDateTime</span></span>|<span data-ttu-id="66162-369">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-369">DateTimeOffset</span></span>|<span data-ttu-id="66162-370">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="66162-370">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="66162-371">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-371">This property is read-only.</span></span>|
|<span data-ttu-id="66162-372">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="66162-372">usersLoggedOn</span></span>|<span data-ttu-id="66162-373">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="66162-373">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="66162-374">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-374">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="66162-375">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-375">This property is read-only.</span></span>|
|<span data-ttu-id="66162-376">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="66162-376">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="66162-377">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-377">DateTimeOffset</span></span>|<span data-ttu-id="66162-378">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="66162-378">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="66162-379">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="66162-379">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="66162-380">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-380">Read Only.</span></span> <span data-ttu-id="66162-381">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-381">This property is read-only.</span></span>|
|<span data-ttu-id="66162-382">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="66162-382">autopilotEnrolled</span></span>|<span data-ttu-id="66162-383">Booliano</span><span class="sxs-lookup"><span data-stu-id="66162-383">Boolean</span></span>|<span data-ttu-id="66162-384">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="66162-384">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="66162-385">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-385">This property is read-only.</span></span>|
|<span data-ttu-id="66162-386">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="66162-386">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="66162-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="66162-387">Boolean</span></span>|<span data-ttu-id="66162-388">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="66162-388">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="66162-389">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-389">This property is read-only.</span></span>|
|<span data-ttu-id="66162-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="66162-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="66162-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66162-391">DateTimeOffset</span></span>|<span data-ttu-id="66162-392">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66162-392">Reports device management certificate expiration date.</span></span> <span data-ttu-id="66162-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-393">This property is read-only.</span></span>|
|<span data-ttu-id="66162-394">iccid</span><span class="sxs-lookup"><span data-stu-id="66162-394">iccid</span></span>|<span data-ttu-id="66162-395">String</span><span class="sxs-lookup"><span data-stu-id="66162-395">String</span></span>|<span data-ttu-id="66162-396">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="66162-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="66162-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-397">This property is read-only.</span></span>|
|<span data-ttu-id="66162-398">udid</span><span class="sxs-lookup"><span data-stu-id="66162-398">udid</span></span>|<span data-ttu-id="66162-399">String</span><span class="sxs-lookup"><span data-stu-id="66162-399">String</span></span>|<span data-ttu-id="66162-400">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="66162-400">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="66162-401">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-401">This property is read-only.</span></span>|
|<span data-ttu-id="66162-402">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66162-402">roleScopeTagIds</span></span>|<span data-ttu-id="66162-403">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="66162-403">String collection</span></span>|<span data-ttu-id="66162-404">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66162-404">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="66162-405">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="66162-405">windowsActiveMalwareCount</span></span>|<span data-ttu-id="66162-406">Int32</span><span class="sxs-lookup"><span data-stu-id="66162-406">Int32</span></span>|<span data-ttu-id="66162-407">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="66162-407">Count of active malware for this windows device.</span></span> <span data-ttu-id="66162-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-408">This property is read-only.</span></span>|
|<span data-ttu-id="66162-409">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="66162-409">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="66162-410">Int32</span><span class="sxs-lookup"><span data-stu-id="66162-410">Int32</span></span>|<span data-ttu-id="66162-411">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="66162-411">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="66162-412">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-412">This property is read-only.</span></span>|
|<span data-ttu-id="66162-413">notes</span><span class="sxs-lookup"><span data-stu-id="66162-413">notes</span></span>|<span data-ttu-id="66162-414">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66162-414">String</span></span>|<span data-ttu-id="66162-415">Observações sobre o dispositivo criado pelo administrador de ti</span><span class="sxs-lookup"><span data-stu-id="66162-415">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="66162-416">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="66162-416">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="66162-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="66162-417">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="66162-418">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="66162-418">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="66162-419">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="66162-419">configurationManagerClientInformation</span></span>|[<span data-ttu-id="66162-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="66162-420">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="66162-421">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="66162-421">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="66162-422">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="66162-422">ethernetMacAddress</span></span>|<span data-ttu-id="66162-423">String</span><span class="sxs-lookup"><span data-stu-id="66162-423">String</span></span>|<span data-ttu-id="66162-424">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="66162-424">Ethernet MAC.</span></span> <span data-ttu-id="66162-425">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-425">This property is read-only.</span></span>|
|<span data-ttu-id="66162-426">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="66162-426">physicalMemoryInBytes</span></span>|<span data-ttu-id="66162-427">Int64</span><span class="sxs-lookup"><span data-stu-id="66162-427">Int64</span></span>|<span data-ttu-id="66162-428">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="66162-428">Total Memory in Bytes.</span></span> <span data-ttu-id="66162-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-429">This property is read-only.</span></span>|
|<span data-ttu-id="66162-430">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="66162-430">processorArchitecture</span></span>|[<span data-ttu-id="66162-431">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="66162-431">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="66162-432">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="66162-432">Processor architecture.</span></span> <span data-ttu-id="66162-433">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66162-433">This property is read-only.</span></span> <span data-ttu-id="66162-434">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="66162-434">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="66162-435">Resposta</span><span class="sxs-lookup"><span data-stu-id="66162-435">Response</span></span>
<span data-ttu-id="66162-436">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66162-436">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66162-437">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66162-437">Example</span></span>

### <a name="request"></a><span data-ttu-id="66162-438">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66162-438">Request</span></span>
<span data-ttu-id="66162-439">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66162-439">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7634

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
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="66162-440">Resposta</span><span class="sxs-lookup"><span data-stu-id="66162-440">Response</span></span>
<span data-ttu-id="66162-p170">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66162-p170">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7683

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
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```





