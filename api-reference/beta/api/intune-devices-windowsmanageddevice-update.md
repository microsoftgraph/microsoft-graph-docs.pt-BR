---
title: Atualizar windowsManagedDevice
description: Atualiza as propriedades de um objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f8b0f597cf6bd763b78a34044b12e1daf147df60
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161780"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="2ee53-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="2ee53-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="2ee53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ee53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ee53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ee53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ee53-106">Atualiza as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="2ee53-106">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ee53-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ee53-107">Prerequisites</span></span>
<span data-ttu-id="2ee53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ee53-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ee53-110">Permission type</span></span>|<span data-ttu-id="2ee53-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ee53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ee53-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ee53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ee53-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee53-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ee53-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ee53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ee53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ee53-115">Not supported.</span></span>|
|<span data-ttu-id="2ee53-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ee53-116">Application</span></span>|<span data-ttu-id="2ee53-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee53-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ee53-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee53-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2ee53-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee53-119">Request headers</span></span>
|<span data-ttu-id="2ee53-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ee53-120">Header</span></span>|<span data-ttu-id="2ee53-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ee53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ee53-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ee53-122">Authorization</span></span>|<span data-ttu-id="2ee53-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ee53-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ee53-124">Accept</span></span>|<span data-ttu-id="2ee53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ee53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ee53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee53-126">Request body</span></span>
<span data-ttu-id="2ee53-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="2ee53-127">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="2ee53-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-128">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="2ee53-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ee53-129">Property</span></span>|<span data-ttu-id="2ee53-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ee53-130">Type</span></span>|<span data-ttu-id="2ee53-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ee53-132">id</span><span class="sxs-lookup"><span data-stu-id="2ee53-132">id</span></span>|<span data-ttu-id="2ee53-133">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-133">String</span></span>|<span data-ttu-id="2ee53-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-134">Unique Identifier for the device.</span></span> <span data-ttu-id="2ee53-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-135">This property is read-only.</span></span> <span data-ttu-id="2ee53-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-137">userId</span><span class="sxs-lookup"><span data-stu-id="2ee53-137">userId</span></span>|<span data-ttu-id="2ee53-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee53-138">String</span></span>|<span data-ttu-id="2ee53-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="2ee53-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-140">This property is read-only.</span></span> <span data-ttu-id="2ee53-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="2ee53-142">deviceName</span></span>|<span data-ttu-id="2ee53-143">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-143">String</span></span>|<span data-ttu-id="2ee53-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-144">Name of the device.</span></span> <span data-ttu-id="2ee53-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-145">This property is read-only.</span></span> <span data-ttu-id="2ee53-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="2ee53-147">hardwareInformation</span></span>|[<span data-ttu-id="2ee53-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="2ee53-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="2ee53-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-149">The hardward details for the device.</span></span>  <span data-ttu-id="2ee53-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="2ee53-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="2ee53-152">ownerType</span></span>|[<span data-ttu-id="2ee53-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="2ee53-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="2ee53-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-154">Ownership of the device.</span></span> <span data-ttu-id="2ee53-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="2ee53-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="2ee53-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="2ee53-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="2ee53-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="2ee53-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-159">Ownership of the device.</span></span> <span data-ttu-id="2ee53-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="2ee53-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="2ee53-162">deviceActionResults</span></span>|<span data-ttu-id="2ee53-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="2ee53-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="2ee53-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="2ee53-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-165">This property is read-only.</span></span> <span data-ttu-id="2ee53-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="2ee53-167">managementState</span></span>|[<span data-ttu-id="2ee53-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="2ee53-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="2ee53-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-169">Management state of the device.</span></span> <span data-ttu-id="2ee53-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-170">This property is read-only.</span></span> <span data-ttu-id="2ee53-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="2ee53-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-173">enrolledDateTime</span></span>|<span data-ttu-id="2ee53-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-174">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-175">Enrollment time of the device.</span></span> <span data-ttu-id="2ee53-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-176">This property is read-only.</span></span> <span data-ttu-id="2ee53-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-178">lastSyncDateTime</span></span>|<span data-ttu-id="2ee53-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-179">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="2ee53-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="2ee53-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-181">This property is read-only.</span></span> <span data-ttu-id="2ee53-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="2ee53-183">chassisType</span></span>|[<span data-ttu-id="2ee53-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="2ee53-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="2ee53-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-185">Chassis type of the device.</span></span> <span data-ttu-id="2ee53-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-186">This property is read-only.</span></span> <span data-ttu-id="2ee53-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="2ee53-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ee53-189">operatingSystem</span></span>|<span data-ttu-id="2ee53-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee53-190">String</span></span>|<span data-ttu-id="2ee53-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-191">Operating system of the device.</span></span> <span data-ttu-id="2ee53-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="2ee53-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="2ee53-194">deviceType</span></span>|[<span data-ttu-id="2ee53-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="2ee53-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="2ee53-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-196">Platform of the device.</span></span> <span data-ttu-id="2ee53-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-197">This property is read-only.</span></span> <span data-ttu-id="2ee53-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="2ee53-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="2ee53-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="2ee53-200">complianceState</span></span>|[<span data-ttu-id="2ee53-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="2ee53-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="2ee53-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-202">Compliance state of the device.</span></span> <span data-ttu-id="2ee53-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-203">This property is read-only.</span></span> <span data-ttu-id="2ee53-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="2ee53-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="2ee53-206">jailBroken</span></span>|<span data-ttu-id="2ee53-207">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-207">String</span></span>|<span data-ttu-id="2ee53-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="2ee53-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="2ee53-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-209">This property is read-only.</span></span> <span data-ttu-id="2ee53-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="2ee53-211">managementAgent</span></span>|[<span data-ttu-id="2ee53-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="2ee53-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="2ee53-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-213">Management channel of the device.</span></span> <span data-ttu-id="2ee53-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="2ee53-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="2ee53-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="2ee53-217">osVersion</span></span>|<span data-ttu-id="2ee53-218">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-218">String</span></span>|<span data-ttu-id="2ee53-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-219">Operating system version of the device.</span></span> <span data-ttu-id="2ee53-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-220">This property is read-only.</span></span> <span data-ttu-id="2ee53-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="2ee53-222">easActivated</span></span>|<span data-ttu-id="2ee53-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee53-223">Boolean</span></span>|<span data-ttu-id="2ee53-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="2ee53-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="2ee53-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-225">This property is read-only.</span></span> <span data-ttu-id="2ee53-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="2ee53-227">easDeviceId</span></span>|<span data-ttu-id="2ee53-228">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-228">String</span></span>|<span data-ttu-id="2ee53-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="2ee53-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-230">This property is read-only.</span></span> <span data-ttu-id="2ee53-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-232">easActivationDateTime</span></span>|<span data-ttu-id="2ee53-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-233">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="2ee53-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-235">This property is read-only.</span></span> <span data-ttu-id="2ee53-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="2ee53-237">aadRegistered</span></span>|<span data-ttu-id="2ee53-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee53-238">Boolean</span></span>|<span data-ttu-id="2ee53-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ee53-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="2ee53-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-240">This property is read-only.</span></span> <span data-ttu-id="2ee53-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="2ee53-242">azureADRegistered</span></span>|<span data-ttu-id="2ee53-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee53-243">Boolean</span></span>|<span data-ttu-id="2ee53-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ee53-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="2ee53-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-245">This property is read-only.</span></span> <span data-ttu-id="2ee53-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="2ee53-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="2ee53-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="2ee53-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="2ee53-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-249">Enrollment type of the device.</span></span> <span data-ttu-id="2ee53-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-250">This property is read-only.</span></span> <span data-ttu-id="2ee53-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="2ee53-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="2ee53-253">lostModeState</span></span>|[<span data-ttu-id="2ee53-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="2ee53-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="2ee53-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2ee53-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="2ee53-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-256">This property is read-only.</span></span> <span data-ttu-id="2ee53-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="2ee53-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="2ee53-259">activationLockBypassCode</span></span>|<span data-ttu-id="2ee53-260">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-260">String</span></span>|<span data-ttu-id="2ee53-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="2ee53-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="2ee53-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-262">This property is read-only.</span></span> <span data-ttu-id="2ee53-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2ee53-264">emailAddress</span></span>|<span data-ttu-id="2ee53-265">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-265">String</span></span>|<span data-ttu-id="2ee53-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="2ee53-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-267">This property is read-only.</span></span> <span data-ttu-id="2ee53-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="2ee53-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="2ee53-270">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-270">String</span></span>|<span data-ttu-id="2ee53-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ee53-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="2ee53-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-272">Read only.</span></span> <span data-ttu-id="2ee53-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-273">This property is read-only.</span></span> <span data-ttu-id="2ee53-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="2ee53-275">azureADDeviceId</span></span>|<span data-ttu-id="2ee53-276">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-276">String</span></span>|<span data-ttu-id="2ee53-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2ee53-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="2ee53-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-278">Read only.</span></span> <span data-ttu-id="2ee53-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-279">This property is read-only.</span></span> <span data-ttu-id="2ee53-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="2ee53-281">deviceRegistrationState</span></span>|[<span data-ttu-id="2ee53-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="2ee53-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="2ee53-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-283">Device registration state.</span></span> <span data-ttu-id="2ee53-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-284">This property is read-only.</span></span> <span data-ttu-id="2ee53-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="2ee53-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ee53-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="2ee53-288">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-288">String</span></span>|<span data-ttu-id="2ee53-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-289">Device category display name.</span></span> <span data-ttu-id="2ee53-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-290">This property is read-only.</span></span> <span data-ttu-id="2ee53-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="2ee53-292">isSupervised</span></span>|<span data-ttu-id="2ee53-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee53-293">Boolean</span></span>|<span data-ttu-id="2ee53-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-294">Device supervised status.</span></span> <span data-ttu-id="2ee53-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-295">This property is read-only.</span></span> <span data-ttu-id="2ee53-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="2ee53-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-298">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ee53-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="2ee53-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-300">This property is read-only.</span></span> <span data-ttu-id="2ee53-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="2ee53-302">exchangeAccessState</span></span>|[<span data-ttu-id="2ee53-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="2ee53-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="2ee53-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ee53-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="2ee53-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-305">This property is read-only.</span></span> <span data-ttu-id="2ee53-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="2ee53-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="2ee53-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="2ee53-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="2ee53-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="2ee53-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ee53-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="2ee53-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-311">This property is read-only.</span></span> <span data-ttu-id="2ee53-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="2ee53-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="2ee53-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="2ee53-315">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-315">String</span></span>|<span data-ttu-id="2ee53-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="2ee53-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-317">This property is read-only.</span></span> <span data-ttu-id="2ee53-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="2ee53-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="2ee53-320">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-320">String</span></span>|<span data-ttu-id="2ee53-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="2ee53-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="2ee53-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-322">This property is read-only.</span></span> <span data-ttu-id="2ee53-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="2ee53-324">isEncrypted</span></span>|<span data-ttu-id="2ee53-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ee53-325">Boolean</span></span>|<span data-ttu-id="2ee53-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-326">Device encryption status.</span></span> <span data-ttu-id="2ee53-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-327">This property is read-only.</span></span> <span data-ttu-id="2ee53-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ee53-329">userPrincipalName</span></span>|<span data-ttu-id="2ee53-330">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-330">String</span></span>|<span data-ttu-id="2ee53-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-331">Device user principal name.</span></span> <span data-ttu-id="2ee53-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-332">This property is read-only.</span></span> <span data-ttu-id="2ee53-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-334">modelo</span><span class="sxs-lookup"><span data-stu-id="2ee53-334">model</span></span>|<span data-ttu-id="2ee53-335">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-335">String</span></span>|<span data-ttu-id="2ee53-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-336">Model of the device.</span></span> <span data-ttu-id="2ee53-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-337">This property is read-only.</span></span> <span data-ttu-id="2ee53-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="2ee53-339">manufacturer</span></span>|<span data-ttu-id="2ee53-340">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-340">String</span></span>|<span data-ttu-id="2ee53-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-341">Manufacturer of the device.</span></span> <span data-ttu-id="2ee53-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-342">This property is read-only.</span></span> <span data-ttu-id="2ee53-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-344">imei</span><span class="sxs-lookup"><span data-stu-id="2ee53-344">imei</span></span>|<span data-ttu-id="2ee53-345">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-345">String</span></span>|<span data-ttu-id="2ee53-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="2ee53-346">IMEI.</span></span> <span data-ttu-id="2ee53-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-347">This property is read-only.</span></span> <span data-ttu-id="2ee53-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2ee53-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-350">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="2ee53-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="2ee53-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-352">This property is read-only.</span></span> <span data-ttu-id="2ee53-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2ee53-354">serialNumber</span></span>|<span data-ttu-id="2ee53-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee53-355">String</span></span>|<span data-ttu-id="2ee53-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="2ee53-356">SerialNumber.</span></span> <span data-ttu-id="2ee53-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-357">This property is read-only.</span></span> <span data-ttu-id="2ee53-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="2ee53-359">phoneNumber</span></span>|<span data-ttu-id="2ee53-360">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-360">String</span></span>|<span data-ttu-id="2ee53-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-361">Phone number of the device.</span></span> <span data-ttu-id="2ee53-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-362">This property is read-only.</span></span> <span data-ttu-id="2ee53-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="2ee53-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="2ee53-365">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-365">String</span></span>|<span data-ttu-id="2ee53-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="2ee53-366">Android security patch level.</span></span> <span data-ttu-id="2ee53-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-367">This property is read-only.</span></span> <span data-ttu-id="2ee53-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ee53-369">userDisplayName</span></span>|<span data-ttu-id="2ee53-370">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-370">String</span></span>|<span data-ttu-id="2ee53-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ee53-371">User display name.</span></span> <span data-ttu-id="2ee53-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-372">This property is read-only.</span></span> <span data-ttu-id="2ee53-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="2ee53-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="2ee53-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="2ee53-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="2ee53-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="2ee53-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="2ee53-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-377">This property is read-only.</span></span> <span data-ttu-id="2ee53-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="2ee53-379">wiFiMacAddress</span></span>|<span data-ttu-id="2ee53-380">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-380">String</span></span>|<span data-ttu-id="2ee53-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="2ee53-381">Wi-Fi MAC.</span></span> <span data-ttu-id="2ee53-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-382">This property is read-only.</span></span> <span data-ttu-id="2ee53-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="2ee53-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="2ee53-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="2ee53-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="2ee53-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-386">The device health attestation state.</span></span> <span data-ttu-id="2ee53-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-387">This property is read-only.</span></span> <span data-ttu-id="2ee53-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="2ee53-389">subscriberCarrier</span></span>|<span data-ttu-id="2ee53-390">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-390">String</span></span>|<span data-ttu-id="2ee53-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="2ee53-391">Subscriber Carrier.</span></span> <span data-ttu-id="2ee53-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-392">This property is read-only.</span></span> <span data-ttu-id="2ee53-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-394">meid</span><span class="sxs-lookup"><span data-stu-id="2ee53-394">meid</span></span>|<span data-ttu-id="2ee53-395">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-395">String</span></span>|<span data-ttu-id="2ee53-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="2ee53-396">MEID.</span></span> <span data-ttu-id="2ee53-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-397">This property is read-only.</span></span> <span data-ttu-id="2ee53-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="2ee53-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="2ee53-400">Int64</span><span class="sxs-lookup"><span data-stu-id="2ee53-400">Int64</span></span>|<span data-ttu-id="2ee53-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="2ee53-401">Total Storage in Bytes.</span></span> <span data-ttu-id="2ee53-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-402">This property is read-only.</span></span> <span data-ttu-id="2ee53-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="2ee53-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="2ee53-405">Int64</span><span class="sxs-lookup"><span data-stu-id="2ee53-405">Int64</span></span>|<span data-ttu-id="2ee53-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="2ee53-406">Free Storage in Bytes.</span></span> <span data-ttu-id="2ee53-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-407">This property is read-only.</span></span> <span data-ttu-id="2ee53-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="2ee53-409">managedDeviceName</span></span>|<span data-ttu-id="2ee53-410">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-410">String</span></span>|<span data-ttu-id="2ee53-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="2ee53-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="2ee53-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="2ee53-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="2ee53-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="2ee53-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="2ee53-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="2ee53-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="2ee53-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-417">Read Only.</span></span> <span data-ttu-id="2ee53-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-418">This property is read-only.</span></span> <span data-ttu-id="2ee53-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="2ee53-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-421">retireAfterDateTime</span></span>|<span data-ttu-id="2ee53-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-422">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="2ee53-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="2ee53-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-424">This property is read-only.</span></span> <span data-ttu-id="2ee53-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="2ee53-426">usersLoggedOn</span></span>|<span data-ttu-id="2ee53-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="2ee53-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="2ee53-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-429">This property is read-only.</span></span> <span data-ttu-id="2ee53-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ee53-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="2ee53-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-432">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="2ee53-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="2ee53-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="2ee53-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="2ee53-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-435">Read Only.</span></span> <span data-ttu-id="2ee53-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-436">This property is read-only.</span></span> <span data-ttu-id="2ee53-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="2ee53-438">autopilotEnrolled</span></span>|<span data-ttu-id="2ee53-439">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee53-439">Boolean</span></span>|<span data-ttu-id="2ee53-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="2ee53-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="2ee53-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-441">This property is read-only.</span></span> <span data-ttu-id="2ee53-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="2ee53-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="2ee53-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee53-444">Boolean</span></span>|<span data-ttu-id="2ee53-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ee53-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="2ee53-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-446">This property is read-only.</span></span> <span data-ttu-id="2ee53-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="2ee53-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="2ee53-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ee53-449">DateTimeOffset</span></span>|<span data-ttu-id="2ee53-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2ee53-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="2ee53-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-451">This property is read-only.</span></span> <span data-ttu-id="2ee53-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-453">iccid</span><span class="sxs-lookup"><span data-stu-id="2ee53-453">iccid</span></span>|<span data-ttu-id="2ee53-454">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-454">String</span></span>|<span data-ttu-id="2ee53-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="2ee53-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="2ee53-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-456">This property is read-only.</span></span> <span data-ttu-id="2ee53-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-458">udid</span><span class="sxs-lookup"><span data-stu-id="2ee53-458">udid</span></span>|<span data-ttu-id="2ee53-459">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-459">String</span></span>|<span data-ttu-id="2ee53-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="2ee53-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="2ee53-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-461">This property is read-only.</span></span> <span data-ttu-id="2ee53-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ee53-463">roleScopeTagIds</span></span>|<span data-ttu-id="2ee53-464">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee53-464">String collection</span></span>|<span data-ttu-id="2ee53-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ee53-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="2ee53-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="2ee53-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="2ee53-468">Int32</span><span class="sxs-lookup"><span data-stu-id="2ee53-468">Int32</span></span>|<span data-ttu-id="2ee53-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="2ee53-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="2ee53-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-470">This property is read-only.</span></span> <span data-ttu-id="2ee53-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="2ee53-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="2ee53-473">Int32</span><span class="sxs-lookup"><span data-stu-id="2ee53-473">Int32</span></span>|<span data-ttu-id="2ee53-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="2ee53-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="2ee53-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-475">This property is read-only.</span></span> <span data-ttu-id="2ee53-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-477">notes</span><span class="sxs-lookup"><span data-stu-id="2ee53-477">notes</span></span>|<span data-ttu-id="2ee53-478">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-478">String</span></span>|<span data-ttu-id="2ee53-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="2ee53-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="2ee53-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="2ee53-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="2ee53-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="2ee53-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="2ee53-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="2ee53-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="2ee53-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="2ee53-486">ethernetMacAddress</span></span>|<span data-ttu-id="2ee53-487">String</span><span class="sxs-lookup"><span data-stu-id="2ee53-487">String</span></span>|<span data-ttu-id="2ee53-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="2ee53-488">Ethernet MAC.</span></span> <span data-ttu-id="2ee53-489">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-489">This property is read-only.</span></span> <span data-ttu-id="2ee53-490">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-491">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="2ee53-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="2ee53-492">Int64</span><span class="sxs-lookup"><span data-stu-id="2ee53-492">Int64</span></span>|<span data-ttu-id="2ee53-493">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="2ee53-493">Total Memory in Bytes.</span></span> <span data-ttu-id="2ee53-494">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-494">This property is read-only.</span></span> <span data-ttu-id="2ee53-495">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ee53-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="2ee53-496">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="2ee53-496">processorArchitecture</span></span>|[<span data-ttu-id="2ee53-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="2ee53-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="2ee53-498">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="2ee53-498">Processor architecture.</span></span> <span data-ttu-id="2ee53-499">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ee53-499">This property is read-only.</span></span> <span data-ttu-id="2ee53-500">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="2ee53-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="2ee53-501">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="2ee53-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="2ee53-502">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee53-502">Response</span></span>
<span data-ttu-id="2ee53-503">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ee53-503">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ee53-504">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ee53-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ee53-505">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ee53-505">Request</span></span>
<span data-ttu-id="2ee53-506">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ee53-506">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7641

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

### <a name="response"></a><span data-ttu-id="2ee53-507">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee53-507">Response</span></span>
<span data-ttu-id="2ee53-p171">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ee53-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7690

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





