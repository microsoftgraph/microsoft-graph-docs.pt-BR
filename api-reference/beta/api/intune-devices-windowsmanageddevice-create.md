---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2dcdb96ea9e51bce5e44e7c5fa5837b6a63116d1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185620"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="de286-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="de286-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="de286-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de286-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de286-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de286-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="de286-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de286-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de286-107">Prerequisites</span></span>
<span data-ttu-id="de286-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de286-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de286-110">Permission type</span></span>|<span data-ttu-id="de286-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de286-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de286-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de286-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de286-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de286-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="de286-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de286-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de286-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de286-115">Not supported.</span></span>|
|<span data-ttu-id="de286-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de286-116">Application</span></span>|<span data-ttu-id="de286-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de286-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de286-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de286-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="de286-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de286-119">Request headers</span></span>
|<span data-ttu-id="de286-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de286-120">Header</span></span>|<span data-ttu-id="de286-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de286-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de286-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de286-122">Authorization</span></span>|<span data-ttu-id="de286-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de286-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de286-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de286-124">Accept</span></span>|<span data-ttu-id="de286-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de286-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de286-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de286-126">Request body</span></span>
<span data-ttu-id="de286-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="de286-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="de286-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="de286-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="de286-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de286-129">Property</span></span>|<span data-ttu-id="de286-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="de286-130">Type</span></span>|<span data-ttu-id="de286-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="de286-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de286-132">id</span><span class="sxs-lookup"><span data-stu-id="de286-132">id</span></span>|<span data-ttu-id="de286-133">String</span><span class="sxs-lookup"><span data-stu-id="de286-133">String</span></span>|<span data-ttu-id="de286-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-134">Unique Identifier for the device.</span></span> <span data-ttu-id="de286-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-135">This property is read-only.</span></span> <span data-ttu-id="de286-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-137">userId</span><span class="sxs-lookup"><span data-stu-id="de286-137">userId</span></span>|<span data-ttu-id="de286-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de286-138">String</span></span>|<span data-ttu-id="de286-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="de286-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-140">This property is read-only.</span></span> <span data-ttu-id="de286-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="de286-142">deviceName</span></span>|<span data-ttu-id="de286-143">String</span><span class="sxs-lookup"><span data-stu-id="de286-143">String</span></span>|<span data-ttu-id="de286-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-144">Name of the device.</span></span> <span data-ttu-id="de286-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-145">This property is read-only.</span></span> <span data-ttu-id="de286-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="de286-147">hardwareInformation</span></span>|[<span data-ttu-id="de286-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="de286-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="de286-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-149">The hardward details for the device.</span></span>  <span data-ttu-id="de286-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="de286-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="de286-152">ownerType</span></span>|[<span data-ttu-id="de286-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="de286-153">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="de286-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-154">Ownership of the device.</span></span> <span data-ttu-id="de286-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="de286-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="de286-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="de286-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="de286-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="de286-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="de286-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-159">Ownership of the device.</span></span> <span data-ttu-id="de286-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="de286-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="de286-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="de286-162">deviceActionResults</span></span>|<span data-ttu-id="de286-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="de286-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="de286-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="de286-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="de286-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-165">This property is read-only.</span></span> <span data-ttu-id="de286-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="de286-167">managementState</span></span>|[<span data-ttu-id="de286-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="de286-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="de286-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-169">Management state of the device.</span></span> <span data-ttu-id="de286-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-170">This property is read-only.</span></span> <span data-ttu-id="de286-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="de286-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="de286-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-173">enrolledDateTime</span></span>|<span data-ttu-id="de286-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-174">DateTimeOffset</span></span>|<span data-ttu-id="de286-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-175">Enrollment time of the device.</span></span> <span data-ttu-id="de286-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-176">This property is read-only.</span></span> <span data-ttu-id="de286-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-178">lastSyncDateTime</span></span>|<span data-ttu-id="de286-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-179">DateTimeOffset</span></span>|<span data-ttu-id="de286-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="de286-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="de286-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-181">This property is read-only.</span></span> <span data-ttu-id="de286-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="de286-183">chassisType</span></span>|[<span data-ttu-id="de286-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="de286-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="de286-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-185">Chassis type of the device.</span></span> <span data-ttu-id="de286-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-186">This property is read-only.</span></span> <span data-ttu-id="de286-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="de286-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="de286-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="de286-189">operatingSystem</span></span>|<span data-ttu-id="de286-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de286-190">String</span></span>|<span data-ttu-id="de286-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-191">Operating system of the device.</span></span> <span data-ttu-id="de286-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="de286-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="de286-194">deviceType</span></span>|[<span data-ttu-id="de286-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="de286-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="de286-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-196">Platform of the device.</span></span> <span data-ttu-id="de286-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-197">This property is read-only.</span></span> <span data-ttu-id="de286-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="de286-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="de286-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="de286-200">complianceState</span></span>|[<span data-ttu-id="de286-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="de286-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="de286-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-202">Compliance state of the device.</span></span> <span data-ttu-id="de286-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-203">This property is read-only.</span></span> <span data-ttu-id="de286-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="de286-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="de286-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="de286-206">jailBroken</span></span>|<span data-ttu-id="de286-207">String</span><span class="sxs-lookup"><span data-stu-id="de286-207">String</span></span>|<span data-ttu-id="de286-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="de286-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="de286-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-209">This property is read-only.</span></span> <span data-ttu-id="de286-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="de286-211">managementAgent</span></span>|[<span data-ttu-id="de286-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="de286-212">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="de286-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-213">Management channel of the device.</span></span> <span data-ttu-id="de286-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="de286-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="de286-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="de286-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="de286-217">osVersion</span></span>|<span data-ttu-id="de286-218">String</span><span class="sxs-lookup"><span data-stu-id="de286-218">String</span></span>|<span data-ttu-id="de286-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-219">Operating system version of the device.</span></span> <span data-ttu-id="de286-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-220">This property is read-only.</span></span> <span data-ttu-id="de286-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="de286-222">easActivated</span></span>|<span data-ttu-id="de286-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="de286-223">Boolean</span></span>|<span data-ttu-id="de286-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="de286-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="de286-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-225">This property is read-only.</span></span> <span data-ttu-id="de286-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="de286-227">easDeviceId</span></span>|<span data-ttu-id="de286-228">String</span><span class="sxs-lookup"><span data-stu-id="de286-228">String</span></span>|<span data-ttu-id="de286-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="de286-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-230">This property is read-only.</span></span> <span data-ttu-id="de286-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-232">easActivationDateTime</span></span>|<span data-ttu-id="de286-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-233">DateTimeOffset</span></span>|<span data-ttu-id="de286-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="de286-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-235">This property is read-only.</span></span> <span data-ttu-id="de286-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="de286-237">aadRegistered</span></span>|<span data-ttu-id="de286-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="de286-238">Boolean</span></span>|<span data-ttu-id="de286-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de286-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="de286-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-240">This property is read-only.</span></span> <span data-ttu-id="de286-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="de286-242">azureADRegistered</span></span>|<span data-ttu-id="de286-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="de286-243">Boolean</span></span>|<span data-ttu-id="de286-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de286-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="de286-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-245">This property is read-only.</span></span> <span data-ttu-id="de286-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="de286-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="de286-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="de286-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="de286-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-249">Enrollment type of the device.</span></span> <span data-ttu-id="de286-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-250">This property is read-only.</span></span> <span data-ttu-id="de286-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount` e `appleUserEnrollmentWithAzureAD`.</span><span class="sxs-lookup"><span data-stu-id="de286-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `appleUserEnrollmentWithAzureAD`.</span></span>|
|<span data-ttu-id="de286-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="de286-253">lostModeState</span></span>|[<span data-ttu-id="de286-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="de286-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="de286-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="de286-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="de286-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-256">This property is read-only.</span></span> <span data-ttu-id="de286-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="de286-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="de286-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="de286-259">activationLockBypassCode</span></span>|<span data-ttu-id="de286-260">String</span><span class="sxs-lookup"><span data-stu-id="de286-260">String</span></span>|<span data-ttu-id="de286-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="de286-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="de286-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-262">This property is read-only.</span></span> <span data-ttu-id="de286-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="de286-264">emailAddress</span></span>|<span data-ttu-id="de286-265">String</span><span class="sxs-lookup"><span data-stu-id="de286-265">String</span></span>|<span data-ttu-id="de286-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="de286-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-267">This property is read-only.</span></span> <span data-ttu-id="de286-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="de286-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="de286-270">String</span><span class="sxs-lookup"><span data-stu-id="de286-270">String</span></span>|<span data-ttu-id="de286-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de286-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="de286-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-272">Read only.</span></span> <span data-ttu-id="de286-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-273">This property is read-only.</span></span> <span data-ttu-id="de286-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="de286-275">azureADDeviceId</span></span>|<span data-ttu-id="de286-276">String</span><span class="sxs-lookup"><span data-stu-id="de286-276">String</span></span>|<span data-ttu-id="de286-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de286-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="de286-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-278">Read only.</span></span> <span data-ttu-id="de286-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-279">This property is read-only.</span></span> <span data-ttu-id="de286-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="de286-281">deviceRegistrationState</span></span>|[<span data-ttu-id="de286-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="de286-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="de286-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-283">Device registration state.</span></span> <span data-ttu-id="de286-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-284">This property is read-only.</span></span> <span data-ttu-id="de286-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="de286-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="de286-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="de286-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="de286-288">String</span><span class="sxs-lookup"><span data-stu-id="de286-288">String</span></span>|<span data-ttu-id="de286-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-289">Device category display name.</span></span> <span data-ttu-id="de286-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-290">This property is read-only.</span></span> <span data-ttu-id="de286-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="de286-292">isSupervised</span></span>|<span data-ttu-id="de286-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="de286-293">Boolean</span></span>|<span data-ttu-id="de286-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-294">Device supervised status.</span></span> <span data-ttu-id="de286-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-295">This property is read-only.</span></span> <span data-ttu-id="de286-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="de286-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-298">DateTimeOffset</span></span>|<span data-ttu-id="de286-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="de286-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="de286-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-300">This property is read-only.</span></span> <span data-ttu-id="de286-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="de286-302">exchangeAccessState</span></span>|[<span data-ttu-id="de286-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="de286-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="de286-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="de286-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="de286-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-305">This property is read-only.</span></span> <span data-ttu-id="de286-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="de286-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="de286-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="de286-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="de286-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="de286-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="de286-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="de286-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="de286-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-311">This property is read-only.</span></span> <span data-ttu-id="de286-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="de286-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="de286-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="de286-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="de286-315">String</span><span class="sxs-lookup"><span data-stu-id="de286-315">String</span></span>|<span data-ttu-id="de286-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="de286-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-317">This property is read-only.</span></span> <span data-ttu-id="de286-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="de286-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="de286-320">String</span><span class="sxs-lookup"><span data-stu-id="de286-320">String</span></span>|<span data-ttu-id="de286-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="de286-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="de286-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-322">This property is read-only.</span></span> <span data-ttu-id="de286-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="de286-324">isEncrypted</span></span>|<span data-ttu-id="de286-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="de286-325">Boolean</span></span>|<span data-ttu-id="de286-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-326">Device encryption status.</span></span> <span data-ttu-id="de286-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-327">This property is read-only.</span></span> <span data-ttu-id="de286-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de286-329">userPrincipalName</span></span>|<span data-ttu-id="de286-330">String</span><span class="sxs-lookup"><span data-stu-id="de286-330">String</span></span>|<span data-ttu-id="de286-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-331">Device user principal name.</span></span> <span data-ttu-id="de286-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-332">This property is read-only.</span></span> <span data-ttu-id="de286-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-334">modelo</span><span class="sxs-lookup"><span data-stu-id="de286-334">model</span></span>|<span data-ttu-id="de286-335">String</span><span class="sxs-lookup"><span data-stu-id="de286-335">String</span></span>|<span data-ttu-id="de286-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-336">Model of the device.</span></span> <span data-ttu-id="de286-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-337">This property is read-only.</span></span> <span data-ttu-id="de286-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="de286-339">manufacturer</span></span>|<span data-ttu-id="de286-340">String</span><span class="sxs-lookup"><span data-stu-id="de286-340">String</span></span>|<span data-ttu-id="de286-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-341">Manufacturer of the device.</span></span> <span data-ttu-id="de286-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-342">This property is read-only.</span></span> <span data-ttu-id="de286-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-344">imei</span><span class="sxs-lookup"><span data-stu-id="de286-344">imei</span></span>|<span data-ttu-id="de286-345">String</span><span class="sxs-lookup"><span data-stu-id="de286-345">String</span></span>|<span data-ttu-id="de286-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="de286-346">IMEI.</span></span> <span data-ttu-id="de286-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-347">This property is read-only.</span></span> <span data-ttu-id="de286-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="de286-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-350">DateTimeOffset</span></span>|<span data-ttu-id="de286-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="de286-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="de286-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-352">This property is read-only.</span></span> <span data-ttu-id="de286-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="de286-354">serialNumber</span></span>|<span data-ttu-id="de286-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de286-355">String</span></span>|<span data-ttu-id="de286-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="de286-356">SerialNumber.</span></span> <span data-ttu-id="de286-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-357">This property is read-only.</span></span> <span data-ttu-id="de286-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="de286-359">phoneNumber</span></span>|<span data-ttu-id="de286-360">String</span><span class="sxs-lookup"><span data-stu-id="de286-360">String</span></span>|<span data-ttu-id="de286-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-361">Phone number of the device.</span></span> <span data-ttu-id="de286-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-362">This property is read-only.</span></span> <span data-ttu-id="de286-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="de286-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="de286-365">String</span><span class="sxs-lookup"><span data-stu-id="de286-365">String</span></span>|<span data-ttu-id="de286-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="de286-366">Android security patch level.</span></span> <span data-ttu-id="de286-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-367">This property is read-only.</span></span> <span data-ttu-id="de286-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="de286-369">userDisplayName</span></span>|<span data-ttu-id="de286-370">String</span><span class="sxs-lookup"><span data-stu-id="de286-370">String</span></span>|<span data-ttu-id="de286-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="de286-371">User display name.</span></span> <span data-ttu-id="de286-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-372">This property is read-only.</span></span> <span data-ttu-id="de286-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="de286-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="de286-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="de286-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="de286-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="de286-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="de286-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-377">This property is read-only.</span></span> <span data-ttu-id="de286-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="de286-379">wiFiMacAddress</span></span>|<span data-ttu-id="de286-380">String</span><span class="sxs-lookup"><span data-stu-id="de286-380">String</span></span>|<span data-ttu-id="de286-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="de286-381">Wi-Fi MAC.</span></span> <span data-ttu-id="de286-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-382">This property is read-only.</span></span> <span data-ttu-id="de286-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="de286-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="de286-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="de286-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="de286-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-386">The device health attestation state.</span></span> <span data-ttu-id="de286-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-387">This property is read-only.</span></span> <span data-ttu-id="de286-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="de286-389">subscriberCarrier</span></span>|<span data-ttu-id="de286-390">String</span><span class="sxs-lookup"><span data-stu-id="de286-390">String</span></span>|<span data-ttu-id="de286-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="de286-391">Subscriber Carrier.</span></span> <span data-ttu-id="de286-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-392">This property is read-only.</span></span> <span data-ttu-id="de286-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-394">meid</span><span class="sxs-lookup"><span data-stu-id="de286-394">meid</span></span>|<span data-ttu-id="de286-395">String</span><span class="sxs-lookup"><span data-stu-id="de286-395">String</span></span>|<span data-ttu-id="de286-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="de286-396">MEID.</span></span> <span data-ttu-id="de286-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-397">This property is read-only.</span></span> <span data-ttu-id="de286-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="de286-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="de286-400">Int64</span><span class="sxs-lookup"><span data-stu-id="de286-400">Int64</span></span>|<span data-ttu-id="de286-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="de286-401">Total Storage in Bytes.</span></span> <span data-ttu-id="de286-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-402">This property is read-only.</span></span> <span data-ttu-id="de286-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="de286-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="de286-405">Int64</span><span class="sxs-lookup"><span data-stu-id="de286-405">Int64</span></span>|<span data-ttu-id="de286-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="de286-406">Free Storage in Bytes.</span></span> <span data-ttu-id="de286-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-407">This property is read-only.</span></span> <span data-ttu-id="de286-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="de286-409">managedDeviceName</span></span>|<span data-ttu-id="de286-410">String</span><span class="sxs-lookup"><span data-stu-id="de286-410">String</span></span>|<span data-ttu-id="de286-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="de286-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="de286-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="de286-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="de286-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="de286-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="de286-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="de286-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="de286-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-417">Read Only.</span></span> <span data-ttu-id="de286-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-418">This property is read-only.</span></span> <span data-ttu-id="de286-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="de286-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="de286-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="de286-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="de286-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-421">retireAfterDateTime</span></span>|<span data-ttu-id="de286-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-422">DateTimeOffset</span></span>|<span data-ttu-id="de286-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="de286-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="de286-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-424">This property is read-only.</span></span> <span data-ttu-id="de286-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="de286-426">usersLoggedOn</span></span>|<span data-ttu-id="de286-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="de286-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="de286-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="de286-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-429">This property is read-only.</span></span> <span data-ttu-id="de286-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="de286-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="de286-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-432">DateTimeOffset</span></span>|<span data-ttu-id="de286-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="de286-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="de286-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="de286-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="de286-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-435">Read Only.</span></span> <span data-ttu-id="de286-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-436">This property is read-only.</span></span> <span data-ttu-id="de286-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="de286-438">autopilotEnrolled</span></span>|<span data-ttu-id="de286-439">Booliano</span><span class="sxs-lookup"><span data-stu-id="de286-439">Boolean</span></span>|<span data-ttu-id="de286-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="de286-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="de286-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-441">This property is read-only.</span></span> <span data-ttu-id="de286-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="de286-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="de286-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="de286-444">Boolean</span></span>|<span data-ttu-id="de286-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="de286-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="de286-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-446">This property is read-only.</span></span> <span data-ttu-id="de286-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="de286-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="de286-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de286-449">DateTimeOffset</span></span>|<span data-ttu-id="de286-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="de286-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="de286-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-451">This property is read-only.</span></span> <span data-ttu-id="de286-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-453">iccid</span><span class="sxs-lookup"><span data-stu-id="de286-453">iccid</span></span>|<span data-ttu-id="de286-454">String</span><span class="sxs-lookup"><span data-stu-id="de286-454">String</span></span>|<span data-ttu-id="de286-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="de286-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="de286-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-456">This property is read-only.</span></span> <span data-ttu-id="de286-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-458">udid</span><span class="sxs-lookup"><span data-stu-id="de286-458">udid</span></span>|<span data-ttu-id="de286-459">String</span><span class="sxs-lookup"><span data-stu-id="de286-459">String</span></span>|<span data-ttu-id="de286-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="de286-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="de286-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-461">This property is read-only.</span></span> <span data-ttu-id="de286-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de286-463">roleScopeTagIds</span></span>|<span data-ttu-id="de286-464">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de286-464">String collection</span></span>|<span data-ttu-id="de286-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de286-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="de286-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="de286-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="de286-468">Int32</span><span class="sxs-lookup"><span data-stu-id="de286-468">Int32</span></span>|<span data-ttu-id="de286-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="de286-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="de286-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-470">This property is read-only.</span></span> <span data-ttu-id="de286-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="de286-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="de286-473">Int32</span><span class="sxs-lookup"><span data-stu-id="de286-473">Int32</span></span>|<span data-ttu-id="de286-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="de286-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="de286-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de286-475">This property is read-only.</span></span> <span data-ttu-id="de286-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-477">notes</span><span class="sxs-lookup"><span data-stu-id="de286-477">notes</span></span>|<span data-ttu-id="de286-478">String</span><span class="sxs-lookup"><span data-stu-id="de286-478">String</span></span>|<span data-ttu-id="de286-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="de286-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="de286-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="de286-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="de286-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="de286-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="de286-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="de286-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="de286-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="de286-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="de286-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="de286-486">Resposta</span><span class="sxs-lookup"><span data-stu-id="de286-486">Response</span></span>
<span data-ttu-id="de286-487">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de286-487">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de286-488">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de286-488">Example</span></span>

### <a name="request"></a><span data-ttu-id="de286-489">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de286-489">Request</span></span>
<span data-ttu-id="de286-490">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de286-490">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7520

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
  }
}
```

### <a name="response"></a><span data-ttu-id="de286-491">Resposta</span><span class="sxs-lookup"><span data-stu-id="de286-491">Response</span></span>
<span data-ttu-id="de286-p168">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de286-p168">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7569

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
  }
}
```




