---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fdc1c7c142e0c00a5eb8b9129018d1ee4e434e6f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797358"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="fd38c-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="fd38c-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="fd38c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd38c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd38c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd38c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd38c-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="fd38c-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd38c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd38c-107">Prerequisites</span></span>
<span data-ttu-id="fd38c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd38c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd38c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd38c-110">Permission type</span></span>|<span data-ttu-id="fd38c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd38c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd38c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd38c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd38c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd38c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fd38c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd38c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd38c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd38c-115">Not supported.</span></span>|
|<span data-ttu-id="fd38c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd38c-116">Application</span></span>|<span data-ttu-id="fd38c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd38c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd38c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd38c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="fd38c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd38c-119">Request headers</span></span>
|<span data-ttu-id="fd38c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd38c-120">Header</span></span>|<span data-ttu-id="fd38c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd38c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd38c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd38c-122">Authorization</span></span>|<span data-ttu-id="fd38c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd38c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd38c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd38c-124">Accept</span></span>|<span data-ttu-id="fd38c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd38c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd38c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd38c-126">Request body</span></span>
<span data-ttu-id="fd38c-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="fd38c-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="fd38c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="fd38c-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="fd38c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd38c-129">Property</span></span>|<span data-ttu-id="fd38c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd38c-130">Type</span></span>|<span data-ttu-id="fd38c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd38c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd38c-132">id</span><span class="sxs-lookup"><span data-stu-id="fd38c-132">id</span></span>|<span data-ttu-id="fd38c-133">String</span><span class="sxs-lookup"><span data-stu-id="fd38c-133">String</span></span>|<span data-ttu-id="fd38c-134">Identificador exclusivo do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-135">userId</span><span class="sxs-lookup"><span data-stu-id="fd38c-135">userId</span></span>|<span data-ttu-id="fd38c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-136">String</span></span>|<span data-ttu-id="fd38c-137">Identificador exclusivo do usuário associado ao dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="fd38c-138">deviceName</span></span>|<span data-ttu-id="fd38c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-139">String</span></span>|<span data-ttu-id="fd38c-140">Nome do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="fd38c-141">hardwareInformation</span></span>|[<span data-ttu-id="fd38c-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="fd38c-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="fd38c-143">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-143">The hardward details for the device.</span></span>  <span data-ttu-id="fd38c-144">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="fd38c-145">ownerType</span></span>|[<span data-ttu-id="fd38c-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="fd38c-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="fd38c-147">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-147">Ownership of the device.</span></span> <span data-ttu-id="fd38c-148">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-149">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="fd38c-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="fd38c-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="fd38c-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="fd38c-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="fd38c-152">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-152">Ownership of the device.</span></span> <span data-ttu-id="fd38c-153">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-154">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="fd38c-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="fd38c-155">deviceActionResults</span></span>|<span data-ttu-id="fd38c-156">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="fd38c-157">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="fd38c-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="fd38c-158">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-159">ManagementState</span><span class="sxs-lookup"><span data-stu-id="fd38c-159">managementState</span></span>|[<span data-ttu-id="fd38c-160">ManagementState</span><span class="sxs-lookup"><span data-stu-id="fd38c-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="fd38c-161">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-161">Management state of the device.</span></span> <span data-ttu-id="fd38c-162">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-163">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="fd38c-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="fd38c-164">enrolledDateTime</span></span>|<span data-ttu-id="fd38c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-165">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-166">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-166">Enrollment time of the device.</span></span> <span data-ttu-id="fd38c-167">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fd38c-168">lastSyncDateTime</span></span>|<span data-ttu-id="fd38c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-169">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-170">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="fd38c-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="fd38c-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="fd38c-172">chassisType</span></span>|[<span data-ttu-id="fd38c-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="fd38c-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="fd38c-174">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-174">Chassis type of the device.</span></span> <span data-ttu-id="fd38c-175">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-176">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="fd38c-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd38c-177">operatingSystem</span></span>|<span data-ttu-id="fd38c-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-178">String</span></span>|<span data-ttu-id="fd38c-179">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-179">Operating system of the device.</span></span> <span data-ttu-id="fd38c-180">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="fd38c-181">deviceType</span></span>|[<span data-ttu-id="fd38c-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="fd38c-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="fd38c-183">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-183">Platform of the device.</span></span> <span data-ttu-id="fd38c-184">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-185">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="fd38c-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="fd38c-186">complianceState</span></span>|[<span data-ttu-id="fd38c-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="fd38c-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="fd38c-188">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-188">Compliance state of the device.</span></span> <span data-ttu-id="fd38c-189">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-190">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="fd38c-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="fd38c-191">jailBroken</span></span>|<span data-ttu-id="fd38c-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-192">String</span></span>|<span data-ttu-id="fd38c-193">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="fd38c-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="fd38c-194">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="fd38c-195">managementAgent</span></span>|[<span data-ttu-id="fd38c-196">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="fd38c-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="fd38c-197">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-197">Management channel of the device.</span></span> <span data-ttu-id="fd38c-198">Intune, EAS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-199">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="fd38c-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="fd38c-200">osVersion</span></span>|<span data-ttu-id="fd38c-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-201">String</span></span>|<span data-ttu-id="fd38c-202">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-202">Operating system version of the device.</span></span> <span data-ttu-id="fd38c-203">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="fd38c-204">easActivated</span></span>|<span data-ttu-id="fd38c-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd38c-205">Boolean</span></span>|<span data-ttu-id="fd38c-206">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="fd38c-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="fd38c-207">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="fd38c-208">easDeviceId</span></span>|<span data-ttu-id="fd38c-209">String</span><span class="sxs-lookup"><span data-stu-id="fd38c-209">String</span></span>|<span data-ttu-id="fd38c-210">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="fd38c-211">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd38c-212">easActivationDateTime</span></span>|<span data-ttu-id="fd38c-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-213">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-214">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="fd38c-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="fd38c-216">aadRegistered</span></span>|<span data-ttu-id="fd38c-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd38c-217">Boolean</span></span>|<span data-ttu-id="fd38c-218">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fd38c-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="fd38c-219">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="fd38c-220">azureADRegistered</span></span>|<span data-ttu-id="fd38c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd38c-221">Boolean</span></span>|<span data-ttu-id="fd38c-222">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fd38c-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="fd38c-223">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="fd38c-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="fd38c-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="fd38c-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="fd38c-226">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-226">Enrollment type of the device.</span></span> <span data-ttu-id="fd38c-227">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-228">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="fd38c-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="fd38c-229">lostModeState</span></span>|[<span data-ttu-id="fd38c-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="fd38c-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="fd38c-231">Indica se o modo perdido está habilitado ou desabilitado herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-232">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="fd38c-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="fd38c-233">activationLockBypassCode</span></span>|<span data-ttu-id="fd38c-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-234">String</span></span>|<span data-ttu-id="fd38c-235">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="fd38c-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="fd38c-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fd38c-237">emailAddress</span></span>|<span data-ttu-id="fd38c-238">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-238">String</span></span>|<span data-ttu-id="fd38c-239">Email (s) para o usuário associado ao dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="fd38c-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="fd38c-241">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-241">String</span></span>|<span data-ttu-id="fd38c-242">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fd38c-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="fd38c-243">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd38c-243">Read only.</span></span> <span data-ttu-id="fd38c-244">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="fd38c-245">azureADDeviceId</span></span>|<span data-ttu-id="fd38c-246">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-246">String</span></span>|<span data-ttu-id="fd38c-247">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fd38c-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="fd38c-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd38c-248">Read only.</span></span> <span data-ttu-id="fd38c-249">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="fd38c-250">deviceRegistrationState</span></span>|[<span data-ttu-id="fd38c-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="fd38c-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="fd38c-252">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-252">Device registration state.</span></span> <span data-ttu-id="fd38c-253">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-254">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="fd38c-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="fd38c-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="fd38c-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-256">String</span></span>|<span data-ttu-id="fd38c-257">Nome de exibição de categoria de dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="fd38c-258">isSupervised</span></span>|<span data-ttu-id="fd38c-259">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd38c-259">Boolean</span></span>|<span data-ttu-id="fd38c-260">Status supervisionado do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fd38c-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="fd38c-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-262">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-263">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd38c-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="fd38c-264">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="fd38c-265">exchangeAccessState</span></span>|[<span data-ttu-id="fd38c-266">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="fd38c-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="fd38c-267">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd38c-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="fd38c-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-269">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="fd38c-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="fd38c-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="fd38c-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="fd38c-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="fd38c-272">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd38c-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="fd38c-273">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-274">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="fd38c-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="fd38c-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="fd38c-276">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-276">String</span></span>|<span data-ttu-id="fd38c-277">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="fd38c-278">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="fd38c-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="fd38c-280">String</span><span class="sxs-lookup"><span data-stu-id="fd38c-280">String</span></span>|<span data-ttu-id="fd38c-281">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="fd38c-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="fd38c-282">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="fd38c-283">isEncrypted</span></span>|<span data-ttu-id="fd38c-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd38c-284">Boolean</span></span>|<span data-ttu-id="fd38c-285">Status de criptografia do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd38c-286">userPrincipalName</span></span>|<span data-ttu-id="fd38c-287">String</span><span class="sxs-lookup"><span data-stu-id="fd38c-287">String</span></span>|<span data-ttu-id="fd38c-288">Nome principal de usuário do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-289">modelo</span><span class="sxs-lookup"><span data-stu-id="fd38c-289">model</span></span>|<span data-ttu-id="fd38c-290">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-290">String</span></span>|<span data-ttu-id="fd38c-291">Modelo do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-292">fabricante</span><span class="sxs-lookup"><span data-stu-id="fd38c-292">manufacturer</span></span>|<span data-ttu-id="fd38c-293">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-293">String</span></span>|<span data-ttu-id="fd38c-294">Fabricante do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-295">imei</span><span class="sxs-lookup"><span data-stu-id="fd38c-295">imei</span></span>|<span data-ttu-id="fd38c-296">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-296">String</span></span>|<span data-ttu-id="fd38c-297">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd38c-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="fd38c-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-299">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-300">O DateTime quando o período de cortesia de conformidade do dispositivo expira herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="fd38c-301">serialNumber</span></span>|<span data-ttu-id="fd38c-302">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-302">String</span></span>|<span data-ttu-id="fd38c-303">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="fd38c-304">phoneNumber</span></span>|<span data-ttu-id="fd38c-305">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-305">String</span></span>|<span data-ttu-id="fd38c-306">Número de telefone do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="fd38c-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="fd38c-308">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-308">String</span></span>|<span data-ttu-id="fd38c-309">Nível de patch de segurança do Android herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fd38c-310">userDisplayName</span></span>|<span data-ttu-id="fd38c-311">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-311">String</span></span>|<span data-ttu-id="fd38c-312">Nome de exibição do usuário herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="fd38c-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="fd38c-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="fd38c-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="fd38c-315">Recursos habilitados pelo cliente do ConfigrMgr herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="fd38c-316">wiFiMacAddress</span></span>|<span data-ttu-id="fd38c-317">String</span><span class="sxs-lookup"><span data-stu-id="fd38c-317">String</span></span>|<span data-ttu-id="fd38c-318">MAC Wi-Fi herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="fd38c-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="fd38c-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="fd38c-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="fd38c-321">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-321">The device health attestation state.</span></span> <span data-ttu-id="fd38c-322">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="fd38c-323">subscriberCarrier</span></span>|<span data-ttu-id="fd38c-324">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-324">String</span></span>|<span data-ttu-id="fd38c-325">Operadora de assinante herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-326">meid</span><span class="sxs-lookup"><span data-stu-id="fd38c-326">meid</span></span>|<span data-ttu-id="fd38c-327">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-327">String</span></span>|<span data-ttu-id="fd38c-328">MEID herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="fd38c-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="fd38c-330">Int64</span><span class="sxs-lookup"><span data-stu-id="fd38c-330">Int64</span></span>|<span data-ttu-id="fd38c-331">Armazenamento total em bytes herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="fd38c-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="fd38c-333">Int64</span><span class="sxs-lookup"><span data-stu-id="fd38c-333">Int64</span></span>|<span data-ttu-id="fd38c-334">Armazenamento gratuito em bytes herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="fd38c-335">managedDeviceName</span></span>|<span data-ttu-id="fd38c-336">String</span><span class="sxs-lookup"><span data-stu-id="fd38c-336">String</span></span>|<span data-ttu-id="fd38c-337">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="fd38c-338">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="fd38c-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="fd38c-339">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="fd38c-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="fd38c-341">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="fd38c-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="fd38c-342">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="fd38c-343">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd38c-343">Read Only.</span></span> <span data-ttu-id="fd38c-344">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="fd38c-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="fd38c-345">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="fd38c-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="fd38c-346">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="fd38c-346">usersLoggedOn</span></span>|<span data-ttu-id="fd38c-347">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="fd38c-348">Indica os últimos usuários conectados de um dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-349">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd38c-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="fd38c-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-350">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-351">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="fd38c-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="fd38c-352">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="fd38c-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="fd38c-353">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd38c-353">Read Only.</span></span> <span data-ttu-id="fd38c-354">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-355">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="fd38c-355">autopilotEnrolled</span></span>|<span data-ttu-id="fd38c-356">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd38c-356">Boolean</span></span>|<span data-ttu-id="fd38c-357">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="fd38c-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="fd38c-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-359">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="fd38c-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="fd38c-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd38c-360">Boolean</span></span>|<span data-ttu-id="fd38c-361">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd38c-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="fd38c-362">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-363">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="fd38c-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="fd38c-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd38c-364">DateTimeOffset</span></span>|<span data-ttu-id="fd38c-365">Relata a data de expiração do certificado de gerenciamento de dispositivos herdada de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-366">ICCID</span><span class="sxs-lookup"><span data-stu-id="fd38c-366">iccid</span></span>|<span data-ttu-id="fd38c-367">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-367">String</span></span>|<span data-ttu-id="fd38c-368">Identificador de cartão de circuito integrado, é O número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="fd38c-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="fd38c-369">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-370">UDID</span><span class="sxs-lookup"><span data-stu-id="fd38c-370">udid</span></span>|<span data-ttu-id="fd38c-371">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-371">String</span></span>|<span data-ttu-id="fd38c-372">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="fd38c-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="fd38c-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-374">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd38c-374">roleScopeTagIds</span></span>|<span data-ttu-id="fd38c-375">Coleção String</span><span class="sxs-lookup"><span data-stu-id="fd38c-375">String collection</span></span>|<span data-ttu-id="fd38c-376">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fd38c-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="fd38c-377">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-378">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="fd38c-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="fd38c-379">Int32</span><span class="sxs-lookup"><span data-stu-id="fd38c-379">Int32</span></span>|<span data-ttu-id="fd38c-380">Contagem de malware ativo para este dispositivo do Windows herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-381">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="fd38c-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="fd38c-382">Int32</span><span class="sxs-lookup"><span data-stu-id="fd38c-382">Int32</span></span>|<span data-ttu-id="fd38c-383">Contagem de malware corrigido para este dispositivo Windows herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-384">notes</span><span class="sxs-lookup"><span data-stu-id="fd38c-384">notes</span></span>|<span data-ttu-id="fd38c-385">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd38c-385">String</span></span>|<span data-ttu-id="fd38c-386">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="fd38c-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="fd38c-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="fd38c-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="fd38c-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="fd38c-389">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fd38c-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fd38c-390">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd38c-390">Response</span></span>
<span data-ttu-id="fd38c-391">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd38c-391">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd38c-392">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd38c-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd38c-393">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd38c-393">Request</span></span>
<span data-ttu-id="fd38c-394">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd38c-394">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7231

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

### <a name="response"></a><span data-ttu-id="fd38c-395">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd38c-395">Response</span></span>
<span data-ttu-id="fd38c-p141">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd38c-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7280

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





