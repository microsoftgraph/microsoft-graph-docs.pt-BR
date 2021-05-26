---
title: Atualizar windowsManagedDevice
description: Atualize as propriedades de um objeto windowsManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42e985f6563e68f6530ae2feb89777af4533a7c6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662953"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="3e683-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="3e683-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="3e683-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e683-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e683-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e683-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e683-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e683-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e683-107">Atualize as propriedades de um [objeto windowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e683-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e683-108">Prerequisites</span></span>
<span data-ttu-id="3e683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e683-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e683-111">Permission type</span></span>|<span data-ttu-id="3e683-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e683-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e683-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e683-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e683-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e683-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3e683-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e683-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e683-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e683-116">Not supported.</span></span>|
|<span data-ttu-id="3e683-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e683-117">Application</span></span>|<span data-ttu-id="3e683-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e683-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e683-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e683-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3e683-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e683-120">Request headers</span></span>
|<span data-ttu-id="3e683-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e683-121">Header</span></span>|<span data-ttu-id="3e683-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3e683-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e683-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e683-123">Authorization</span></span>|<span data-ttu-id="3e683-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e683-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e683-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e683-125">Accept</span></span>|<span data-ttu-id="3e683-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e683-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e683-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e683-127">Request body</span></span>
<span data-ttu-id="3e683-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="3e683-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="3e683-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e683-130">Property</span></span>|<span data-ttu-id="3e683-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e683-131">Type</span></span>|<span data-ttu-id="3e683-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e683-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e683-133">id</span><span class="sxs-lookup"><span data-stu-id="3e683-133">id</span></span>|<span data-ttu-id="3e683-134">String</span><span class="sxs-lookup"><span data-stu-id="3e683-134">String</span></span>|<span data-ttu-id="3e683-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-135">Unique Identifier for the device.</span></span> <span data-ttu-id="3e683-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-136">This property is read-only.</span></span> <span data-ttu-id="3e683-137">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-138">userId</span><span class="sxs-lookup"><span data-stu-id="3e683-138">userId</span></span>|<span data-ttu-id="3e683-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e683-139">String</span></span>|<span data-ttu-id="3e683-140">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="3e683-141">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-141">This property is read-only.</span></span> <span data-ttu-id="3e683-142">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="3e683-143">deviceName</span></span>|<span data-ttu-id="3e683-144">String</span><span class="sxs-lookup"><span data-stu-id="3e683-144">String</span></span>|<span data-ttu-id="3e683-145">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-145">Name of the device.</span></span> <span data-ttu-id="3e683-146">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-146">This property is read-only.</span></span> <span data-ttu-id="3e683-147">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="3e683-148">hardwareInformation</span></span>|[<span data-ttu-id="3e683-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="3e683-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="3e683-150">Os detalhes rígidos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-150">The hardward details for the device.</span></span>  <span data-ttu-id="3e683-151">Inclui informações como espaço de armazenamento, fabricante, número de série etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="3e683-152">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="3e683-153">ownerType</span></span>|[<span data-ttu-id="3e683-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="3e683-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="3e683-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-155">Ownership of the device.</span></span> <span data-ttu-id="3e683-156">Pode ser 'empresa' ou 'pessoal' Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="3e683-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="3e683-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3e683-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="3e683-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3e683-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="3e683-160">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-160">Ownership of the device.</span></span> <span data-ttu-id="3e683-161">Pode ser 'empresa' ou 'pessoal' Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-162">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="3e683-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="3e683-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="3e683-163">deviceActionResults</span></span>|<span data-ttu-id="3e683-164">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="3e683-165">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="3e683-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="3e683-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-166">This property is read-only.</span></span> <span data-ttu-id="3e683-167">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-168">managementState</span><span class="sxs-lookup"><span data-stu-id="3e683-168">managementState</span></span>|[<span data-ttu-id="3e683-169">managementState</span><span class="sxs-lookup"><span data-stu-id="3e683-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="3e683-170">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-170">Management state of the device.</span></span> <span data-ttu-id="3e683-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-171">This property is read-only.</span></span> <span data-ttu-id="3e683-172">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-173">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="3e683-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="3e683-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-174">enrolledDateTime</span></span>|<span data-ttu-id="3e683-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-175">DateTimeOffset</span></span>|<span data-ttu-id="3e683-176">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-176">Enrollment time of the device.</span></span> <span data-ttu-id="3e683-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-177">This property is read-only.</span></span> <span data-ttu-id="3e683-178">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-179">lastSyncDateTime</span></span>|<span data-ttu-id="3e683-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-180">DateTimeOffset</span></span>|<span data-ttu-id="3e683-181">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="3e683-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="3e683-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-182">This property is read-only.</span></span> <span data-ttu-id="3e683-183">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="3e683-184">chassisType</span></span>|[<span data-ttu-id="3e683-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="3e683-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="3e683-186">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-186">Chassis type of the device.</span></span> <span data-ttu-id="3e683-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-187">This property is read-only.</span></span> <span data-ttu-id="3e683-188">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-189">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="3e683-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="3e683-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3e683-190">operatingSystem</span></span>|<span data-ttu-id="3e683-191">String</span><span class="sxs-lookup"><span data-stu-id="3e683-191">String</span></span>|<span data-ttu-id="3e683-192">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-192">Operating system of the device.</span></span> <span data-ttu-id="3e683-193">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="3e683-194">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="3e683-195">deviceType</span></span>|[<span data-ttu-id="3e683-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="3e683-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="3e683-197">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-197">Platform of the device.</span></span> <span data-ttu-id="3e683-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-198">This property is read-only.</span></span> <span data-ttu-id="3e683-199">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-200">Os valores possíveis são: `desktop` , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="3e683-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="3e683-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="3e683-201">complianceState</span></span>|[<span data-ttu-id="3e683-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="3e683-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="3e683-203">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-203">Compliance state of the device.</span></span> <span data-ttu-id="3e683-204">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-204">This property is read-only.</span></span> <span data-ttu-id="3e683-205">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-206">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="3e683-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="3e683-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="3e683-207">jailBroken</span></span>|<span data-ttu-id="3e683-208">String</span><span class="sxs-lookup"><span data-stu-id="3e683-208">String</span></span>|<span data-ttu-id="3e683-209">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="3e683-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="3e683-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-210">This property is read-only.</span></span> <span data-ttu-id="3e683-211">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="3e683-212">managementAgent</span></span>|[<span data-ttu-id="3e683-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="3e683-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="3e683-214">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-214">Management channel of the device.</span></span> <span data-ttu-id="3e683-215">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="3e683-216">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-217">Os valores possíveis são: `eas` , , , , , , , , , `mdm` , , `easMdm` , , , `intuneClient` , `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown` `jamf` `googleCloudDevicePolicyController` `microsoft365ManagedMdm` `msSense` `intuneAosp` .</span><span class="sxs-lookup"><span data-stu-id="3e683-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`, `intuneAosp`.</span></span>|
|<span data-ttu-id="3e683-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="3e683-218">osVersion</span></span>|<span data-ttu-id="3e683-219">String</span><span class="sxs-lookup"><span data-stu-id="3e683-219">String</span></span>|<span data-ttu-id="3e683-220">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-220">Operating system version of the device.</span></span> <span data-ttu-id="3e683-221">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-221">This property is read-only.</span></span> <span data-ttu-id="3e683-222">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="3e683-223">easActivated</span></span>|<span data-ttu-id="3e683-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e683-224">Boolean</span></span>|<span data-ttu-id="3e683-225">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3e683-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="3e683-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-226">This property is read-only.</span></span> <span data-ttu-id="3e683-227">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="3e683-228">easDeviceId</span></span>|<span data-ttu-id="3e683-229">String</span><span class="sxs-lookup"><span data-stu-id="3e683-229">String</span></span>|<span data-ttu-id="3e683-230">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="3e683-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-231">This property is read-only.</span></span> <span data-ttu-id="3e683-232">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-233">easActivationDateTime</span></span>|<span data-ttu-id="3e683-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-234">DateTimeOffset</span></span>|<span data-ttu-id="3e683-235">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="3e683-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-236">This property is read-only.</span></span> <span data-ttu-id="3e683-237">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="3e683-238">aadRegistered</span></span>|<span data-ttu-id="3e683-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e683-239">Boolean</span></span>|<span data-ttu-id="3e683-240">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3e683-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="3e683-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-241">This property is read-only.</span></span> <span data-ttu-id="3e683-242">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="3e683-243">azureADRegistered</span></span>|<span data-ttu-id="3e683-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e683-244">Boolean</span></span>|<span data-ttu-id="3e683-245">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3e683-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="3e683-246">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-246">This property is read-only.</span></span> <span data-ttu-id="3e683-247">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3e683-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="3e683-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3e683-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="3e683-250">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-250">Enrollment type of the device.</span></span> <span data-ttu-id="3e683-251">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-251">This property is read-only.</span></span> <span data-ttu-id="3e683-252">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-253">Os valores possíveis são: `unknown` , , , , , , , , `userEnrollment` , , , `deviceEnrollmentManager` , , `appleBulkWithUser` , , , `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` , `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` .</span><span class="sxs-lookup"><span data-stu-id="3e683-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="3e683-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="3e683-254">lostModeState</span></span>|[<span data-ttu-id="3e683-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="3e683-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="3e683-256">Indica se o modo Perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="3e683-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="3e683-257">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-257">This property is read-only.</span></span> <span data-ttu-id="3e683-258">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-259">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="3e683-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="3e683-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="3e683-260">activationLockBypassCode</span></span>|<span data-ttu-id="3e683-261">String</span><span class="sxs-lookup"><span data-stu-id="3e683-261">String</span></span>|<span data-ttu-id="3e683-262">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="3e683-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="3e683-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-263">This property is read-only.</span></span> <span data-ttu-id="3e683-264">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3e683-265">emailAddress</span></span>|<span data-ttu-id="3e683-266">String</span><span class="sxs-lookup"><span data-stu-id="3e683-266">String</span></span>|<span data-ttu-id="3e683-267">Email(s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="3e683-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-268">This property is read-only.</span></span> <span data-ttu-id="3e683-269">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="3e683-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="3e683-271">String</span><span class="sxs-lookup"><span data-stu-id="3e683-271">String</span></span>|<span data-ttu-id="3e683-272">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3e683-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3e683-273">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-273">Read only.</span></span> <span data-ttu-id="3e683-274">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-274">This property is read-only.</span></span> <span data-ttu-id="3e683-275">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="3e683-276">azureADDeviceId</span></span>|<span data-ttu-id="3e683-277">String</span><span class="sxs-lookup"><span data-stu-id="3e683-277">String</span></span>|<span data-ttu-id="3e683-278">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3e683-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3e683-279">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-279">Read only.</span></span> <span data-ttu-id="3e683-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-280">This property is read-only.</span></span> <span data-ttu-id="3e683-281">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3e683-282">deviceRegistrationState</span></span>|[<span data-ttu-id="3e683-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3e683-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="3e683-284">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-284">Device registration state.</span></span> <span data-ttu-id="3e683-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-285">This property is read-only.</span></span> <span data-ttu-id="3e683-286">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-287">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3e683-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="3e683-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e683-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="3e683-289">String</span><span class="sxs-lookup"><span data-stu-id="3e683-289">String</span></span>|<span data-ttu-id="3e683-290">Nome de exibição de categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-290">Device category display name.</span></span> <span data-ttu-id="3e683-291">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-291">This property is read-only.</span></span> <span data-ttu-id="3e683-292">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="3e683-293">isSupervised</span></span>|<span data-ttu-id="3e683-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e683-294">Boolean</span></span>|<span data-ttu-id="3e683-295">Status supervisionado pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-295">Device supervised status.</span></span> <span data-ttu-id="3e683-296">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-296">This property is read-only.</span></span> <span data-ttu-id="3e683-297">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3e683-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-299">DateTimeOffset</span></span>|<span data-ttu-id="3e683-300">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e683-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="3e683-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-301">This property is read-only.</span></span> <span data-ttu-id="3e683-302">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3e683-303">exchangeAccessState</span></span>|[<span data-ttu-id="3e683-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3e683-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="3e683-305">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e683-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="3e683-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-306">This property is read-only.</span></span> <span data-ttu-id="3e683-307">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-308">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="3e683-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="3e683-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3e683-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="3e683-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3e683-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="3e683-311">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e683-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="3e683-312">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-312">This property is read-only.</span></span> <span data-ttu-id="3e683-313">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-314">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="3e683-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="3e683-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="3e683-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="3e683-316">String</span><span class="sxs-lookup"><span data-stu-id="3e683-316">String</span></span>|<span data-ttu-id="3e683-317">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="3e683-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-318">This property is read-only.</span></span> <span data-ttu-id="3e683-319">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3e683-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="3e683-321">String</span><span class="sxs-lookup"><span data-stu-id="3e683-321">String</span></span>|<span data-ttu-id="3e683-322">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="3e683-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="3e683-323">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-323">This property is read-only.</span></span> <span data-ttu-id="3e683-324">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="3e683-325">isEncrypted</span></span>|<span data-ttu-id="3e683-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e683-326">Boolean</span></span>|<span data-ttu-id="3e683-327">Status da criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-327">Device encryption status.</span></span> <span data-ttu-id="3e683-328">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-328">This property is read-only.</span></span> <span data-ttu-id="3e683-329">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3e683-330">userPrincipalName</span></span>|<span data-ttu-id="3e683-331">String</span><span class="sxs-lookup"><span data-stu-id="3e683-331">String</span></span>|<span data-ttu-id="3e683-332">Nome principal do usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-332">Device user principal name.</span></span> <span data-ttu-id="3e683-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-333">This property is read-only.</span></span> <span data-ttu-id="3e683-334">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-335">modelo</span><span class="sxs-lookup"><span data-stu-id="3e683-335">model</span></span>|<span data-ttu-id="3e683-336">String</span><span class="sxs-lookup"><span data-stu-id="3e683-336">String</span></span>|<span data-ttu-id="3e683-337">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-337">Model of the device.</span></span> <span data-ttu-id="3e683-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-338">This property is read-only.</span></span> <span data-ttu-id="3e683-339">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-340">fabricante</span><span class="sxs-lookup"><span data-stu-id="3e683-340">manufacturer</span></span>|<span data-ttu-id="3e683-341">String</span><span class="sxs-lookup"><span data-stu-id="3e683-341">String</span></span>|<span data-ttu-id="3e683-342">Fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-342">Manufacturer of the device.</span></span> <span data-ttu-id="3e683-343">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-343">This property is read-only.</span></span> <span data-ttu-id="3e683-344">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-345">imei</span><span class="sxs-lookup"><span data-stu-id="3e683-345">imei</span></span>|<span data-ttu-id="3e683-346">String</span><span class="sxs-lookup"><span data-stu-id="3e683-346">String</span></span>|<span data-ttu-id="3e683-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="3e683-347">IMEI.</span></span> <span data-ttu-id="3e683-348">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-348">This property is read-only.</span></span> <span data-ttu-id="3e683-349">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3e683-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-351">DateTimeOffset</span></span>|<span data-ttu-id="3e683-352">DateTime quando o período de carência de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="3e683-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="3e683-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-353">This property is read-only.</span></span> <span data-ttu-id="3e683-354">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="3e683-355">serialNumber</span></span>|<span data-ttu-id="3e683-356">String</span><span class="sxs-lookup"><span data-stu-id="3e683-356">String</span></span>|<span data-ttu-id="3e683-357">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="3e683-357">SerialNumber.</span></span> <span data-ttu-id="3e683-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-358">This property is read-only.</span></span> <span data-ttu-id="3e683-359">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3e683-360">phoneNumber</span></span>|<span data-ttu-id="3e683-361">String</span><span class="sxs-lookup"><span data-stu-id="3e683-361">String</span></span>|<span data-ttu-id="3e683-362">Telefone número do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-362">Phone number of the device.</span></span> <span data-ttu-id="3e683-363">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-363">This property is read-only.</span></span> <span data-ttu-id="3e683-364">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3e683-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="3e683-366">String</span><span class="sxs-lookup"><span data-stu-id="3e683-366">String</span></span>|<span data-ttu-id="3e683-367">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="3e683-367">Android security patch level.</span></span> <span data-ttu-id="3e683-368">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-368">This property is read-only.</span></span> <span data-ttu-id="3e683-369">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e683-370">userDisplayName</span></span>|<span data-ttu-id="3e683-371">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e683-371">String</span></span>|<span data-ttu-id="3e683-372">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="3e683-372">User display name.</span></span> <span data-ttu-id="3e683-373">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-373">This property is read-only.</span></span> <span data-ttu-id="3e683-374">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3e683-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="3e683-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3e683-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="3e683-377">Recursos habilitados para cliente ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="3e683-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="3e683-378">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-378">This property is read-only.</span></span> <span data-ttu-id="3e683-379">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="3e683-380">wiFiMacAddress</span></span>|<span data-ttu-id="3e683-381">String</span><span class="sxs-lookup"><span data-stu-id="3e683-381">String</span></span>|<span data-ttu-id="3e683-382">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="3e683-382">Wi-Fi MAC.</span></span> <span data-ttu-id="3e683-383">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-383">This property is read-only.</span></span> <span data-ttu-id="3e683-384">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3e683-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="3e683-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3e683-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="3e683-387">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-387">The device health attestation state.</span></span> <span data-ttu-id="3e683-388">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-388">This property is read-only.</span></span> <span data-ttu-id="3e683-389">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="3e683-390">subscriberCarrier</span></span>|<span data-ttu-id="3e683-391">String</span><span class="sxs-lookup"><span data-stu-id="3e683-391">String</span></span>|<span data-ttu-id="3e683-392">Operadora de Assinantes.</span><span class="sxs-lookup"><span data-stu-id="3e683-392">Subscriber Carrier.</span></span> <span data-ttu-id="3e683-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-393">This property is read-only.</span></span> <span data-ttu-id="3e683-394">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-395">meid</span><span class="sxs-lookup"><span data-stu-id="3e683-395">meid</span></span>|<span data-ttu-id="3e683-396">String</span><span class="sxs-lookup"><span data-stu-id="3e683-396">String</span></span>|<span data-ttu-id="3e683-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="3e683-397">MEID.</span></span> <span data-ttu-id="3e683-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-398">This property is read-only.</span></span> <span data-ttu-id="3e683-399">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3e683-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="3e683-401">Int64</span><span class="sxs-lookup"><span data-stu-id="3e683-401">Int64</span></span>|<span data-ttu-id="3e683-402">Total Armazenamento em Bytes.</span><span class="sxs-lookup"><span data-stu-id="3e683-402">Total Storage in Bytes.</span></span> <span data-ttu-id="3e683-403">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-403">This property is read-only.</span></span> <span data-ttu-id="3e683-404">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3e683-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="3e683-406">Int64</span><span class="sxs-lookup"><span data-stu-id="3e683-406">Int64</span></span>|<span data-ttu-id="3e683-407">Free Armazenamento em Bytes.</span><span class="sxs-lookup"><span data-stu-id="3e683-407">Free Storage in Bytes.</span></span> <span data-ttu-id="3e683-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-408">This property is read-only.</span></span> <span data-ttu-id="3e683-409">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="3e683-410">managedDeviceName</span></span>|<span data-ttu-id="3e683-411">String</span><span class="sxs-lookup"><span data-stu-id="3e683-411">String</span></span>|<span data-ttu-id="3e683-412">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="3e683-413">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3e683-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="3e683-414">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="3e683-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="3e683-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="3e683-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="3e683-417">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="3e683-418">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-418">Read Only.</span></span> <span data-ttu-id="3e683-419">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-419">This property is read-only.</span></span> <span data-ttu-id="3e683-420">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-421">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="3e683-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="3e683-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-422">retireAfterDateTime</span></span>|<span data-ttu-id="3e683-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-423">DateTimeOffset</span></span>|<span data-ttu-id="3e683-424">Indica a hora após a resuspensão automática de um dispositivo devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="3e683-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="3e683-425">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-425">This property is read-only.</span></span> <span data-ttu-id="3e683-426">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="3e683-427">usersLoggedOn</span></span>|<span data-ttu-id="3e683-428">[coleção loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="3e683-429">Indica o último usuário conectado a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="3e683-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-430">This property is read-only.</span></span> <span data-ttu-id="3e683-431">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e683-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="3e683-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-433">DateTimeOffset</span></span>|<span data-ttu-id="3e683-434">Relata que DateTime a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="3e683-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="3e683-435">Quando definidas, as configurações do MDM do Intune substituirão as configurações da Política de Grupo se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="3e683-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="3e683-436">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-436">Read Only.</span></span> <span data-ttu-id="3e683-437">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-437">This property is read-only.</span></span> <span data-ttu-id="3e683-438">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="3e683-439">autopilotEnrolled</span></span>|<span data-ttu-id="3e683-440">Booleano</span><span class="sxs-lookup"><span data-stu-id="3e683-440">Boolean</span></span>|<span data-ttu-id="3e683-441">Relata se o dispositivo gerenciado está inscrito por meio de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="3e683-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="3e683-442">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-442">This property is read-only.</span></span> <span data-ttu-id="3e683-443">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="3e683-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="3e683-445">Booleano</span><span class="sxs-lookup"><span data-stu-id="3e683-445">Boolean</span></span>|<span data-ttu-id="3e683-446">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="3e683-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="3e683-447">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-447">This property is read-only.</span></span> <span data-ttu-id="3e683-448">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="3e683-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="3e683-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e683-450">DateTimeOffset</span></span>|<span data-ttu-id="3e683-451">Relata a data de expiração do certificado de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="3e683-452">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-452">This property is read-only.</span></span> <span data-ttu-id="3e683-453">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-454">iccid</span><span class="sxs-lookup"><span data-stu-id="3e683-454">iccid</span></span>|<span data-ttu-id="3e683-455">String</span><span class="sxs-lookup"><span data-stu-id="3e683-455">String</span></span>|<span data-ttu-id="3e683-456">Identificador integrado de cartão de circuito, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="3e683-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="3e683-457">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-457">This property is read-only.</span></span> <span data-ttu-id="3e683-458">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-459">udid</span><span class="sxs-lookup"><span data-stu-id="3e683-459">udid</span></span>|<span data-ttu-id="3e683-460">String</span><span class="sxs-lookup"><span data-stu-id="3e683-460">String</span></span>|<span data-ttu-id="3e683-461">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="3e683-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="3e683-462">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-462">This property is read-only.</span></span> <span data-ttu-id="3e683-463">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e683-464">roleScopeTagIds</span></span>|<span data-ttu-id="3e683-465">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e683-465">String collection</span></span>|<span data-ttu-id="3e683-466">Lista de IDs de marca de escopo para esta instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e683-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="3e683-467">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="3e683-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="3e683-469">Int32</span><span class="sxs-lookup"><span data-stu-id="3e683-469">Int32</span></span>|<span data-ttu-id="3e683-470">Contagem de malware ativo para este dispositivo windows.</span><span class="sxs-lookup"><span data-stu-id="3e683-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="3e683-471">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-471">This property is read-only.</span></span> <span data-ttu-id="3e683-472">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="3e683-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="3e683-474">Int32</span><span class="sxs-lookup"><span data-stu-id="3e683-474">Int32</span></span>|<span data-ttu-id="3e683-475">Contagem de malwares remediados para este dispositivo windows.</span><span class="sxs-lookup"><span data-stu-id="3e683-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="3e683-476">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-476">This property is read-only.</span></span> <span data-ttu-id="3e683-477">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-478">notes</span><span class="sxs-lookup"><span data-stu-id="3e683-478">notes</span></span>|<span data-ttu-id="3e683-479">String</span><span class="sxs-lookup"><span data-stu-id="3e683-479">String</span></span>|<span data-ttu-id="3e683-480">Observações sobre o dispositivo criado pelo administrador de IT Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="3e683-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="3e683-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="3e683-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="3e683-483">Estado de saúde do cliente do gerenciador de configuração, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="3e683-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="3e683-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="3e683-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="3e683-486">Informações do cliente do Gerenciador de Configurações, válidas apenas para dispositivos gerenciados, gerenciados pelo duelo ou gerenciados pelo Agente ConfigMgr Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="3e683-487">ethernetMacAddress</span></span>|<span data-ttu-id="3e683-488">String</span><span class="sxs-lookup"><span data-stu-id="3e683-488">String</span></span>|<span data-ttu-id="3e683-489">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="3e683-489">Ethernet MAC.</span></span> <span data-ttu-id="3e683-490">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-490">This property is read-only.</span></span> <span data-ttu-id="3e683-491">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="3e683-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="3e683-493">Int64</span><span class="sxs-lookup"><span data-stu-id="3e683-493">Int64</span></span>|<span data-ttu-id="3e683-494">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="3e683-494">Total Memory in Bytes.</span></span> <span data-ttu-id="3e683-495">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-495">This property is read-only.</span></span> <span data-ttu-id="3e683-496">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="3e683-497">processorArchitecture</span></span>|[<span data-ttu-id="3e683-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="3e683-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="3e683-499">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="3e683-499">Processor architecture.</span></span> <span data-ttu-id="3e683-500">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-500">This property is read-only.</span></span> <span data-ttu-id="3e683-501">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-502">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="3e683-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="3e683-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="3e683-503">specificationVersion</span></span>|<span data-ttu-id="3e683-504">String</span><span class="sxs-lookup"><span data-stu-id="3e683-504">String</span></span>|<span data-ttu-id="3e683-505">Versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="3e683-505">Specification version.</span></span> <span data-ttu-id="3e683-506">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-506">This property is read-only.</span></span> <span data-ttu-id="3e683-507">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-508">joinType</span><span class="sxs-lookup"><span data-stu-id="3e683-508">joinType</span></span>|[<span data-ttu-id="3e683-509">joinType</span><span class="sxs-lookup"><span data-stu-id="3e683-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="3e683-510">Tipo de junção de dispositivo Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-511">Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="3e683-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="3e683-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="3e683-512">skuFamily</span></span>|<span data-ttu-id="3e683-513">String</span><span class="sxs-lookup"><span data-stu-id="3e683-513">String</span></span>|<span data-ttu-id="3e683-514">Família sku de dispositivo Herdada [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="3e683-515">skuNumber</span></span>|<span data-ttu-id="3e683-516">Int32</span><span class="sxs-lookup"><span data-stu-id="3e683-516">Int32</span></span>|<span data-ttu-id="3e683-517">Número sku do dispositivo, consulte também: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="3e683-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="3e683-518">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="3e683-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="3e683-519">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e683-519">This property is read-only.</span></span> <span data-ttu-id="3e683-520">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="3e683-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="3e683-521">managementFeatures</span></span>|[<span data-ttu-id="3e683-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="3e683-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="3e683-523">Recursos de gerenciamento de dispositivo Herdados [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3e683-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="3e683-524">Os valores possíveis são: `none` e `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="3e683-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|
|<span data-ttu-id="3e683-525">chromeOSDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="3e683-525">chromeOSDeviceInfo</span></span>|<span data-ttu-id="3e683-526">[Coleção chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-526">[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) collection</span></span>|<span data-ttu-id="3e683-527">Lista de propriedades do Dispositivo ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="3e683-527">List of properties of the ChromeOS Device.</span></span> <span data-ttu-id="3e683-528">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3e683-528">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3e683-529">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e683-529">Response</span></span>
<span data-ttu-id="3e683-530">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e683-530">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e683-531">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e683-531">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e683-532">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e683-532">Request</span></span>
<span data-ttu-id="3e683-533">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e683-533">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 8564

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
    "subnetAddress": "Subnet Address value",
    "esimIdentifier": "Esim Identifier value",
    "systemManagementBIOSVersion": "System Management BIOSVersion value",
    "tpmManufacturer": "Tpm Manufacturer value",
    "tpmVersion": "Tpm Version value"
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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3e683-534">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e683-534">Response</span></span>
<span data-ttu-id="3e683-p176">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e683-p176">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8613

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
    "subnetAddress": "Subnet Address value",
    "esimIdentifier": "Esim Identifier value",
    "systemManagementBIOSVersion": "System Management BIOSVersion value",
    "tpmManufacturer": "Tpm Manufacturer value",
    "tpmVersion": "Tpm Version value"
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
  "managementFeatures": "microsoftManagedDesktop",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "Name value",
      "value": "Value value",
      "valueType": "Value Type value",
      "updatable": true
    }
  ]
}
```




