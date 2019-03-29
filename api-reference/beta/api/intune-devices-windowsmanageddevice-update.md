---
title: Atualizar windowsManagedDevice
description: Atualiza as propriedades de um objeto windowsManagedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1fd03350e06b467713ee1338e62f58cab45b44a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962551"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="80e00-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="80e00-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="80e00-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80e00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80e00-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80e00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80e00-106">Atualiza as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="80e00-106">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80e00-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80e00-107">Prerequisites</span></span>
<span data-ttu-id="80e00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80e00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80e00-110">Permission type</span></span>|<span data-ttu-id="80e00-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80e00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80e00-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80e00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80e00-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e00-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="80e00-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80e00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80e00-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80e00-115">Not supported.</span></span>|
|<span data-ttu-id="80e00-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80e00-116">Application</span></span>|<span data-ttu-id="80e00-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80e00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80e00-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80e00-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="80e00-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80e00-119">Request headers</span></span>
|<span data-ttu-id="80e00-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80e00-120">Header</span></span>|<span data-ttu-id="80e00-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80e00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80e00-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80e00-122">Authorization</span></span>|<span data-ttu-id="80e00-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80e00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80e00-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80e00-124">Accept</span></span>|<span data-ttu-id="80e00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80e00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80e00-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80e00-126">Request body</span></span>
<span data-ttu-id="80e00-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="80e00-127">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="80e00-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-128">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="80e00-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80e00-129">Property</span></span>|<span data-ttu-id="80e00-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80e00-130">Type</span></span>|<span data-ttu-id="80e00-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80e00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e00-132">id</span><span class="sxs-lookup"><span data-stu-id="80e00-132">id</span></span>|<span data-ttu-id="80e00-133">String</span><span class="sxs-lookup"><span data-stu-id="80e00-133">String</span></span>|<span data-ttu-id="80e00-134">Identificador exclusivo do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-135">userId</span><span class="sxs-lookup"><span data-stu-id="80e00-135">userId</span></span>|<span data-ttu-id="80e00-136">String</span><span class="sxs-lookup"><span data-stu-id="80e00-136">String</span></span>|<span data-ttu-id="80e00-137">Identificador exclusivo do usuário associado ao dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="80e00-138">deviceName</span></span>|<span data-ttu-id="80e00-139">String</span><span class="sxs-lookup"><span data-stu-id="80e00-139">String</span></span>|<span data-ttu-id="80e00-140">Nome do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="80e00-141">hardwareInformation</span></span>|[<span data-ttu-id="80e00-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="80e00-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="80e00-143">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-143">The hardward details for the device.</span></span>  <span data-ttu-id="80e00-144">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="80e00-145">ownerType</span></span>|[<span data-ttu-id="80e00-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="80e00-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="80e00-147">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-147">Ownership of the device.</span></span> <span data-ttu-id="80e00-148">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-149">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="80e00-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="80e00-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="80e00-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="80e00-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="80e00-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="80e00-152">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-152">Ownership of the device.</span></span> <span data-ttu-id="80e00-153">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-154">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="80e00-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="80e00-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="80e00-155">deviceActionResults</span></span>|<span data-ttu-id="80e00-156">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="80e00-157">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="80e00-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="80e00-158">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-159">ManagementState</span><span class="sxs-lookup"><span data-stu-id="80e00-159">managementState</span></span>|[<span data-ttu-id="80e00-160">ManagementState</span><span class="sxs-lookup"><span data-stu-id="80e00-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="80e00-161">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-161">Management state of the device.</span></span> <span data-ttu-id="80e00-162">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-163">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="80e00-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="80e00-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="80e00-164">enrolledDateTime</span></span>|<span data-ttu-id="80e00-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-165">DateTimeOffset</span></span>|<span data-ttu-id="80e00-166">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-166">Enrollment time of the device.</span></span> <span data-ttu-id="80e00-167">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80e00-168">lastSyncDateTime</span></span>|<span data-ttu-id="80e00-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-169">DateTimeOffset</span></span>|<span data-ttu-id="80e00-170">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="80e00-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="80e00-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="80e00-172">chassisType</span></span>|[<span data-ttu-id="80e00-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="80e00-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="80e00-174">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-174">Chassis type of the device.</span></span> <span data-ttu-id="80e00-175">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-176">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="80e00-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="80e00-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="80e00-177">operatingSystem</span></span>|<span data-ttu-id="80e00-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80e00-178">String</span></span>|<span data-ttu-id="80e00-179">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-179">Operating system of the device.</span></span> <span data-ttu-id="80e00-180">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="80e00-181">deviceType</span></span>|[<span data-ttu-id="80e00-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="80e00-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="80e00-183">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-183">Platform of the device.</span></span> <span data-ttu-id="80e00-184">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-185">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="80e00-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="80e00-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="80e00-186">complianceState</span></span>|[<span data-ttu-id="80e00-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="80e00-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="80e00-188">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-188">Compliance state of the device.</span></span> <span data-ttu-id="80e00-189">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-190">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="80e00-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="80e00-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="80e00-191">jailBroken</span></span>|<span data-ttu-id="80e00-192">String</span><span class="sxs-lookup"><span data-stu-id="80e00-192">String</span></span>|<span data-ttu-id="80e00-193">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="80e00-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="80e00-194">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="80e00-195">managementAgent</span></span>|[<span data-ttu-id="80e00-196">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="80e00-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="80e00-197">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-197">Management channel of the device.</span></span> <span data-ttu-id="80e00-198">Intune, EAS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-199">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="80e00-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="80e00-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="80e00-200">osVersion</span></span>|<span data-ttu-id="80e00-201">String</span><span class="sxs-lookup"><span data-stu-id="80e00-201">String</span></span>|<span data-ttu-id="80e00-202">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-202">Operating system version of the device.</span></span> <span data-ttu-id="80e00-203">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="80e00-204">easActivated</span></span>|<span data-ttu-id="80e00-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-205">Boolean</span></span>|<span data-ttu-id="80e00-206">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="80e00-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="80e00-207">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="80e00-208">easDeviceId</span></span>|<span data-ttu-id="80e00-209">String</span><span class="sxs-lookup"><span data-stu-id="80e00-209">String</span></span>|<span data-ttu-id="80e00-210">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="80e00-211">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="80e00-212">easActivationDateTime</span></span>|<span data-ttu-id="80e00-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-213">DateTimeOffset</span></span>|<span data-ttu-id="80e00-214">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="80e00-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="80e00-216">aadRegistered</span></span>|<span data-ttu-id="80e00-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-217">Boolean</span></span>|<span data-ttu-id="80e00-218">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="80e00-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="80e00-219">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="80e00-220">azureADRegistered</span></span>|<span data-ttu-id="80e00-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-221">Boolean</span></span>|<span data-ttu-id="80e00-222">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="80e00-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="80e00-223">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="80e00-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="80e00-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="80e00-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="80e00-226">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-226">Enrollment type of the device.</span></span> <span data-ttu-id="80e00-227">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-228">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="80e00-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="80e00-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="80e00-229">lostModeState</span></span>|[<span data-ttu-id="80e00-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="80e00-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="80e00-231">Indica se o modo perdido está habilitado ou desabilitado herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-232">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="80e00-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="80e00-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="80e00-233">activationLockBypassCode</span></span>|<span data-ttu-id="80e00-234">String</span><span class="sxs-lookup"><span data-stu-id="80e00-234">String</span></span>|<span data-ttu-id="80e00-235">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="80e00-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="80e00-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="80e00-237">emailAddress</span></span>|<span data-ttu-id="80e00-238">String</span><span class="sxs-lookup"><span data-stu-id="80e00-238">String</span></span>|<span data-ttu-id="80e00-239">Email (s) para o usuário associado ao dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="80e00-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="80e00-241">String</span><span class="sxs-lookup"><span data-stu-id="80e00-241">String</span></span>|<span data-ttu-id="80e00-242">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="80e00-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="80e00-243">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e00-243">Read only.</span></span> <span data-ttu-id="80e00-244">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="80e00-245">azureADDeviceId</span></span>|<span data-ttu-id="80e00-246">String</span><span class="sxs-lookup"><span data-stu-id="80e00-246">String</span></span>|<span data-ttu-id="80e00-247">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="80e00-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="80e00-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e00-248">Read only.</span></span> <span data-ttu-id="80e00-249">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="80e00-250">deviceRegistrationState</span></span>|[<span data-ttu-id="80e00-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="80e00-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="80e00-252">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-252">Device registration state.</span></span> <span data-ttu-id="80e00-253">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-254">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="80e00-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="80e00-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="80e00-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="80e00-256">String</span><span class="sxs-lookup"><span data-stu-id="80e00-256">String</span></span>|<span data-ttu-id="80e00-257">Nome de exibição de categoria de dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="80e00-258">isSupervised</span></span>|<span data-ttu-id="80e00-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-259">Boolean</span></span>|<span data-ttu-id="80e00-260">Status supervisionado do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80e00-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="80e00-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-262">DateTimeOffset</span></span>|<span data-ttu-id="80e00-263">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="80e00-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="80e00-264">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="80e00-265">exchangeAccessState</span></span>|[<span data-ttu-id="80e00-266">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="80e00-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="80e00-267">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="80e00-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="80e00-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-269">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="80e00-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="80e00-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="80e00-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="80e00-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="80e00-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="80e00-272">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="80e00-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="80e00-273">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-274">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="80e00-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="80e00-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="80e00-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="80e00-276">String</span><span class="sxs-lookup"><span data-stu-id="80e00-276">String</span></span>|<span data-ttu-id="80e00-277">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="80e00-278">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="80e00-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="80e00-280">String</span><span class="sxs-lookup"><span data-stu-id="80e00-280">String</span></span>|<span data-ttu-id="80e00-281">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="80e00-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="80e00-282">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="80e00-283">isEncrypted</span></span>|<span data-ttu-id="80e00-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-284">Boolean</span></span>|<span data-ttu-id="80e00-285">Status de criptografia do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80e00-286">userPrincipalName</span></span>|<span data-ttu-id="80e00-287">String</span><span class="sxs-lookup"><span data-stu-id="80e00-287">String</span></span>|<span data-ttu-id="80e00-288">Nome principal de usuário do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-289">modelo</span><span class="sxs-lookup"><span data-stu-id="80e00-289">model</span></span>|<span data-ttu-id="80e00-290">String</span><span class="sxs-lookup"><span data-stu-id="80e00-290">String</span></span>|<span data-ttu-id="80e00-291">Modelo do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-292">fabricante</span><span class="sxs-lookup"><span data-stu-id="80e00-292">manufacturer</span></span>|<span data-ttu-id="80e00-293">String</span><span class="sxs-lookup"><span data-stu-id="80e00-293">String</span></span>|<span data-ttu-id="80e00-294">Fabricante do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-295">imei</span><span class="sxs-lookup"><span data-stu-id="80e00-295">imei</span></span>|<span data-ttu-id="80e00-296">String</span><span class="sxs-lookup"><span data-stu-id="80e00-296">String</span></span>|<span data-ttu-id="80e00-297">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="80e00-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="80e00-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-299">DateTimeOffset</span></span>|<span data-ttu-id="80e00-300">O DateTime quando o período de cortesia de conformidade do dispositivo expira herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="80e00-301">serialNumber</span></span>|<span data-ttu-id="80e00-302">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80e00-302">String</span></span>|<span data-ttu-id="80e00-303">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="80e00-304">phoneNumber</span></span>|<span data-ttu-id="80e00-305">String</span><span class="sxs-lookup"><span data-stu-id="80e00-305">String</span></span>|<span data-ttu-id="80e00-306">Número de telefone do dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="80e00-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="80e00-308">String</span><span class="sxs-lookup"><span data-stu-id="80e00-308">String</span></span>|<span data-ttu-id="80e00-309">Nível de patch de segurança do Android herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="80e00-310">userDisplayName</span></span>|<span data-ttu-id="80e00-311">String</span><span class="sxs-lookup"><span data-stu-id="80e00-311">String</span></span>|<span data-ttu-id="80e00-312">Nome de exibição do usuário herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="80e00-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="80e00-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="80e00-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="80e00-315">Recursos habilitados pelo cliente do ConfigrMgr herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="80e00-316">wiFiMacAddress</span></span>|<span data-ttu-id="80e00-317">String</span><span class="sxs-lookup"><span data-stu-id="80e00-317">String</span></span>|<span data-ttu-id="80e00-318">MAC Wi-Fi herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="80e00-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="80e00-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="80e00-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="80e00-321">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-321">The device health attestation state.</span></span> <span data-ttu-id="80e00-322">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="80e00-323">subscriberCarrier</span></span>|<span data-ttu-id="80e00-324">String</span><span class="sxs-lookup"><span data-stu-id="80e00-324">String</span></span>|<span data-ttu-id="80e00-325">Operadora de assinante herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-326">meid</span><span class="sxs-lookup"><span data-stu-id="80e00-326">meid</span></span>|<span data-ttu-id="80e00-327">String</span><span class="sxs-lookup"><span data-stu-id="80e00-327">String</span></span>|<span data-ttu-id="80e00-328">MEID herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="80e00-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="80e00-330">Int64</span><span class="sxs-lookup"><span data-stu-id="80e00-330">Int64</span></span>|<span data-ttu-id="80e00-331">Armazenamento total em bytes herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="80e00-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="80e00-333">Int64</span><span class="sxs-lookup"><span data-stu-id="80e00-333">Int64</span></span>|<span data-ttu-id="80e00-334">Armazenamento gratuito em bytes herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="80e00-335">managedDeviceName</span></span>|<span data-ttu-id="80e00-336">String</span><span class="sxs-lookup"><span data-stu-id="80e00-336">String</span></span>|<span data-ttu-id="80e00-337">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="80e00-338">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="80e00-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="80e00-339">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="80e00-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="80e00-341">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="80e00-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="80e00-342">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="80e00-343">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e00-343">Read Only.</span></span> <span data-ttu-id="80e00-344">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="80e00-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="80e00-345">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="80e00-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="80e00-346">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="80e00-346">usersLoggedOn</span></span>|<span data-ttu-id="80e00-347">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="80e00-348">Indica os últimos usuários conectados de um dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-349">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="80e00-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="80e00-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-350">DateTimeOffset</span></span>|<span data-ttu-id="80e00-351">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="80e00-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="80e00-352">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="80e00-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="80e00-353">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e00-353">Read Only.</span></span> <span data-ttu-id="80e00-354">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-355">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="80e00-355">autopilotEnrolled</span></span>|<span data-ttu-id="80e00-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-356">Boolean</span></span>|<span data-ttu-id="80e00-357">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="80e00-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="80e00-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-359">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="80e00-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="80e00-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e00-360">Boolean</span></span>|<span data-ttu-id="80e00-361">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="80e00-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="80e00-362">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-363">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="80e00-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="80e00-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e00-364">DateTimeOffset</span></span>|<span data-ttu-id="80e00-365">Relata a data de expiração do certificado de gerenciamento de dispositivos herdada de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-366">ICCID</span><span class="sxs-lookup"><span data-stu-id="80e00-366">iccid</span></span>|<span data-ttu-id="80e00-367">String</span><span class="sxs-lookup"><span data-stu-id="80e00-367">String</span></span>|<span data-ttu-id="80e00-368">Identificador de cartão de circuito integrado, é O número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="80e00-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="80e00-369">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-370">UDID</span><span class="sxs-lookup"><span data-stu-id="80e00-370">udid</span></span>|<span data-ttu-id="80e00-371">String</span><span class="sxs-lookup"><span data-stu-id="80e00-371">String</span></span>|<span data-ttu-id="80e00-372">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="80e00-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="80e00-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-374">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80e00-374">roleScopeTagIds</span></span>|<span data-ttu-id="80e00-375">Coleção String</span><span class="sxs-lookup"><span data-stu-id="80e00-375">String collection</span></span>|<span data-ttu-id="80e00-376">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80e00-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="80e00-377">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-378">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="80e00-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="80e00-379">Int32</span><span class="sxs-lookup"><span data-stu-id="80e00-379">Int32</span></span>|<span data-ttu-id="80e00-380">Contagem de malware ativo para este dispositivo do Windows herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-381">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="80e00-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="80e00-382">Int32</span><span class="sxs-lookup"><span data-stu-id="80e00-382">Int32</span></span>|<span data-ttu-id="80e00-383">Contagem de malware corrigido para este dispositivo Windows herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-384">notes</span><span class="sxs-lookup"><span data-stu-id="80e00-384">notes</span></span>|<span data-ttu-id="80e00-385">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80e00-385">String</span></span>|<span data-ttu-id="80e00-386">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="80e00-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="80e00-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="80e00-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="80e00-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="80e00-389">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="80e00-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="80e00-390">Resposta</span><span class="sxs-lookup"><span data-stu-id="80e00-390">Response</span></span>
<span data-ttu-id="80e00-391">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80e00-391">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80e00-392">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80e00-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="80e00-393">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80e00-393">Request</span></span>
<span data-ttu-id="80e00-394">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80e00-394">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
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

### <a name="response"></a><span data-ttu-id="80e00-395">Resposta</span><span class="sxs-lookup"><span data-stu-id="80e00-395">Response</span></span>
<span data-ttu-id="80e00-p141">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80e00-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




