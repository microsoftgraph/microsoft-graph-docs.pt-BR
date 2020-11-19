---
title: Atualizar windowsManagedDevice
description: Atualiza as propriedades de um objeto windowsManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47f21dfeb3f1c88c681f25bb658d319739377880
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49218772"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="52949-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="52949-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="52949-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52949-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52949-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52949-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52949-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52949-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52949-107">Atualiza as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="52949-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52949-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52949-108">Prerequisites</span></span>
<span data-ttu-id="52949-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52949-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52949-111">Permission type</span></span>|<span data-ttu-id="52949-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52949-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52949-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52949-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52949-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52949-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52949-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52949-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52949-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52949-116">Not supported.</span></span>|
|<span data-ttu-id="52949-117">Application</span><span class="sxs-lookup"><span data-stu-id="52949-117">Application</span></span>|<span data-ttu-id="52949-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52949-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52949-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52949-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="52949-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52949-120">Request headers</span></span>
|<span data-ttu-id="52949-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52949-121">Header</span></span>|<span data-ttu-id="52949-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52949-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52949-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52949-123">Authorization</span></span>|<span data-ttu-id="52949-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52949-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52949-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52949-125">Accept</span></span>|<span data-ttu-id="52949-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52949-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52949-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52949-127">Request body</span></span>
<span data-ttu-id="52949-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="52949-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="52949-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="52949-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52949-130">Property</span></span>|<span data-ttu-id="52949-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52949-131">Type</span></span>|<span data-ttu-id="52949-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52949-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52949-133">id</span><span class="sxs-lookup"><span data-stu-id="52949-133">id</span></span>|<span data-ttu-id="52949-134">String</span><span class="sxs-lookup"><span data-stu-id="52949-134">String</span></span>|<span data-ttu-id="52949-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-135">Unique Identifier for the device.</span></span> <span data-ttu-id="52949-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-136">This property is read-only.</span></span> <span data-ttu-id="52949-137">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-138">userId</span><span class="sxs-lookup"><span data-stu-id="52949-138">userId</span></span>|<span data-ttu-id="52949-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52949-139">String</span></span>|<span data-ttu-id="52949-140">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="52949-141">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-141">This property is read-only.</span></span> <span data-ttu-id="52949-142">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="52949-143">deviceName</span></span>|<span data-ttu-id="52949-144">String</span><span class="sxs-lookup"><span data-stu-id="52949-144">String</span></span>|<span data-ttu-id="52949-145">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-145">Name of the device.</span></span> <span data-ttu-id="52949-146">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-146">This property is read-only.</span></span> <span data-ttu-id="52949-147">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="52949-148">hardwareInformation</span></span>|[<span data-ttu-id="52949-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="52949-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="52949-150">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-150">The hardward details for the device.</span></span>  <span data-ttu-id="52949-151">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="52949-152">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="52949-153">ownerType</span></span>|[<span data-ttu-id="52949-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="52949-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="52949-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-155">Ownership of the device.</span></span> <span data-ttu-id="52949-156">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="52949-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="52949-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="52949-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="52949-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="52949-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="52949-160">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-160">Ownership of the device.</span></span> <span data-ttu-id="52949-161">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-162">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="52949-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="52949-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="52949-163">deviceActionResults</span></span>|<span data-ttu-id="52949-164">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="52949-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="52949-165">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="52949-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="52949-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-166">This property is read-only.</span></span> <span data-ttu-id="52949-167">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="52949-168">managementState</span></span>|[<span data-ttu-id="52949-169">ManagementState</span><span class="sxs-lookup"><span data-stu-id="52949-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="52949-170">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-170">Management state of the device.</span></span> <span data-ttu-id="52949-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-171">This property is read-only.</span></span> <span data-ttu-id="52949-172">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-173">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="52949-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="52949-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-174">enrolledDateTime</span></span>|<span data-ttu-id="52949-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-175">DateTimeOffset</span></span>|<span data-ttu-id="52949-176">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-176">Enrollment time of the device.</span></span> <span data-ttu-id="52949-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-177">This property is read-only.</span></span> <span data-ttu-id="52949-178">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-179">lastSyncDateTime</span></span>|<span data-ttu-id="52949-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-180">DateTimeOffset</span></span>|<span data-ttu-id="52949-181">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="52949-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="52949-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-182">This property is read-only.</span></span> <span data-ttu-id="52949-183">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="52949-184">chassisType</span></span>|[<span data-ttu-id="52949-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="52949-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="52949-186">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-186">Chassis type of the device.</span></span> <span data-ttu-id="52949-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-187">This property is read-only.</span></span> <span data-ttu-id="52949-188">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-189">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="52949-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="52949-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="52949-190">operatingSystem</span></span>|<span data-ttu-id="52949-191">String</span><span class="sxs-lookup"><span data-stu-id="52949-191">String</span></span>|<span data-ttu-id="52949-192">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-192">Operating system of the device.</span></span> <span data-ttu-id="52949-193">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="52949-194">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="52949-195">deviceType</span></span>|[<span data-ttu-id="52949-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="52949-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="52949-197">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-197">Platform of the device.</span></span> <span data-ttu-id="52949-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-198">This property is read-only.</span></span> <span data-ttu-id="52949-199">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-200">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `blackberry` `palm` `unknown` `cloudPC` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="52949-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="52949-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="52949-201">complianceState</span></span>|[<span data-ttu-id="52949-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="52949-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="52949-203">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-203">Compliance state of the device.</span></span> <span data-ttu-id="52949-204">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-204">This property is read-only.</span></span> <span data-ttu-id="52949-205">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-206">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="52949-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="52949-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="52949-207">jailBroken</span></span>|<span data-ttu-id="52949-208">String</span><span class="sxs-lookup"><span data-stu-id="52949-208">String</span></span>|<span data-ttu-id="52949-209">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="52949-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="52949-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-210">This property is read-only.</span></span> <span data-ttu-id="52949-211">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="52949-212">managementAgent</span></span>|[<span data-ttu-id="52949-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="52949-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="52949-214">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-214">Management channel of the device.</span></span> <span data-ttu-id="52949-215">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="52949-216">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-217">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="52949-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="52949-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="52949-218">osVersion</span></span>|<span data-ttu-id="52949-219">String</span><span class="sxs-lookup"><span data-stu-id="52949-219">String</span></span>|<span data-ttu-id="52949-220">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-220">Operating system version of the device.</span></span> <span data-ttu-id="52949-221">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-221">This property is read-only.</span></span> <span data-ttu-id="52949-222">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="52949-223">easActivated</span></span>|<span data-ttu-id="52949-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="52949-224">Boolean</span></span>|<span data-ttu-id="52949-225">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="52949-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="52949-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-226">This property is read-only.</span></span> <span data-ttu-id="52949-227">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="52949-228">easDeviceId</span></span>|<span data-ttu-id="52949-229">String</span><span class="sxs-lookup"><span data-stu-id="52949-229">String</span></span>|<span data-ttu-id="52949-230">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="52949-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-231">This property is read-only.</span></span> <span data-ttu-id="52949-232">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-233">easActivationDateTime</span></span>|<span data-ttu-id="52949-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-234">DateTimeOffset</span></span>|<span data-ttu-id="52949-235">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="52949-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-236">This property is read-only.</span></span> <span data-ttu-id="52949-237">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="52949-238">aadRegistered</span></span>|<span data-ttu-id="52949-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="52949-239">Boolean</span></span>|<span data-ttu-id="52949-240">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52949-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="52949-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-241">This property is read-only.</span></span> <span data-ttu-id="52949-242">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="52949-243">azureADRegistered</span></span>|<span data-ttu-id="52949-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="52949-244">Boolean</span></span>|<span data-ttu-id="52949-245">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52949-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="52949-246">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-246">This property is read-only.</span></span> <span data-ttu-id="52949-247">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="52949-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="52949-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="52949-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="52949-250">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-250">Enrollment type of the device.</span></span> <span data-ttu-id="52949-251">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-251">This property is read-only.</span></span> <span data-ttu-id="52949-252">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-253">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="52949-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="52949-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="52949-254">lostModeState</span></span>|[<span data-ttu-id="52949-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="52949-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="52949-256">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="52949-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="52949-257">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-257">This property is read-only.</span></span> <span data-ttu-id="52949-258">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-259">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="52949-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="52949-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="52949-260">activationLockBypassCode</span></span>|<span data-ttu-id="52949-261">String</span><span class="sxs-lookup"><span data-stu-id="52949-261">String</span></span>|<span data-ttu-id="52949-262">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="52949-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="52949-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-263">This property is read-only.</span></span> <span data-ttu-id="52949-264">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="52949-265">emailAddress</span></span>|<span data-ttu-id="52949-266">String</span><span class="sxs-lookup"><span data-stu-id="52949-266">String</span></span>|<span data-ttu-id="52949-267">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="52949-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-268">This property is read-only.</span></span> <span data-ttu-id="52949-269">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="52949-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="52949-271">String</span><span class="sxs-lookup"><span data-stu-id="52949-271">String</span></span>|<span data-ttu-id="52949-272">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52949-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="52949-273">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-273">Read only.</span></span> <span data-ttu-id="52949-274">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-274">This property is read-only.</span></span> <span data-ttu-id="52949-275">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="52949-276">azureADDeviceId</span></span>|<span data-ttu-id="52949-277">String</span><span class="sxs-lookup"><span data-stu-id="52949-277">String</span></span>|<span data-ttu-id="52949-278">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52949-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="52949-279">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-279">Read only.</span></span> <span data-ttu-id="52949-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-280">This property is read-only.</span></span> <span data-ttu-id="52949-281">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="52949-282">deviceRegistrationState</span></span>|[<span data-ttu-id="52949-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="52949-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="52949-284">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-284">Device registration state.</span></span> <span data-ttu-id="52949-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-285">This property is read-only.</span></span> <span data-ttu-id="52949-286">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-287">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="52949-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="52949-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="52949-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="52949-289">String</span><span class="sxs-lookup"><span data-stu-id="52949-289">String</span></span>|<span data-ttu-id="52949-290">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-290">Device category display name.</span></span> <span data-ttu-id="52949-291">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-291">This property is read-only.</span></span> <span data-ttu-id="52949-292">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="52949-293">isSupervised</span></span>|<span data-ttu-id="52949-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="52949-294">Boolean</span></span>|<span data-ttu-id="52949-295">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-295">Device supervised status.</span></span> <span data-ttu-id="52949-296">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-296">This property is read-only.</span></span> <span data-ttu-id="52949-297">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="52949-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-299">DateTimeOffset</span></span>|<span data-ttu-id="52949-300">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="52949-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="52949-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-301">This property is read-only.</span></span> <span data-ttu-id="52949-302">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="52949-303">exchangeAccessState</span></span>|[<span data-ttu-id="52949-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="52949-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="52949-305">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="52949-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="52949-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-306">This property is read-only.</span></span> <span data-ttu-id="52949-307">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-308">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="52949-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="52949-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="52949-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="52949-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="52949-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="52949-311">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="52949-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="52949-312">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-312">This property is read-only.</span></span> <span data-ttu-id="52949-313">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-314">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="52949-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="52949-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="52949-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="52949-316">String</span><span class="sxs-lookup"><span data-stu-id="52949-316">String</span></span>|<span data-ttu-id="52949-317">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="52949-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-318">This property is read-only.</span></span> <span data-ttu-id="52949-319">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="52949-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="52949-321">String</span><span class="sxs-lookup"><span data-stu-id="52949-321">String</span></span>|<span data-ttu-id="52949-322">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="52949-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="52949-323">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-323">This property is read-only.</span></span> <span data-ttu-id="52949-324">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="52949-325">isEncrypted</span></span>|<span data-ttu-id="52949-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="52949-326">Boolean</span></span>|<span data-ttu-id="52949-327">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-327">Device encryption status.</span></span> <span data-ttu-id="52949-328">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-328">This property is read-only.</span></span> <span data-ttu-id="52949-329">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52949-330">userPrincipalName</span></span>|<span data-ttu-id="52949-331">String</span><span class="sxs-lookup"><span data-stu-id="52949-331">String</span></span>|<span data-ttu-id="52949-332">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-332">Device user principal name.</span></span> <span data-ttu-id="52949-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-333">This property is read-only.</span></span> <span data-ttu-id="52949-334">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-335">modelo</span><span class="sxs-lookup"><span data-stu-id="52949-335">model</span></span>|<span data-ttu-id="52949-336">String</span><span class="sxs-lookup"><span data-stu-id="52949-336">String</span></span>|<span data-ttu-id="52949-337">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-337">Model of the device.</span></span> <span data-ttu-id="52949-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-338">This property is read-only.</span></span> <span data-ttu-id="52949-339">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-340">fabricante</span><span class="sxs-lookup"><span data-stu-id="52949-340">manufacturer</span></span>|<span data-ttu-id="52949-341">String</span><span class="sxs-lookup"><span data-stu-id="52949-341">String</span></span>|<span data-ttu-id="52949-342">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-342">Manufacturer of the device.</span></span> <span data-ttu-id="52949-343">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-343">This property is read-only.</span></span> <span data-ttu-id="52949-344">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-345">imei</span><span class="sxs-lookup"><span data-stu-id="52949-345">imei</span></span>|<span data-ttu-id="52949-346">String</span><span class="sxs-lookup"><span data-stu-id="52949-346">String</span></span>|<span data-ttu-id="52949-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="52949-347">IMEI.</span></span> <span data-ttu-id="52949-348">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-348">This property is read-only.</span></span> <span data-ttu-id="52949-349">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="52949-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-351">DateTimeOffset</span></span>|<span data-ttu-id="52949-352">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="52949-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="52949-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-353">This property is read-only.</span></span> <span data-ttu-id="52949-354">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="52949-355">serialNumber</span></span>|<span data-ttu-id="52949-356">String</span><span class="sxs-lookup"><span data-stu-id="52949-356">String</span></span>|<span data-ttu-id="52949-357">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="52949-357">SerialNumber.</span></span> <span data-ttu-id="52949-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-358">This property is read-only.</span></span> <span data-ttu-id="52949-359">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="52949-360">phoneNumber</span></span>|<span data-ttu-id="52949-361">String</span><span class="sxs-lookup"><span data-stu-id="52949-361">String</span></span>|<span data-ttu-id="52949-362">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-362">Phone number of the device.</span></span> <span data-ttu-id="52949-363">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-363">This property is read-only.</span></span> <span data-ttu-id="52949-364">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="52949-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="52949-366">String</span><span class="sxs-lookup"><span data-stu-id="52949-366">String</span></span>|<span data-ttu-id="52949-367">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="52949-367">Android security patch level.</span></span> <span data-ttu-id="52949-368">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-368">This property is read-only.</span></span> <span data-ttu-id="52949-369">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="52949-370">userDisplayName</span></span>|<span data-ttu-id="52949-371">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52949-371">String</span></span>|<span data-ttu-id="52949-372">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="52949-372">User display name.</span></span> <span data-ttu-id="52949-373">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-373">This property is read-only.</span></span> <span data-ttu-id="52949-374">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="52949-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="52949-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="52949-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="52949-377">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="52949-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="52949-378">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-378">This property is read-only.</span></span> <span data-ttu-id="52949-379">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="52949-380">wiFiMacAddress</span></span>|<span data-ttu-id="52949-381">String</span><span class="sxs-lookup"><span data-stu-id="52949-381">String</span></span>|<span data-ttu-id="52949-382">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="52949-382">Wi-Fi MAC.</span></span> <span data-ttu-id="52949-383">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-383">This property is read-only.</span></span> <span data-ttu-id="52949-384">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="52949-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="52949-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="52949-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="52949-387">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-387">The device health attestation state.</span></span> <span data-ttu-id="52949-388">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-388">This property is read-only.</span></span> <span data-ttu-id="52949-389">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="52949-390">subscriberCarrier</span></span>|<span data-ttu-id="52949-391">String</span><span class="sxs-lookup"><span data-stu-id="52949-391">String</span></span>|<span data-ttu-id="52949-392">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="52949-392">Subscriber Carrier.</span></span> <span data-ttu-id="52949-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-393">This property is read-only.</span></span> <span data-ttu-id="52949-394">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-395">meid</span><span class="sxs-lookup"><span data-stu-id="52949-395">meid</span></span>|<span data-ttu-id="52949-396">String</span><span class="sxs-lookup"><span data-stu-id="52949-396">String</span></span>|<span data-ttu-id="52949-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="52949-397">MEID.</span></span> <span data-ttu-id="52949-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-398">This property is read-only.</span></span> <span data-ttu-id="52949-399">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="52949-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="52949-401">Int64</span><span class="sxs-lookup"><span data-stu-id="52949-401">Int64</span></span>|<span data-ttu-id="52949-402">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="52949-402">Total Storage in Bytes.</span></span> <span data-ttu-id="52949-403">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-403">This property is read-only.</span></span> <span data-ttu-id="52949-404">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="52949-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="52949-406">Int64</span><span class="sxs-lookup"><span data-stu-id="52949-406">Int64</span></span>|<span data-ttu-id="52949-407">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="52949-407">Free Storage in Bytes.</span></span> <span data-ttu-id="52949-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-408">This property is read-only.</span></span> <span data-ttu-id="52949-409">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="52949-410">managedDeviceName</span></span>|<span data-ttu-id="52949-411">String</span><span class="sxs-lookup"><span data-stu-id="52949-411">String</span></span>|<span data-ttu-id="52949-412">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="52949-413">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="52949-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="52949-414">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="52949-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="52949-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="52949-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="52949-417">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="52949-418">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-418">Read Only.</span></span> <span data-ttu-id="52949-419">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-419">This property is read-only.</span></span> <span data-ttu-id="52949-420">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-421">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="52949-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="52949-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-422">retireAfterDateTime</span></span>|<span data-ttu-id="52949-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-423">DateTimeOffset</span></span>|<span data-ttu-id="52949-424">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="52949-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="52949-425">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-425">This property is read-only.</span></span> <span data-ttu-id="52949-426">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="52949-427">usersLoggedOn</span></span>|<span data-ttu-id="52949-428">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="52949-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="52949-429">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="52949-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-430">This property is read-only.</span></span> <span data-ttu-id="52949-431">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="52949-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="52949-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-433">DateTimeOffset</span></span>|<span data-ttu-id="52949-434">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="52949-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="52949-435">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="52949-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="52949-436">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-436">Read Only.</span></span> <span data-ttu-id="52949-437">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-437">This property is read-only.</span></span> <span data-ttu-id="52949-438">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="52949-439">autopilotEnrolled</span></span>|<span data-ttu-id="52949-440">Booliano</span><span class="sxs-lookup"><span data-stu-id="52949-440">Boolean</span></span>|<span data-ttu-id="52949-441">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="52949-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="52949-442">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-442">This property is read-only.</span></span> <span data-ttu-id="52949-443">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="52949-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="52949-445">Booliano</span><span class="sxs-lookup"><span data-stu-id="52949-445">Boolean</span></span>|<span data-ttu-id="52949-446">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="52949-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="52949-447">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-447">This property is read-only.</span></span> <span data-ttu-id="52949-448">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="52949-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="52949-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52949-450">DateTimeOffset</span></span>|<span data-ttu-id="52949-451">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="52949-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="52949-452">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-452">This property is read-only.</span></span> <span data-ttu-id="52949-453">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-454">iccid</span><span class="sxs-lookup"><span data-stu-id="52949-454">iccid</span></span>|<span data-ttu-id="52949-455">String</span><span class="sxs-lookup"><span data-stu-id="52949-455">String</span></span>|<span data-ttu-id="52949-456">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="52949-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="52949-457">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-457">This property is read-only.</span></span> <span data-ttu-id="52949-458">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-459">udid</span><span class="sxs-lookup"><span data-stu-id="52949-459">udid</span></span>|<span data-ttu-id="52949-460">String</span><span class="sxs-lookup"><span data-stu-id="52949-460">String</span></span>|<span data-ttu-id="52949-461">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="52949-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="52949-462">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-462">This property is read-only.</span></span> <span data-ttu-id="52949-463">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="52949-464">roleScopeTagIds</span></span>|<span data-ttu-id="52949-465">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="52949-465">String collection</span></span>|<span data-ttu-id="52949-466">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52949-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="52949-467">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="52949-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="52949-469">Int32</span><span class="sxs-lookup"><span data-stu-id="52949-469">Int32</span></span>|<span data-ttu-id="52949-470">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="52949-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="52949-471">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-471">This property is read-only.</span></span> <span data-ttu-id="52949-472">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="52949-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="52949-474">Int32</span><span class="sxs-lookup"><span data-stu-id="52949-474">Int32</span></span>|<span data-ttu-id="52949-475">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="52949-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="52949-476">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-476">This property is read-only.</span></span> <span data-ttu-id="52949-477">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-478">notes</span><span class="sxs-lookup"><span data-stu-id="52949-478">notes</span></span>|<span data-ttu-id="52949-479">String</span><span class="sxs-lookup"><span data-stu-id="52949-479">String</span></span>|<span data-ttu-id="52949-480">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="52949-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="52949-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="52949-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="52949-483">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="52949-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="52949-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="52949-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="52949-486">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="52949-487">ethernetMacAddress</span></span>|<span data-ttu-id="52949-488">String</span><span class="sxs-lookup"><span data-stu-id="52949-488">String</span></span>|<span data-ttu-id="52949-489">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="52949-489">Ethernet MAC.</span></span> <span data-ttu-id="52949-490">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-490">This property is read-only.</span></span> <span data-ttu-id="52949-491">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="52949-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="52949-493">Int64</span><span class="sxs-lookup"><span data-stu-id="52949-493">Int64</span></span>|<span data-ttu-id="52949-494">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="52949-494">Total Memory in Bytes.</span></span> <span data-ttu-id="52949-495">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-495">This property is read-only.</span></span> <span data-ttu-id="52949-496">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="52949-497">processorArchitecture</span></span>|[<span data-ttu-id="52949-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="52949-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="52949-499">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="52949-499">Processor architecture.</span></span> <span data-ttu-id="52949-500">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-500">This property is read-only.</span></span> <span data-ttu-id="52949-501">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-502">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="52949-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="52949-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="52949-503">specificationVersion</span></span>|<span data-ttu-id="52949-504">String</span><span class="sxs-lookup"><span data-stu-id="52949-504">String</span></span>|<span data-ttu-id="52949-505">Versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="52949-505">Specification version.</span></span> <span data-ttu-id="52949-506">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-506">This property is read-only.</span></span> <span data-ttu-id="52949-507">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-508">joinType</span><span class="sxs-lookup"><span data-stu-id="52949-508">joinType</span></span>|[<span data-ttu-id="52949-509">joinType</span><span class="sxs-lookup"><span data-stu-id="52949-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="52949-510">Tipo de ingresso de dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-511">Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="52949-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="52949-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="52949-512">skuFamily</span></span>|<span data-ttu-id="52949-513">String</span><span class="sxs-lookup"><span data-stu-id="52949-513">String</span></span>|<span data-ttu-id="52949-514">Família de SKU do dispositivo herdada de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="52949-515">skuNumber</span></span>|<span data-ttu-id="52949-516">Int32</span><span class="sxs-lookup"><span data-stu-id="52949-516">Int32</span></span>|<span data-ttu-id="52949-517">Número de SKU do dispositivo, Confira também: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="52949-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="52949-518">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="52949-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="52949-519">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52949-519">This property is read-only.</span></span> <span data-ttu-id="52949-520">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="52949-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="52949-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="52949-521">managementFeatures</span></span>|[<span data-ttu-id="52949-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="52949-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="52949-523">Recursos de gerenciamento de dispositivos herdados do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="52949-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="52949-524">Os valores possíveis são: `none` e `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="52949-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="52949-525">Resposta</span><span class="sxs-lookup"><span data-stu-id="52949-525">Response</span></span>
<span data-ttu-id="52949-526">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52949-526">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52949-527">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52949-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="52949-528">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52949-528">Request</span></span>
<span data-ttu-id="52949-529">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52949-529">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8115

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

### <a name="response"></a><span data-ttu-id="52949-530">Resposta</span><span class="sxs-lookup"><span data-stu-id="52949-530">Response</span></span>
<span data-ttu-id="52949-p175">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52949-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8164

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




