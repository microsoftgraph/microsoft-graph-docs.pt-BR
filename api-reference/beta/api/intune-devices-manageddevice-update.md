---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 701aa64718a2c33ebd651fa58847819ce030dd2c
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176418"
---
# <a name="update-manageddevice"></a><span data-ttu-id="0d82d-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="0d82d-103">Update managedDevice</span></span>

<span data-ttu-id="0d82d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d82d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d82d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d82d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d82d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d82d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d82d-107">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0d82d-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d82d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d82d-108">Prerequisites</span></span>
<span data-ttu-id="0d82d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d82d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d82d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d82d-111">Permission type</span></span>|<span data-ttu-id="0d82d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d82d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d82d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d82d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d82d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d82d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0d82d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d82d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d82d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d82d-116">Not supported.</span></span>|
|<span data-ttu-id="0d82d-117">Application</span><span class="sxs-lookup"><span data-stu-id="0d82d-117">Application</span></span>|<span data-ttu-id="0d82d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d82d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d82d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d82d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0d82d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d82d-120">Request headers</span></span>
|<span data-ttu-id="0d82d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d82d-121">Header</span></span>|<span data-ttu-id="0d82d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d82d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d82d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d82d-123">Authorization</span></span>|<span data-ttu-id="0d82d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d82d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d82d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d82d-125">Accept</span></span>|<span data-ttu-id="0d82d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d82d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d82d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d82d-127">Request body</span></span>
<span data-ttu-id="0d82d-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0d82d-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="0d82d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0d82d-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="0d82d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d82d-130">Property</span></span>|<span data-ttu-id="0d82d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d82d-131">Type</span></span>|<span data-ttu-id="0d82d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d82d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d82d-133">id</span><span class="sxs-lookup"><span data-stu-id="0d82d-133">id</span></span>|<span data-ttu-id="0d82d-134">String</span><span class="sxs-lookup"><span data-stu-id="0d82d-134">String</span></span>|<span data-ttu-id="0d82d-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-135">Unique Identifier for the device.</span></span> <span data-ttu-id="0d82d-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-136">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-137">userId</span><span class="sxs-lookup"><span data-stu-id="0d82d-137">userId</span></span>|<span data-ttu-id="0d82d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-138">String</span></span>|<span data-ttu-id="0d82d-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="0d82d-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-140">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="0d82d-141">deviceName</span></span>|<span data-ttu-id="0d82d-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-142">String</span></span>|<span data-ttu-id="0d82d-143">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-143">Name of the device.</span></span> <span data-ttu-id="0d82d-144">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-144">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-145">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0d82d-145">hardwareInformation</span></span>|[<span data-ttu-id="0d82d-146">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="0d82d-146">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="0d82d-147">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-147">The hardward details for the device.</span></span>  <span data-ttu-id="0d82d-148">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-148">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-149">ownerType</span><span class="sxs-lookup"><span data-stu-id="0d82d-149">ownerType</span></span>|[<span data-ttu-id="0d82d-150">ownerType</span><span class="sxs-lookup"><span data-stu-id="0d82d-150">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="0d82d-151">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-151">Ownership of the device.</span></span> <span data-ttu-id="0d82d-152">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="0d82d-152">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0d82d-153">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-153">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0d82d-154">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0d82d-154">managedDeviceOwnerType</span></span>|[<span data-ttu-id="0d82d-155">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="0d82d-155">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="0d82d-156">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-156">Ownership of the device.</span></span> <span data-ttu-id="0d82d-157">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="0d82d-157">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="0d82d-158">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-158">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0d82d-159">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0d82d-159">deviceActionResults</span></span>|<span data-ttu-id="0d82d-160">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0d82d-160">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="0d82d-161">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="0d82d-161">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="0d82d-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-162">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-163">ManagementState</span><span class="sxs-lookup"><span data-stu-id="0d82d-163">managementState</span></span>|[<span data-ttu-id="0d82d-164">ManagementState</span><span class="sxs-lookup"><span data-stu-id="0d82d-164">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="0d82d-165">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-165">Management state of the device.</span></span> <span data-ttu-id="0d82d-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-166">This property is read-only.</span></span> <span data-ttu-id="0d82d-167">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-167">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="0d82d-168">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-168">enrolledDateTime</span></span>|<span data-ttu-id="0d82d-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-169">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-170">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-170">Enrollment time of the device.</span></span> <span data-ttu-id="0d82d-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-171">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-172">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-172">lastSyncDateTime</span></span>|<span data-ttu-id="0d82d-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-173">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-174">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="0d82d-174">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="0d82d-175">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-175">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-176">chassisType</span><span class="sxs-lookup"><span data-stu-id="0d82d-176">chassisType</span></span>|[<span data-ttu-id="0d82d-177">chassisType</span><span class="sxs-lookup"><span data-stu-id="0d82d-177">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="0d82d-178">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-178">Chassis type of the device.</span></span> <span data-ttu-id="0d82d-179">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-179">This property is read-only.</span></span> <span data-ttu-id="0d82d-180">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-180">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="0d82d-181">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d82d-181">operatingSystem</span></span>|<span data-ttu-id="0d82d-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-182">String</span></span>|<span data-ttu-id="0d82d-183">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-183">Operating system of the device.</span></span> <span data-ttu-id="0d82d-184">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-184">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-185">deviceType</span><span class="sxs-lookup"><span data-stu-id="0d82d-185">deviceType</span></span>|[<span data-ttu-id="0d82d-186">deviceType</span><span class="sxs-lookup"><span data-stu-id="0d82d-186">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0d82d-187">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-187">Platform of the device.</span></span> <span data-ttu-id="0d82d-188">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-188">This property is read-only.</span></span> <span data-ttu-id="0d82d-189">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="0d82d-189">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0d82d-190">complianceState</span><span class="sxs-lookup"><span data-stu-id="0d82d-190">complianceState</span></span>|[<span data-ttu-id="0d82d-191">complianceState</span><span class="sxs-lookup"><span data-stu-id="0d82d-191">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="0d82d-192">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-192">Compliance state of the device.</span></span> <span data-ttu-id="0d82d-193">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-193">This property is read-only.</span></span> <span data-ttu-id="0d82d-194">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-194">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0d82d-195">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0d82d-195">jailBroken</span></span>|<span data-ttu-id="0d82d-196">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-196">String</span></span>|<span data-ttu-id="0d82d-197">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="0d82d-197">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="0d82d-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-198">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-199">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0d82d-199">managementAgent</span></span>|[<span data-ttu-id="0d82d-200">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="0d82d-200">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="0d82d-201">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-201">Management channel of the device.</span></span> <span data-ttu-id="0d82d-202">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-202">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="0d82d-203">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-203">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="0d82d-204">osVersion</span><span class="sxs-lookup"><span data-stu-id="0d82d-204">osVersion</span></span>|<span data-ttu-id="0d82d-205">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-205">String</span></span>|<span data-ttu-id="0d82d-206">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-206">Operating system version of the device.</span></span> <span data-ttu-id="0d82d-207">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-207">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-208">easActivated</span><span class="sxs-lookup"><span data-stu-id="0d82d-208">easActivated</span></span>|<span data-ttu-id="0d82d-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-209">Boolean</span></span>|<span data-ttu-id="0d82d-210">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0d82d-210">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="0d82d-211">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-211">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-212">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0d82d-212">easDeviceId</span></span>|<span data-ttu-id="0d82d-213">String</span><span class="sxs-lookup"><span data-stu-id="0d82d-213">String</span></span>|<span data-ttu-id="0d82d-214">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-214">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="0d82d-215">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-215">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-216">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-216">easActivationDateTime</span></span>|<span data-ttu-id="0d82d-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-217">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-218">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-218">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="0d82d-219">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-219">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-220">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="0d82d-220">aadRegistered</span></span>|<span data-ttu-id="0d82d-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-221">Boolean</span></span>|<span data-ttu-id="0d82d-222">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d82d-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="0d82d-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-223">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-224">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0d82d-224">azureADRegistered</span></span>|<span data-ttu-id="0d82d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-225">Boolean</span></span>|<span data-ttu-id="0d82d-226">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d82d-226">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="0d82d-227">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-227">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-228">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0d82d-228">deviceEnrollmentType</span></span>|[<span data-ttu-id="0d82d-229">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0d82d-229">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="0d82d-230">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-230">Enrollment type of the device.</span></span> <span data-ttu-id="0d82d-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-231">This property is read-only.</span></span> <span data-ttu-id="0d82d-232">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-232">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="0d82d-233">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0d82d-233">lostModeState</span></span>|[<span data-ttu-id="0d82d-234">lostModeState</span><span class="sxs-lookup"><span data-stu-id="0d82d-234">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="0d82d-235">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="0d82d-235">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="0d82d-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-236">This property is read-only.</span></span> <span data-ttu-id="0d82d-237">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-237">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="0d82d-238">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0d82d-238">activationLockBypassCode</span></span>|<span data-ttu-id="0d82d-239">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-239">String</span></span>|<span data-ttu-id="0d82d-240">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="0d82d-240">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="0d82d-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-241">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-242">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0d82d-242">emailAddress</span></span>|<span data-ttu-id="0d82d-243">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-243">String</span></span>|<span data-ttu-id="0d82d-244">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-244">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="0d82d-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-245">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-246">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="0d82d-246">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="0d82d-247">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-247">String</span></span>|<span data-ttu-id="0d82d-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d82d-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0d82d-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-249">Read only.</span></span> <span data-ttu-id="0d82d-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-250">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-251">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0d82d-251">azureADDeviceId</span></span>|<span data-ttu-id="0d82d-252">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-252">String</span></span>|<span data-ttu-id="0d82d-253">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d82d-253">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0d82d-254">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-254">Read only.</span></span> <span data-ttu-id="0d82d-255">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-255">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-256">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0d82d-256">deviceRegistrationState</span></span>|[<span data-ttu-id="0d82d-257">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0d82d-257">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="0d82d-258">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-258">Device registration state.</span></span> <span data-ttu-id="0d82d-259">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-259">This property is read-only.</span></span> <span data-ttu-id="0d82d-260">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-260">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="0d82d-261">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0d82d-261">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0d82d-262">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-262">String</span></span>|<span data-ttu-id="0d82d-263">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-263">Device category display name.</span></span> <span data-ttu-id="0d82d-264">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-264">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-265">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0d82d-265">isSupervised</span></span>|<span data-ttu-id="0d82d-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-266">Boolean</span></span>|<span data-ttu-id="0d82d-267">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-267">Device supervised status.</span></span> <span data-ttu-id="0d82d-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-268">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-269">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-269">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0d82d-270">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-270">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-271">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d82d-271">Last time the device contacted Exchange.</span></span> <span data-ttu-id="0d82d-272">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-272">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-273">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0d82d-273">exchangeAccessState</span></span>|[<span data-ttu-id="0d82d-274">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0d82d-274">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="0d82d-275">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d82d-275">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0d82d-276">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-276">This property is read-only.</span></span> <span data-ttu-id="0d82d-277">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-277">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0d82d-278">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0d82d-278">exchangeAccessStateReason</span></span>|[<span data-ttu-id="0d82d-279">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0d82d-279">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="0d82d-280">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d82d-280">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0d82d-281">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-281">This property is read-only.</span></span> <span data-ttu-id="0d82d-282">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-282">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0d82d-283">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0d82d-283">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0d82d-284">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-284">String</span></span>|<span data-ttu-id="0d82d-285">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-285">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="0d82d-286">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-286">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-287">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0d82d-287">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0d82d-288">String</span><span class="sxs-lookup"><span data-stu-id="0d82d-288">String</span></span>|<span data-ttu-id="0d82d-289">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="0d82d-289">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="0d82d-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-290">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-291">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0d82d-291">isEncrypted</span></span>|<span data-ttu-id="0d82d-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-292">Boolean</span></span>|<span data-ttu-id="0d82d-293">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-293">Device encryption status.</span></span> <span data-ttu-id="0d82d-294">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-294">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-295">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0d82d-295">userPrincipalName</span></span>|<span data-ttu-id="0d82d-296">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-296">String</span></span>|<span data-ttu-id="0d82d-297">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-297">Device user principal name.</span></span> <span data-ttu-id="0d82d-298">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-298">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-299">modelo</span><span class="sxs-lookup"><span data-stu-id="0d82d-299">model</span></span>|<span data-ttu-id="0d82d-300">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-300">String</span></span>|<span data-ttu-id="0d82d-301">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-301">Model of the device.</span></span> <span data-ttu-id="0d82d-302">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-302">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-303">fabricante</span><span class="sxs-lookup"><span data-stu-id="0d82d-303">manufacturer</span></span>|<span data-ttu-id="0d82d-304">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-304">String</span></span>|<span data-ttu-id="0d82d-305">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-305">Manufacturer of the device.</span></span> <span data-ttu-id="0d82d-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-306">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-307">imei</span><span class="sxs-lookup"><span data-stu-id="0d82d-307">imei</span></span>|<span data-ttu-id="0d82d-308">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-308">String</span></span>|<span data-ttu-id="0d82d-309">IMEI.</span><span class="sxs-lookup"><span data-stu-id="0d82d-309">IMEI.</span></span> <span data-ttu-id="0d82d-310">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-310">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-311">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-311">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0d82d-312">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-312">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-313">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="0d82d-313">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="0d82d-314">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-314">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-315">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0d82d-315">serialNumber</span></span>|<span data-ttu-id="0d82d-316">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-316">String</span></span>|<span data-ttu-id="0d82d-317">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="0d82d-317">SerialNumber.</span></span> <span data-ttu-id="0d82d-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-318">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-319">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0d82d-319">phoneNumber</span></span>|<span data-ttu-id="0d82d-320">String</span><span class="sxs-lookup"><span data-stu-id="0d82d-320">String</span></span>|<span data-ttu-id="0d82d-321">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-321">Phone number of the device.</span></span> <span data-ttu-id="0d82d-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-322">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-323">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0d82d-323">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0d82d-324">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-324">String</span></span>|<span data-ttu-id="0d82d-325">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="0d82d-325">Android security patch level.</span></span> <span data-ttu-id="0d82d-326">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-326">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-327">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0d82d-327">userDisplayName</span></span>|<span data-ttu-id="0d82d-328">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-328">String</span></span>|<span data-ttu-id="0d82d-329">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d82d-329">User display name.</span></span> <span data-ttu-id="0d82d-330">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-330">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-331">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0d82d-331">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0d82d-332">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0d82d-332">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0d82d-333">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="0d82d-333">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="0d82d-334">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-334">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-335">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0d82d-335">wiFiMacAddress</span></span>|<span data-ttu-id="0d82d-336">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-336">String</span></span>|<span data-ttu-id="0d82d-337">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="0d82d-337">Wi-Fi MAC.</span></span> <span data-ttu-id="0d82d-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-338">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-339">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0d82d-339">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0d82d-340">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0d82d-340">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="0d82d-341">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-341">The device health attestation state.</span></span> <span data-ttu-id="0d82d-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-342">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-343">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0d82d-343">subscriberCarrier</span></span>|<span data-ttu-id="0d82d-344">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-344">String</span></span>|<span data-ttu-id="0d82d-345">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="0d82d-345">Subscriber Carrier.</span></span> <span data-ttu-id="0d82d-346">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-346">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-347">meid</span><span class="sxs-lookup"><span data-stu-id="0d82d-347">meid</span></span>|<span data-ttu-id="0d82d-348">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-348">String</span></span>|<span data-ttu-id="0d82d-349">MEID.</span><span class="sxs-lookup"><span data-stu-id="0d82d-349">MEID.</span></span> <span data-ttu-id="0d82d-350">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-350">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-351">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0d82d-351">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0d82d-352">Int64</span><span class="sxs-lookup"><span data-stu-id="0d82d-352">Int64</span></span>|<span data-ttu-id="0d82d-353">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="0d82d-353">Total Storage in Bytes.</span></span> <span data-ttu-id="0d82d-354">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-354">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-355">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0d82d-355">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0d82d-356">Int64</span><span class="sxs-lookup"><span data-stu-id="0d82d-356">Int64</span></span>|<span data-ttu-id="0d82d-357">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="0d82d-357">Free Storage in Bytes.</span></span> <span data-ttu-id="0d82d-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-358">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-359">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0d82d-359">managedDeviceName</span></span>|<span data-ttu-id="0d82d-360">String</span><span class="sxs-lookup"><span data-stu-id="0d82d-360">String</span></span>|<span data-ttu-id="0d82d-361">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-361">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0d82d-362">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="0d82d-362">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0d82d-363">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0d82d-363">partnerReportedThreatState</span></span>|[<span data-ttu-id="0d82d-364">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="0d82d-364">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="0d82d-365">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-365">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0d82d-366">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-366">Read Only.</span></span> <span data-ttu-id="0d82d-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-367">This property is read-only.</span></span> <span data-ttu-id="0d82d-368">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-368">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="0d82d-369">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-369">retireAfterDateTime</span></span>|<span data-ttu-id="0d82d-370">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-370">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-371">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="0d82d-371">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="0d82d-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-372">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-373">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="0d82d-373">usersLoggedOn</span></span>|<span data-ttu-id="0d82d-374">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="0d82d-374">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="0d82d-375">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-375">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="0d82d-376">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-376">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-377">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d82d-377">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="0d82d-378">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-378">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-379">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="0d82d-379">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="0d82d-380">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="0d82d-380">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="0d82d-381">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-381">Read Only.</span></span> <span data-ttu-id="0d82d-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-382">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-383">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="0d82d-383">autopilotEnrolled</span></span>|<span data-ttu-id="0d82d-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-384">Boolean</span></span>|<span data-ttu-id="0d82d-385">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="0d82d-385">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="0d82d-386">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-386">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="0d82d-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="0d82d-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d82d-388">Boolean</span></span>|<span data-ttu-id="0d82d-389">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d82d-389">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="0d82d-390">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-390">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0d82d-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="0d82d-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d82d-392">DateTimeOffset</span></span>|<span data-ttu-id="0d82d-393">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0d82d-393">Reports device management certificate expiration date.</span></span> <span data-ttu-id="0d82d-394">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-394">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-395">iccid</span><span class="sxs-lookup"><span data-stu-id="0d82d-395">iccid</span></span>|<span data-ttu-id="0d82d-396">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-396">String</span></span>|<span data-ttu-id="0d82d-397">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="0d82d-397">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="0d82d-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-398">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-399">udid</span><span class="sxs-lookup"><span data-stu-id="0d82d-399">udid</span></span>|<span data-ttu-id="0d82d-400">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-400">String</span></span>|<span data-ttu-id="0d82d-401">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="0d82d-401">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="0d82d-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-402">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-403">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d82d-403">roleScopeTagIds</span></span>|<span data-ttu-id="0d82d-404">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-404">String collection</span></span>|<span data-ttu-id="0d82d-405">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-405">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="0d82d-406">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="0d82d-406">windowsActiveMalwareCount</span></span>|<span data-ttu-id="0d82d-407">Int32</span><span class="sxs-lookup"><span data-stu-id="0d82d-407">Int32</span></span>|<span data-ttu-id="0d82d-408">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="0d82d-408">Count of active malware for this windows device.</span></span> <span data-ttu-id="0d82d-409">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-409">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-410">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="0d82d-410">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="0d82d-411">Int32</span><span class="sxs-lookup"><span data-stu-id="0d82d-411">Int32</span></span>|<span data-ttu-id="0d82d-412">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="0d82d-412">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="0d82d-413">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-413">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-414">notes</span><span class="sxs-lookup"><span data-stu-id="0d82d-414">notes</span></span>|<span data-ttu-id="0d82d-415">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-415">String</span></span>|<span data-ttu-id="0d82d-416">Observações sobre o dispositivo criado pelo administrador de ti</span><span class="sxs-lookup"><span data-stu-id="0d82d-416">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="0d82d-417">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0d82d-417">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="0d82d-418">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="0d82d-418">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="0d82d-419">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="0d82d-419">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="0d82d-420">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="0d82d-420">configurationManagerClientInformation</span></span>|[<span data-ttu-id="0d82d-421">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="0d82d-421">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="0d82d-422">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="0d82d-422">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|
|<span data-ttu-id="0d82d-423">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="0d82d-423">ethernetMacAddress</span></span>|<span data-ttu-id="0d82d-424">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-424">String</span></span>|<span data-ttu-id="0d82d-425">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="0d82d-425">Ethernet MAC.</span></span> <span data-ttu-id="0d82d-426">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-426">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-427">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="0d82d-427">physicalMemoryInBytes</span></span>|<span data-ttu-id="0d82d-428">Int64</span><span class="sxs-lookup"><span data-stu-id="0d82d-428">Int64</span></span>|<span data-ttu-id="0d82d-429">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="0d82d-429">Total Memory in Bytes.</span></span> <span data-ttu-id="0d82d-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-430">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-431">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="0d82d-431">processorArchitecture</span></span>|[<span data-ttu-id="0d82d-432">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="0d82d-432">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="0d82d-433">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="0d82d-433">Processor architecture.</span></span> <span data-ttu-id="0d82d-434">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-434">This property is read-only.</span></span> <span data-ttu-id="0d82d-435">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-435">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="0d82d-436">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="0d82d-436">specificationVersion</span></span>|<span data-ttu-id="0d82d-437">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-437">String</span></span>|<span data-ttu-id="0d82d-438">Versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="0d82d-438">Specification version.</span></span> <span data-ttu-id="0d82d-439">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d82d-439">This property is read-only.</span></span>|
|<span data-ttu-id="0d82d-440">JoinType</span><span class="sxs-lookup"><span data-stu-id="0d82d-440">joinType</span></span>|[<span data-ttu-id="0d82d-441">JoinType</span><span class="sxs-lookup"><span data-stu-id="0d82d-441">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="0d82d-442">Tipo de ingresso de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d82d-442">Device join type.</span></span> <span data-ttu-id="0d82d-443">Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="0d82d-443">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="0d82d-444">skuFamily</span><span class="sxs-lookup"><span data-stu-id="0d82d-444">skuFamily</span></span>|<span data-ttu-id="0d82d-445">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0d82d-445">String</span></span>|<span data-ttu-id="0d82d-446">Família de SKU do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d82d-446">Device sku family</span></span>|



## <a name="response"></a><span data-ttu-id="0d82d-447">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d82d-447">Response</span></span>
<span data-ttu-id="0d82d-448">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d82d-448">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d82d-449">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d82d-449">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d82d-450">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d82d-450">Request</span></span>
<span data-ttu-id="0d82d-451">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d82d-451">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d82d-452">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d82d-452">Response</span></span>
<span data-ttu-id="0d82d-p172">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d82d-p172">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



