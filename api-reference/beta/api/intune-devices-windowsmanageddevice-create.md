---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af818cb68e924a0225dcce869200c9ed04d00527
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909271"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="1e511-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="1e511-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="1e511-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e511-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e511-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e511-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e511-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="1e511-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e511-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e511-107">Prerequisites</span></span>
<span data-ttu-id="1e511-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e511-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e511-110">Permission type</span></span>|<span data-ttu-id="1e511-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e511-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e511-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e511-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e511-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e511-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1e511-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e511-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e511-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e511-115">Not supported.</span></span>|
|<span data-ttu-id="1e511-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e511-116">Application</span></span>|<span data-ttu-id="1e511-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e511-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e511-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e511-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="1e511-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e511-119">Request headers</span></span>
|<span data-ttu-id="1e511-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e511-120">Header</span></span>|<span data-ttu-id="1e511-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e511-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e511-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e511-122">Authorization</span></span>|<span data-ttu-id="1e511-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e511-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e511-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e511-124">Accept</span></span>|<span data-ttu-id="1e511-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e511-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e511-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e511-126">Request body</span></span>
<span data-ttu-id="1e511-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="1e511-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="1e511-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="1e511-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="1e511-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e511-129">Property</span></span>|<span data-ttu-id="1e511-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e511-130">Type</span></span>|<span data-ttu-id="1e511-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e511-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e511-132">id</span><span class="sxs-lookup"><span data-stu-id="1e511-132">id</span></span>|<span data-ttu-id="1e511-133">String</span><span class="sxs-lookup"><span data-stu-id="1e511-133">String</span></span>|<span data-ttu-id="1e511-134">Identificador exclusivo do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-135">userId</span><span class="sxs-lookup"><span data-stu-id="1e511-135">userId</span></span>|<span data-ttu-id="1e511-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-136">String</span></span>|<span data-ttu-id="1e511-137">Identificador exclusivo do usuário associado ao dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="1e511-138">deviceName</span></span>|<span data-ttu-id="1e511-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-139">String</span></span>|<span data-ttu-id="1e511-140">Nome do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="1e511-141">hardwareInformation</span></span>|[<span data-ttu-id="1e511-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="1e511-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="1e511-143">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-143">The hardward details for the device.</span></span>  <span data-ttu-id="1e511-144">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="1e511-145">ownerType</span></span>|[<span data-ttu-id="1e511-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="1e511-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="1e511-147">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-147">Ownership of the device.</span></span> <span data-ttu-id="1e511-148">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-149">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="1e511-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="1e511-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1e511-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="1e511-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1e511-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="1e511-152">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-152">Ownership of the device.</span></span> <span data-ttu-id="1e511-153">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-154">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="1e511-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="1e511-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="1e511-155">deviceActionResults</span></span>|<span data-ttu-id="1e511-156">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="1e511-157">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="1e511-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="1e511-158">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-159">ManagementState</span><span class="sxs-lookup"><span data-stu-id="1e511-159">managementState</span></span>|[<span data-ttu-id="1e511-160">ManagementState</span><span class="sxs-lookup"><span data-stu-id="1e511-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="1e511-161">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-161">Management state of the device.</span></span> <span data-ttu-id="1e511-162">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-163">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="1e511-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="1e511-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-164">enrolledDateTime</span></span>|<span data-ttu-id="1e511-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-165">DateTimeOffset</span></span>|<span data-ttu-id="1e511-166">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-166">Enrollment time of the device.</span></span> <span data-ttu-id="1e511-167">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-168">lastSyncDateTime</span></span>|<span data-ttu-id="1e511-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-169">DateTimeOffset</span></span>|<span data-ttu-id="1e511-170">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="1e511-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="1e511-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="1e511-172">chassisType</span></span>|[<span data-ttu-id="1e511-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="1e511-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="1e511-174">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-174">Chassis type of the device.</span></span> <span data-ttu-id="1e511-175">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-176">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="1e511-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="1e511-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e511-177">operatingSystem</span></span>|<span data-ttu-id="1e511-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-178">String</span></span>|<span data-ttu-id="1e511-179">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-179">Operating system of the device.</span></span> <span data-ttu-id="1e511-180">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="1e511-181">deviceType</span></span>|[<span data-ttu-id="1e511-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="1e511-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="1e511-183">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-183">Platform of the device.</span></span> <span data-ttu-id="1e511-184">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-185">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1e511-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="1e511-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="1e511-186">complianceState</span></span>|[<span data-ttu-id="1e511-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="1e511-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="1e511-188">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-188">Compliance state of the device.</span></span> <span data-ttu-id="1e511-189">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-190">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="1e511-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="1e511-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="1e511-191">jailBroken</span></span>|<span data-ttu-id="1e511-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-192">String</span></span>|<span data-ttu-id="1e511-193">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="1e511-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="1e511-194">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="1e511-195">managementAgent</span></span>|[<span data-ttu-id="1e511-196">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="1e511-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="1e511-197">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-197">Management channel of the device.</span></span> <span data-ttu-id="1e511-198">Intune, EAS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-199">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="1e511-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="1e511-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="1e511-200">osVersion</span></span>|<span data-ttu-id="1e511-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-201">String</span></span>|<span data-ttu-id="1e511-202">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-202">Operating system version of the device.</span></span> <span data-ttu-id="1e511-203">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="1e511-204">easActivated</span></span>|<span data-ttu-id="1e511-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e511-205">Boolean</span></span>|<span data-ttu-id="1e511-206">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="1e511-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="1e511-207">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="1e511-208">easDeviceId</span></span>|<span data-ttu-id="1e511-209">String</span><span class="sxs-lookup"><span data-stu-id="1e511-209">String</span></span>|<span data-ttu-id="1e511-210">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="1e511-211">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-212">easActivationDateTime</span></span>|<span data-ttu-id="1e511-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-213">DateTimeOffset</span></span>|<span data-ttu-id="1e511-214">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="1e511-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="1e511-216">aadRegistered</span></span>|<span data-ttu-id="1e511-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e511-217">Boolean</span></span>|<span data-ttu-id="1e511-218">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e511-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="1e511-219">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="1e511-220">azureADRegistered</span></span>|<span data-ttu-id="1e511-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e511-221">Boolean</span></span>|<span data-ttu-id="1e511-222">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e511-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="1e511-223">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1e511-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="1e511-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1e511-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="1e511-226">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-226">Enrollment type of the device.</span></span> <span data-ttu-id="1e511-227">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-228">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="1e511-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="1e511-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="1e511-229">lostModeState</span></span>|[<span data-ttu-id="1e511-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="1e511-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="1e511-231">Indica se o modo perdido está habilitado ou desabilitado herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-232">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="1e511-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="1e511-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="1e511-233">activationLockBypassCode</span></span>|<span data-ttu-id="1e511-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-234">String</span></span>|<span data-ttu-id="1e511-235">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="1e511-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="1e511-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1e511-237">emailAddress</span></span>|<span data-ttu-id="1e511-238">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-238">String</span></span>|<span data-ttu-id="1e511-239">Email (s) para o usuário associado ao dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="1e511-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="1e511-241">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-241">String</span></span>|<span data-ttu-id="1e511-242">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e511-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="1e511-243">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e511-243">Read only.</span></span> <span data-ttu-id="1e511-244">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="1e511-245">azureADDeviceId</span></span>|<span data-ttu-id="1e511-246">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-246">String</span></span>|<span data-ttu-id="1e511-247">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1e511-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="1e511-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e511-248">Read only.</span></span> <span data-ttu-id="1e511-249">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1e511-250">deviceRegistrationState</span></span>|[<span data-ttu-id="1e511-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1e511-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="1e511-252">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-252">Device registration state.</span></span> <span data-ttu-id="1e511-253">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-254">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1e511-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="1e511-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e511-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="1e511-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-256">String</span></span>|<span data-ttu-id="1e511-257">Nome de exibição de categoria de dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1e511-258">isSupervised</span></span>|<span data-ttu-id="1e511-259">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e511-259">Boolean</span></span>|<span data-ttu-id="1e511-260">Status supervisionado do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1e511-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-262">DateTimeOffset</span></span>|<span data-ttu-id="1e511-263">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e511-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="1e511-264">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1e511-265">exchangeAccessState</span></span>|[<span data-ttu-id="1e511-266">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1e511-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="1e511-267">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e511-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="1e511-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-269">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="1e511-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="1e511-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1e511-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="1e511-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1e511-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="1e511-272">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e511-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="1e511-273">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-274">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="1e511-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="1e511-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="1e511-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="1e511-276">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-276">String</span></span>|<span data-ttu-id="1e511-277">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="1e511-278">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1e511-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="1e511-280">String</span><span class="sxs-lookup"><span data-stu-id="1e511-280">String</span></span>|<span data-ttu-id="1e511-281">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="1e511-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="1e511-282">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1e511-283">isEncrypted</span></span>|<span data-ttu-id="1e511-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e511-284">Boolean</span></span>|<span data-ttu-id="1e511-285">Status de criptografia do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e511-286">userPrincipalName</span></span>|<span data-ttu-id="1e511-287">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-287">String</span></span>|<span data-ttu-id="1e511-288">Nome principal de usuário do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-289">modelo</span><span class="sxs-lookup"><span data-stu-id="1e511-289">model</span></span>|<span data-ttu-id="1e511-290">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-290">String</span></span>|<span data-ttu-id="1e511-291">Modelo do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-292">fabricante</span><span class="sxs-lookup"><span data-stu-id="1e511-292">manufacturer</span></span>|<span data-ttu-id="1e511-293">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-293">String</span></span>|<span data-ttu-id="1e511-294">Fabricante do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-295">imei</span><span class="sxs-lookup"><span data-stu-id="1e511-295">imei</span></span>|<span data-ttu-id="1e511-296">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-296">String</span></span>|<span data-ttu-id="1e511-297">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1e511-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-299">DateTimeOffset</span></span>|<span data-ttu-id="1e511-300">O DateTime quando o período de cortesia de conformidade do dispositivo expira herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1e511-301">serialNumber</span></span>|<span data-ttu-id="1e511-302">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-302">String</span></span>|<span data-ttu-id="1e511-303">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1e511-304">phoneNumber</span></span>|<span data-ttu-id="1e511-305">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-305">String</span></span>|<span data-ttu-id="1e511-306">Número de telefone do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1e511-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="1e511-308">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-308">String</span></span>|<span data-ttu-id="1e511-309">Nível de patch de segurança do Android herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e511-310">userDisplayName</span></span>|<span data-ttu-id="1e511-311">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-311">String</span></span>|<span data-ttu-id="1e511-312">Nome de exibição do usuário herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1e511-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="1e511-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1e511-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="1e511-315">Recursos habilitados pelo cliente do ConfigrMgr herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="1e511-316">wiFiMacAddress</span></span>|<span data-ttu-id="1e511-317">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-317">String</span></span>|<span data-ttu-id="1e511-318">MAC Wi-Fi herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1e511-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="1e511-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1e511-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="1e511-321">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-321">The device health attestation state.</span></span> <span data-ttu-id="1e511-322">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="1e511-323">subscriberCarrier</span></span>|<span data-ttu-id="1e511-324">String</span><span class="sxs-lookup"><span data-stu-id="1e511-324">String</span></span>|<span data-ttu-id="1e511-325">Operadora de assinante herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-326">meid</span><span class="sxs-lookup"><span data-stu-id="1e511-326">meid</span></span>|<span data-ttu-id="1e511-327">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-327">String</span></span>|<span data-ttu-id="1e511-328">MEID herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1e511-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="1e511-330">Int64</span><span class="sxs-lookup"><span data-stu-id="1e511-330">Int64</span></span>|<span data-ttu-id="1e511-331">Armazenamento total em bytes herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1e511-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="1e511-333">Int64</span><span class="sxs-lookup"><span data-stu-id="1e511-333">Int64</span></span>|<span data-ttu-id="1e511-334">Armazenamento gratuito em bytes herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="1e511-335">managedDeviceName</span></span>|<span data-ttu-id="1e511-336">String</span><span class="sxs-lookup"><span data-stu-id="1e511-336">String</span></span>|<span data-ttu-id="1e511-337">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="1e511-338">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="1e511-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="1e511-339">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="1e511-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="1e511-341">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="1e511-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="1e511-342">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="1e511-343">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e511-343">Read Only.</span></span> <span data-ttu-id="1e511-344">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1e511-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="1e511-345">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="1e511-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="1e511-346">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-346">retireAfterDateTime</span></span>|<span data-ttu-id="1e511-347">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-347">DateTimeOffset</span></span>|<span data-ttu-id="1e511-348">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="1e511-348">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="1e511-349">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-350">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="1e511-350">usersLoggedOn</span></span>|<span data-ttu-id="1e511-351">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-351">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="1e511-352">Indica os últimos usuários conectados de um dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-352">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-353">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e511-353">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="1e511-354">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-354">DateTimeOffset</span></span>|<span data-ttu-id="1e511-355">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="1e511-355">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="1e511-356">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="1e511-356">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="1e511-357">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e511-357">Read Only.</span></span> <span data-ttu-id="1e511-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-359">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="1e511-359">autopilotEnrolled</span></span>|<span data-ttu-id="1e511-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e511-360">Boolean</span></span>|<span data-ttu-id="1e511-361">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="1e511-361">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="1e511-362">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-363">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="1e511-363">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="1e511-364">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e511-364">Boolean</span></span>|<span data-ttu-id="1e511-365">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="1e511-365">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="1e511-366">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-366">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-367">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="1e511-367">managementCertificateExpirationDate</span></span>|<span data-ttu-id="1e511-368">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e511-368">DateTimeOffset</span></span>|<span data-ttu-id="1e511-369">Relata a data de expiração do certificado de gerenciamento de dispositivos herdada de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-369">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-370">iccid</span><span class="sxs-lookup"><span data-stu-id="1e511-370">iccid</span></span>|<span data-ttu-id="1e511-371">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-371">String</span></span>|<span data-ttu-id="1e511-372">Identificador de cartão de circuito integrado, é O número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="1e511-372">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="1e511-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-374">udid</span><span class="sxs-lookup"><span data-stu-id="1e511-374">udid</span></span>|<span data-ttu-id="1e511-375">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-375">String</span></span>|<span data-ttu-id="1e511-376">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="1e511-376">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="1e511-377">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-378">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e511-378">roleScopeTagIds</span></span>|<span data-ttu-id="1e511-379">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-379">String collection</span></span>|<span data-ttu-id="1e511-380">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e511-380">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="1e511-381">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-381">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-382">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="1e511-382">windowsActiveMalwareCount</span></span>|<span data-ttu-id="1e511-383">Int32</span><span class="sxs-lookup"><span data-stu-id="1e511-383">Int32</span></span>|<span data-ttu-id="1e511-384">Contagem de malware ativo para este dispositivo do Windows herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-384">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-385">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="1e511-385">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="1e511-386">Int32</span><span class="sxs-lookup"><span data-stu-id="1e511-386">Int32</span></span>|<span data-ttu-id="1e511-387">Contagem de malware corrigido para este dispositivo Windows herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-387">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-388">notes</span><span class="sxs-lookup"><span data-stu-id="1e511-388">notes</span></span>|<span data-ttu-id="1e511-389">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e511-389">String</span></span>|<span data-ttu-id="1e511-390">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-390">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="1e511-391">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="1e511-391">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="1e511-392">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="1e511-392">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="1e511-393">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1e511-393">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1e511-394">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e511-394">Response</span></span>
<span data-ttu-id="1e511-395">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e511-395">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e511-396">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e511-396">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e511-397">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e511-397">Request</span></span>
<span data-ttu-id="1e511-398">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e511-398">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7293

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

### <a name="response"></a><span data-ttu-id="1e511-399">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e511-399">Response</span></span>
<span data-ttu-id="1e511-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e511-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7342

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




