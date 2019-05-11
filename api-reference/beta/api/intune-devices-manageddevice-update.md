---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0dd5c42bd6dba6208ea06c2f85efce1e7972d6eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909586"
---
# <a name="update-manageddevice"></a><span data-ttu-id="994e3-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="994e3-103">Update managedDevice</span></span>

> <span data-ttu-id="994e3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="994e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="994e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="994e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="994e3-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="994e3-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="994e3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="994e3-107">Prerequisites</span></span>
<span data-ttu-id="994e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="994e3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="994e3-110">Permission type</span></span>|<span data-ttu-id="994e3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="994e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="994e3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="994e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="994e3-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994e3-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="994e3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="994e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="994e3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="994e3-115">Not supported.</span></span>|
|<span data-ttu-id="994e3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="994e3-116">Application</span></span>|<span data-ttu-id="994e3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="994e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="994e3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="994e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="994e3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="994e3-119">Request headers</span></span>
|<span data-ttu-id="994e3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="994e3-120">Header</span></span>|<span data-ttu-id="994e3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="994e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="994e3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="994e3-122">Authorization</span></span>|<span data-ttu-id="994e3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="994e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="994e3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="994e3-124">Accept</span></span>|<span data-ttu-id="994e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="994e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="994e3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="994e3-126">Request body</span></span>
<span data-ttu-id="994e3-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="994e3-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="994e3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="994e3-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="994e3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="994e3-129">Property</span></span>|<span data-ttu-id="994e3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="994e3-130">Type</span></span>|<span data-ttu-id="994e3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="994e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="994e3-132">id</span><span class="sxs-lookup"><span data-stu-id="994e3-132">id</span></span>|<span data-ttu-id="994e3-133">String</span><span class="sxs-lookup"><span data-stu-id="994e3-133">String</span></span>|<span data-ttu-id="994e3-134">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="994e3-135">userId</span><span class="sxs-lookup"><span data-stu-id="994e3-135">userId</span></span>|<span data-ttu-id="994e3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-136">String</span></span>|<span data-ttu-id="994e3-137">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="994e3-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="994e3-138">deviceName</span></span>|<span data-ttu-id="994e3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-139">String</span></span>|<span data-ttu-id="994e3-140">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-140">Name of the device</span></span>|
|<span data-ttu-id="994e3-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="994e3-141">hardwareInformation</span></span>|[<span data-ttu-id="994e3-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="994e3-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="994e3-143">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-143">The hardward details for the device.</span></span>  <span data-ttu-id="994e3-144">Inclui informações como espaço de armazenamento, fabricante, número de série, etc.</span><span class="sxs-lookup"><span data-stu-id="994e3-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="994e3-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="994e3-145">ownerType</span></span>|[<span data-ttu-id="994e3-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="994e3-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="994e3-147">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-147">Ownership of the device.</span></span> <span data-ttu-id="994e3-148">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="994e3-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="994e3-149">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="994e3-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="994e3-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="994e3-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="994e3-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="994e3-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="994e3-152">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-152">Ownership of the device.</span></span> <span data-ttu-id="994e3-153">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="994e3-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="994e3-154">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="994e3-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="994e3-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="994e3-155">deviceActionResults</span></span>|<span data-ttu-id="994e3-156">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="994e3-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="994e3-157">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="994e3-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="994e3-158">ManagementState</span><span class="sxs-lookup"><span data-stu-id="994e3-158">managementState</span></span>|[<span data-ttu-id="994e3-159">ManagementState</span><span class="sxs-lookup"><span data-stu-id="994e3-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="994e3-160">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-160">Management state of the device.</span></span> <span data-ttu-id="994e3-161">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="994e3-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="994e3-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-162">enrolledDateTime</span></span>|<span data-ttu-id="994e3-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-163">DateTimeOffset</span></span>|<span data-ttu-id="994e3-164">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="994e3-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-165">lastSyncDateTime</span></span>|<span data-ttu-id="994e3-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-166">DateTimeOffset</span></span>|<span data-ttu-id="994e3-167">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="994e3-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="994e3-168">chassisType</span><span class="sxs-lookup"><span data-stu-id="994e3-168">chassisType</span></span>|[<span data-ttu-id="994e3-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="994e3-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="994e3-170">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-170">Chassis type of the device.</span></span> <span data-ttu-id="994e3-171">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="994e3-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="994e3-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="994e3-172">operatingSystem</span></span>|<span data-ttu-id="994e3-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-173">String</span></span>|<span data-ttu-id="994e3-174">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-174">Operating system of the device.</span></span> <span data-ttu-id="994e3-175">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="994e3-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="994e3-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="994e3-176">deviceType</span></span>|[<span data-ttu-id="994e3-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="994e3-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="994e3-178">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-178">Platform of the device.</span></span> <span data-ttu-id="994e3-179">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="994e3-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="994e3-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="994e3-180">complianceState</span></span>|[<span data-ttu-id="994e3-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="994e3-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="994e3-182">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-182">Compliance state of the device.</span></span> <span data-ttu-id="994e3-183">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="994e3-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="994e3-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="994e3-184">jailBroken</span></span>|<span data-ttu-id="994e3-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-185">String</span></span>|<span data-ttu-id="994e3-186">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="994e3-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="994e3-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="994e3-187">managementAgent</span></span>|[<span data-ttu-id="994e3-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="994e3-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="994e3-189">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-189">Management channel of the device.</span></span> <span data-ttu-id="994e3-190">Intune, EAS, etc. Os valores possíveis são `eas`: `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`,.</span><span class="sxs-lookup"><span data-stu-id="994e3-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="994e3-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="994e3-191">osVersion</span></span>|<span data-ttu-id="994e3-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-192">String</span></span>|<span data-ttu-id="994e3-193">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="994e3-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="994e3-194">easActivated</span></span>|<span data-ttu-id="994e3-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="994e3-195">Boolean</span></span>|<span data-ttu-id="994e3-196">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="994e3-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="994e3-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="994e3-197">easDeviceId</span></span>|<span data-ttu-id="994e3-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-198">String</span></span>|<span data-ttu-id="994e3-199">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="994e3-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-200">easActivationDateTime</span></span>|<span data-ttu-id="994e3-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-201">DateTimeOffset</span></span>|<span data-ttu-id="994e3-202">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="994e3-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="994e3-203">aadRegistered</span></span>|<span data-ttu-id="994e3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="994e3-204">Boolean</span></span>|<span data-ttu-id="994e3-205">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="994e3-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="994e3-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="994e3-206">azureADRegistered</span></span>|<span data-ttu-id="994e3-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="994e3-207">Boolean</span></span>|<span data-ttu-id="994e3-208">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="994e3-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="994e3-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="994e3-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="994e3-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="994e3-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="994e3-211">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-211">Enrollment type of the device.</span></span> <span data-ttu-id="994e3-212">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="994e3-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="994e3-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="994e3-213">lostModeState</span></span>|[<span data-ttu-id="994e3-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="994e3-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="994e3-215">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="994e3-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="994e3-216">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="994e3-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="994e3-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="994e3-217">activationLockBypassCode</span></span>|<span data-ttu-id="994e3-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-218">String</span></span>|<span data-ttu-id="994e3-219">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="994e3-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="994e3-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="994e3-220">emailAddress</span></span>|<span data-ttu-id="994e3-221">String</span><span class="sxs-lookup"><span data-stu-id="994e3-221">String</span></span>|<span data-ttu-id="994e3-222">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="994e3-223">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="994e3-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="994e3-224">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-224">String</span></span>|<span data-ttu-id="994e3-225">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="994e3-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="994e3-226">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="994e3-226">Read only.</span></span>|
|<span data-ttu-id="994e3-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="994e3-227">azureADDeviceId</span></span>|<span data-ttu-id="994e3-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-228">String</span></span>|<span data-ttu-id="994e3-229">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="994e3-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="994e3-230">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="994e3-230">Read only.</span></span>|
|<span data-ttu-id="994e3-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="994e3-231">deviceRegistrationState</span></span>|[<span data-ttu-id="994e3-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="994e3-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="994e3-233">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-233">Device registration state.</span></span> <span data-ttu-id="994e3-234">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="994e3-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="994e3-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="994e3-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="994e3-236">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-236">String</span></span>|<span data-ttu-id="994e3-237">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-237">Device category display name</span></span>|
|<span data-ttu-id="994e3-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="994e3-238">isSupervised</span></span>|<span data-ttu-id="994e3-239">Booliano</span><span class="sxs-lookup"><span data-stu-id="994e3-239">Boolean</span></span>|<span data-ttu-id="994e3-240">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-240">Device supervised status</span></span>|
|<span data-ttu-id="994e3-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="994e3-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-242">DateTimeOffset</span></span>|<span data-ttu-id="994e3-243">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="994e3-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="994e3-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="994e3-244">exchangeAccessState</span></span>|[<span data-ttu-id="994e3-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="994e3-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="994e3-246">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="994e3-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="994e3-247">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="994e3-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="994e3-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="994e3-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="994e3-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="994e3-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="994e3-250">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="994e3-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="994e3-251">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="994e3-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="994e3-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="994e3-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="994e3-253">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-253">String</span></span>|<span data-ttu-id="994e3-254">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="994e3-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="994e3-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="994e3-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-256">String</span></span>|<span data-ttu-id="994e3-257">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="994e3-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="994e3-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="994e3-258">isEncrypted</span></span>|<span data-ttu-id="994e3-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="994e3-259">Boolean</span></span>|<span data-ttu-id="994e3-260">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-260">Device encryption status</span></span>|
|<span data-ttu-id="994e3-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="994e3-261">userPrincipalName</span></span>|<span data-ttu-id="994e3-262">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-262">String</span></span>|<span data-ttu-id="994e3-263">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-263">Device user principal name</span></span>|
|<span data-ttu-id="994e3-264">modelo</span><span class="sxs-lookup"><span data-stu-id="994e3-264">model</span></span>|<span data-ttu-id="994e3-265">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-265">String</span></span>|<span data-ttu-id="994e3-266">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-266">Model of the device</span></span>|
|<span data-ttu-id="994e3-267">fabricante</span><span class="sxs-lookup"><span data-stu-id="994e3-267">manufacturer</span></span>|<span data-ttu-id="994e3-268">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-268">String</span></span>|<span data-ttu-id="994e3-269">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="994e3-270">imei</span><span class="sxs-lookup"><span data-stu-id="994e3-270">imei</span></span>|<span data-ttu-id="994e3-271">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-271">String</span></span>|<span data-ttu-id="994e3-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="994e3-272">IMEI</span></span>|
|<span data-ttu-id="994e3-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="994e3-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-274">DateTimeOffset</span></span>|<span data-ttu-id="994e3-275">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="994e3-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="994e3-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="994e3-276">serialNumber</span></span>|<span data-ttu-id="994e3-277">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-277">String</span></span>|<span data-ttu-id="994e3-278">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="994e3-278">SerialNumber</span></span>|
|<span data-ttu-id="994e3-279">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="994e3-279">phoneNumber</span></span>|<span data-ttu-id="994e3-280">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-280">String</span></span>|<span data-ttu-id="994e3-281">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-281">Phone number of the device</span></span>|
|<span data-ttu-id="994e3-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="994e3-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="994e3-283">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-283">String</span></span>|<span data-ttu-id="994e3-284">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="994e3-284">Android security patch level</span></span>|
|<span data-ttu-id="994e3-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="994e3-285">userDisplayName</span></span>|<span data-ttu-id="994e3-286">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-286">String</span></span>|<span data-ttu-id="994e3-287">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="994e3-287">User display name</span></span>|
|<span data-ttu-id="994e3-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="994e3-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="994e3-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="994e3-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="994e3-290">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="994e3-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="994e3-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="994e3-291">wiFiMacAddress</span></span>|<span data-ttu-id="994e3-292">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-292">String</span></span>|<span data-ttu-id="994e3-293">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="994e3-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="994e3-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="994e3-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="994e3-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="994e3-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="994e3-296">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-296">The device health attestation state.</span></span>|
|<span data-ttu-id="994e3-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="994e3-297">subscriberCarrier</span></span>|<span data-ttu-id="994e3-298">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-298">String</span></span>|<span data-ttu-id="994e3-299">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="994e3-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="994e3-300">meid</span><span class="sxs-lookup"><span data-stu-id="994e3-300">meid</span></span>|<span data-ttu-id="994e3-301">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-301">String</span></span>|<span data-ttu-id="994e3-302">MEID</span><span class="sxs-lookup"><span data-stu-id="994e3-302">MEID</span></span>|
|<span data-ttu-id="994e3-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="994e3-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="994e3-304">Int64</span><span class="sxs-lookup"><span data-stu-id="994e3-304">Int64</span></span>|<span data-ttu-id="994e3-305">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="994e3-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="994e3-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="994e3-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="994e3-307">Int64</span><span class="sxs-lookup"><span data-stu-id="994e3-307">Int64</span></span>|<span data-ttu-id="994e3-308">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="994e3-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="994e3-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="994e3-309">managedDeviceName</span></span>|<span data-ttu-id="994e3-310">String</span><span class="sxs-lookup"><span data-stu-id="994e3-310">String</span></span>|<span data-ttu-id="994e3-311">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="994e3-312">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="994e3-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="994e3-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="994e3-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="994e3-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="994e3-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="994e3-315">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="994e3-316">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="994e3-316">Read Only.</span></span> <span data-ttu-id="994e3-317">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="994e3-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="994e3-318">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-318">retireAfterDateTime</span></span>|<span data-ttu-id="994e3-319">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-319">DateTimeOffset</span></span>|<span data-ttu-id="994e3-320">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="994e3-320">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="994e3-321">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="994e3-321">usersLoggedOn</span></span>|<span data-ttu-id="994e3-322">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="994e3-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="994e3-323">Indica o último usuário conectado de um dispositivo</span><span class="sxs-lookup"><span data-stu-id="994e3-323">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="994e3-324">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="994e3-324">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="994e3-325">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-325">DateTimeOffset</span></span>|<span data-ttu-id="994e3-326">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="994e3-326">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="994e3-327">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="994e3-327">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="994e3-328">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="994e3-328">Read Only.</span></span>|
|<span data-ttu-id="994e3-329">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="994e3-329">autopilotEnrolled</span></span>|<span data-ttu-id="994e3-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="994e3-330">Boolean</span></span>|<span data-ttu-id="994e3-331">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="994e3-331">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="994e3-332">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="994e3-332">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="994e3-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="994e3-333">Boolean</span></span>|<span data-ttu-id="994e3-334">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="994e3-334">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="994e3-335">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="994e3-335">managementCertificateExpirationDate</span></span>|<span data-ttu-id="994e3-336">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e3-336">DateTimeOffset</span></span>|<span data-ttu-id="994e3-337">Relatórios da data de expiração do certificado de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="994e3-337">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="994e3-338">iccid</span><span class="sxs-lookup"><span data-stu-id="994e3-338">iccid</span></span>|<span data-ttu-id="994e3-339">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-339">String</span></span>|<span data-ttu-id="994e3-340">Identificador de cartão de circuito integrado, é O número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="994e3-340">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="994e3-341">udid</span><span class="sxs-lookup"><span data-stu-id="994e3-341">udid</span></span>|<span data-ttu-id="994e3-342">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-342">String</span></span>|<span data-ttu-id="994e3-343">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="994e3-343">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="994e3-344">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="994e3-344">roleScopeTagIds</span></span>|<span data-ttu-id="994e3-345">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="994e3-345">String collection</span></span>|<span data-ttu-id="994e3-346">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="994e3-346">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="994e3-347">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="994e3-347">windowsActiveMalwareCount</span></span>|<span data-ttu-id="994e3-348">Int32</span><span class="sxs-lookup"><span data-stu-id="994e3-348">Int32</span></span>|<span data-ttu-id="994e3-349">Contagem de malwares ativos para este dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="994e3-349">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="994e3-350">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="994e3-350">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="994e3-351">Int32</span><span class="sxs-lookup"><span data-stu-id="994e3-351">Int32</span></span>|<span data-ttu-id="994e3-352">Contagem de malware corrigido para este dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="994e3-352">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="994e3-353">notes</span><span class="sxs-lookup"><span data-stu-id="994e3-353">notes</span></span>|<span data-ttu-id="994e3-354">String</span><span class="sxs-lookup"><span data-stu-id="994e3-354">String</span></span>|<span data-ttu-id="994e3-355">Observações sobre o dispositivo criado pelo administrador de ti</span><span class="sxs-lookup"><span data-stu-id="994e3-355">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="994e3-356">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="994e3-356">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="994e3-357">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="994e3-357">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="994e3-358">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="994e3-358">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="994e3-359">Resposta</span><span class="sxs-lookup"><span data-stu-id="994e3-359">Response</span></span>
<span data-ttu-id="994e3-360">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="994e3-360">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="994e3-361">Exemplo</span><span class="sxs-lookup"><span data-stu-id="994e3-361">Example</span></span>

### <a name="request"></a><span data-ttu-id="994e3-362">Solicitação</span><span class="sxs-lookup"><span data-stu-id="994e3-362">Request</span></span>
<span data-ttu-id="994e3-363">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="994e3-363">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7286

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
  }
}
```

### <a name="response"></a><span data-ttu-id="994e3-364">Resposta</span><span class="sxs-lookup"><span data-stu-id="994e3-364">Response</span></span>
<span data-ttu-id="994e3-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="994e3-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7335

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
  }
}
```




