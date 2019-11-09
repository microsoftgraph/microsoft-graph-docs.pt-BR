---
title: Atualizar windowsManagedDevice
description: Atualiza as propriedades de um objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 347589686718054f5dbd0c143ade0ecb66aef481
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087387"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="f9f28-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="f9f28-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="f9f28-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9f28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9f28-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9f28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9f28-106">Atualiza as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f9f28-106">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9f28-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9f28-107">Prerequisites</span></span>
<span data-ttu-id="f9f28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f28-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9f28-110">Permission type</span></span>|<span data-ttu-id="f9f28-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9f28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9f28-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9f28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9f28-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f28-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9f28-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9f28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9f28-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f28-115">Not supported.</span></span>|
|<span data-ttu-id="f9f28-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9f28-116">Application</span></span>|<span data-ttu-id="f9f28-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f28-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f28-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f28-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f9f28-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f28-119">Request headers</span></span>
|<span data-ttu-id="f9f28-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9f28-120">Header</span></span>|<span data-ttu-id="f9f28-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9f28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9f28-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9f28-122">Authorization</span></span>|<span data-ttu-id="f9f28-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9f28-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9f28-124">Accept</span></span>|<span data-ttu-id="f9f28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f28-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f28-126">Request body</span></span>
<span data-ttu-id="f9f28-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f9f28-127">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="f9f28-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-128">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="f9f28-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9f28-129">Property</span></span>|<span data-ttu-id="f9f28-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9f28-130">Type</span></span>|<span data-ttu-id="f9f28-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9f28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9f28-132">id</span><span class="sxs-lookup"><span data-stu-id="f9f28-132">id</span></span>|<span data-ttu-id="f9f28-133">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-133">String</span></span>|<span data-ttu-id="f9f28-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-134">Unique Identifier for the device.</span></span> <span data-ttu-id="f9f28-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-135">This property is read-only.</span></span> <span data-ttu-id="f9f28-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-137">userId</span><span class="sxs-lookup"><span data-stu-id="f9f28-137">userId</span></span>|<span data-ttu-id="f9f28-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9f28-138">String</span></span>|<span data-ttu-id="f9f28-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="f9f28-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-140">This property is read-only.</span></span> <span data-ttu-id="f9f28-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="f9f28-142">deviceName</span></span>|<span data-ttu-id="f9f28-143">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-143">String</span></span>|<span data-ttu-id="f9f28-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-144">Name of the device.</span></span> <span data-ttu-id="f9f28-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-145">This property is read-only.</span></span> <span data-ttu-id="f9f28-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f9f28-147">hardwareInformation</span></span>|[<span data-ttu-id="f9f28-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f9f28-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="f9f28-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-149">The hardward details for the device.</span></span>  <span data-ttu-id="f9f28-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="f9f28-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="f9f28-152">ownerType</span></span>|[<span data-ttu-id="f9f28-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="f9f28-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="f9f28-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-154">Ownership of the device.</span></span> <span data-ttu-id="f9f28-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f9f28-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f9f28-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="f9f28-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f9f28-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="f9f28-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-159">Ownership of the device.</span></span> <span data-ttu-id="f9f28-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f9f28-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="f9f28-162">deviceActionResults</span></span>|<span data-ttu-id="f9f28-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="f9f28-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="f9f28-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="f9f28-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-165">This property is read-only.</span></span> <span data-ttu-id="f9f28-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="f9f28-167">managementState</span></span>|[<span data-ttu-id="f9f28-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="f9f28-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="f9f28-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-169">Management state of the device.</span></span> <span data-ttu-id="f9f28-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-170">This property is read-only.</span></span> <span data-ttu-id="f9f28-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="f9f28-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-173">enrolledDateTime</span></span>|<span data-ttu-id="f9f28-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-174">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-175">Enrollment time of the device.</span></span> <span data-ttu-id="f9f28-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-176">This property is read-only.</span></span> <span data-ttu-id="f9f28-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-178">lastSyncDateTime</span></span>|<span data-ttu-id="f9f28-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-179">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="f9f28-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="f9f28-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-181">This property is read-only.</span></span> <span data-ttu-id="f9f28-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="f9f28-183">chassisType</span></span>|[<span data-ttu-id="f9f28-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="f9f28-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="f9f28-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-185">Chassis type of the device.</span></span> <span data-ttu-id="f9f28-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-186">This property is read-only.</span></span> <span data-ttu-id="f9f28-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="f9f28-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f9f28-189">operatingSystem</span></span>|<span data-ttu-id="f9f28-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9f28-190">String</span></span>|<span data-ttu-id="f9f28-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-191">Operating system of the device.</span></span> <span data-ttu-id="f9f28-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="f9f28-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="f9f28-194">deviceType</span></span>|[<span data-ttu-id="f9f28-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="f9f28-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f9f28-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-196">Platform of the device.</span></span> <span data-ttu-id="f9f28-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-197">This property is read-only.</span></span> <span data-ttu-id="f9f28-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="f9f28-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f9f28-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="f9f28-200">complianceState</span></span>|[<span data-ttu-id="f9f28-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="f9f28-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="f9f28-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-202">Compliance state of the device.</span></span> <span data-ttu-id="f9f28-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-203">This property is read-only.</span></span> <span data-ttu-id="f9f28-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="f9f28-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="f9f28-206">jailBroken</span></span>|<span data-ttu-id="f9f28-207">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-207">String</span></span>|<span data-ttu-id="f9f28-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="f9f28-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="f9f28-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-209">This property is read-only.</span></span> <span data-ttu-id="f9f28-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="f9f28-211">managementAgent</span></span>|[<span data-ttu-id="f9f28-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="f9f28-212">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="f9f28-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-213">Management channel of the device.</span></span> <span data-ttu-id="f9f28-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="f9f28-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="f9f28-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="f9f28-217">osVersion</span></span>|<span data-ttu-id="f9f28-218">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-218">String</span></span>|<span data-ttu-id="f9f28-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-219">Operating system version of the device.</span></span> <span data-ttu-id="f9f28-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-220">This property is read-only.</span></span> <span data-ttu-id="f9f28-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="f9f28-222">easActivated</span></span>|<span data-ttu-id="f9f28-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9f28-223">Boolean</span></span>|<span data-ttu-id="f9f28-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f9f28-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="f9f28-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-225">This property is read-only.</span></span> <span data-ttu-id="f9f28-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="f9f28-227">easDeviceId</span></span>|<span data-ttu-id="f9f28-228">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-228">String</span></span>|<span data-ttu-id="f9f28-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="f9f28-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-230">This property is read-only.</span></span> <span data-ttu-id="f9f28-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-232">easActivationDateTime</span></span>|<span data-ttu-id="f9f28-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-233">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="f9f28-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-235">This property is read-only.</span></span> <span data-ttu-id="f9f28-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="f9f28-237">aadRegistered</span></span>|<span data-ttu-id="f9f28-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f28-238">Boolean</span></span>|<span data-ttu-id="f9f28-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9f28-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="f9f28-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-240">This property is read-only.</span></span> <span data-ttu-id="f9f28-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="f9f28-242">azureADRegistered</span></span>|<span data-ttu-id="f9f28-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f28-243">Boolean</span></span>|<span data-ttu-id="f9f28-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9f28-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="f9f28-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-245">This property is read-only.</span></span> <span data-ttu-id="f9f28-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f9f28-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="f9f28-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f9f28-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f9f28-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-249">Enrollment type of the device.</span></span> <span data-ttu-id="f9f28-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-250">This property is read-only.</span></span> <span data-ttu-id="f9f28-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="f9f28-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f9f28-253">lostModeState</span></span>|[<span data-ttu-id="f9f28-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f9f28-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="f9f28-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f9f28-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="f9f28-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-256">This property is read-only.</span></span> <span data-ttu-id="f9f28-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f9f28-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="f9f28-259">activationLockBypassCode</span></span>|<span data-ttu-id="f9f28-260">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-260">String</span></span>|<span data-ttu-id="f9f28-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="f9f28-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="f9f28-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-262">This property is read-only.</span></span> <span data-ttu-id="f9f28-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f9f28-264">emailAddress</span></span>|<span data-ttu-id="f9f28-265">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-265">String</span></span>|<span data-ttu-id="f9f28-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="f9f28-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-267">This property is read-only.</span></span> <span data-ttu-id="f9f28-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="f9f28-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f9f28-270">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-270">String</span></span>|<span data-ttu-id="f9f28-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9f28-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f9f28-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-272">Read only.</span></span> <span data-ttu-id="f9f28-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-273">This property is read-only.</span></span> <span data-ttu-id="f9f28-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f9f28-275">azureADDeviceId</span></span>|<span data-ttu-id="f9f28-276">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-276">String</span></span>|<span data-ttu-id="f9f28-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9f28-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f9f28-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-278">Read only.</span></span> <span data-ttu-id="f9f28-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-279">This property is read-only.</span></span> <span data-ttu-id="f9f28-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f9f28-281">deviceRegistrationState</span></span>|[<span data-ttu-id="f9f28-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f9f28-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="f9f28-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-283">Device registration state.</span></span> <span data-ttu-id="f9f28-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-284">This property is read-only.</span></span> <span data-ttu-id="f9f28-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="f9f28-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9f28-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="f9f28-288">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-288">String</span></span>|<span data-ttu-id="f9f28-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-289">Device category display name.</span></span> <span data-ttu-id="f9f28-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-290">This property is read-only.</span></span> <span data-ttu-id="f9f28-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f9f28-292">isSupervised</span></span>|<span data-ttu-id="f9f28-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f28-293">Boolean</span></span>|<span data-ttu-id="f9f28-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-294">Device supervised status.</span></span> <span data-ttu-id="f9f28-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-295">This property is read-only.</span></span> <span data-ttu-id="f9f28-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f9f28-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-298">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9f28-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="f9f28-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-300">This property is read-only.</span></span> <span data-ttu-id="f9f28-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f9f28-302">exchangeAccessState</span></span>|[<span data-ttu-id="f9f28-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f9f28-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="f9f28-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9f28-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="f9f28-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-305">This property is read-only.</span></span> <span data-ttu-id="f9f28-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="f9f28-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f9f28-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="f9f28-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f9f28-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="f9f28-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9f28-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="f9f28-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-311">This property is read-only.</span></span> <span data-ttu-id="f9f28-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="f9f28-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="f9f28-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="f9f28-315">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-315">String</span></span>|<span data-ttu-id="f9f28-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="f9f28-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-317">This property is read-only.</span></span> <span data-ttu-id="f9f28-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f9f28-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="f9f28-320">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-320">String</span></span>|<span data-ttu-id="f9f28-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="f9f28-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="f9f28-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-322">This property is read-only.</span></span> <span data-ttu-id="f9f28-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f9f28-324">isEncrypted</span></span>|<span data-ttu-id="f9f28-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f28-325">Boolean</span></span>|<span data-ttu-id="f9f28-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-326">Device encryption status.</span></span> <span data-ttu-id="f9f28-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-327">This property is read-only.</span></span> <span data-ttu-id="f9f28-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9f28-329">userPrincipalName</span></span>|<span data-ttu-id="f9f28-330">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-330">String</span></span>|<span data-ttu-id="f9f28-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-331">Device user principal name.</span></span> <span data-ttu-id="f9f28-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-332">This property is read-only.</span></span> <span data-ttu-id="f9f28-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-334">modelo</span><span class="sxs-lookup"><span data-stu-id="f9f28-334">model</span></span>|<span data-ttu-id="f9f28-335">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-335">String</span></span>|<span data-ttu-id="f9f28-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-336">Model of the device.</span></span> <span data-ttu-id="f9f28-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-337">This property is read-only.</span></span> <span data-ttu-id="f9f28-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="f9f28-339">manufacturer</span></span>|<span data-ttu-id="f9f28-340">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-340">String</span></span>|<span data-ttu-id="f9f28-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-341">Manufacturer of the device.</span></span> <span data-ttu-id="f9f28-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-342">This property is read-only.</span></span> <span data-ttu-id="f9f28-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-344">imei</span><span class="sxs-lookup"><span data-stu-id="f9f28-344">imei</span></span>|<span data-ttu-id="f9f28-345">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-345">String</span></span>|<span data-ttu-id="f9f28-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="f9f28-346">IMEI.</span></span> <span data-ttu-id="f9f28-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-347">This property is read-only.</span></span> <span data-ttu-id="f9f28-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f9f28-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-350">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="f9f28-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="f9f28-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-352">This property is read-only.</span></span> <span data-ttu-id="f9f28-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f9f28-354">serialNumber</span></span>|<span data-ttu-id="f9f28-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9f28-355">String</span></span>|<span data-ttu-id="f9f28-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="f9f28-356">SerialNumber.</span></span> <span data-ttu-id="f9f28-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-357">This property is read-only.</span></span> <span data-ttu-id="f9f28-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f9f28-359">phoneNumber</span></span>|<span data-ttu-id="f9f28-360">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-360">String</span></span>|<span data-ttu-id="f9f28-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-361">Phone number of the device.</span></span> <span data-ttu-id="f9f28-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-362">This property is read-only.</span></span> <span data-ttu-id="f9f28-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f9f28-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="f9f28-365">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-365">String</span></span>|<span data-ttu-id="f9f28-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="f9f28-366">Android security patch level.</span></span> <span data-ttu-id="f9f28-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-367">This property is read-only.</span></span> <span data-ttu-id="f9f28-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9f28-369">userDisplayName</span></span>|<span data-ttu-id="f9f28-370">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-370">String</span></span>|<span data-ttu-id="f9f28-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9f28-371">User display name.</span></span> <span data-ttu-id="f9f28-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-372">This property is read-only.</span></span> <span data-ttu-id="f9f28-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f9f28-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="f9f28-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f9f28-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="f9f28-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="f9f28-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="f9f28-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-377">This property is read-only.</span></span> <span data-ttu-id="f9f28-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="f9f28-379">wiFiMacAddress</span></span>|<span data-ttu-id="f9f28-380">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-380">String</span></span>|<span data-ttu-id="f9f28-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f9f28-381">Wi-Fi MAC.</span></span> <span data-ttu-id="f9f28-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-382">This property is read-only.</span></span> <span data-ttu-id="f9f28-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f9f28-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="f9f28-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f9f28-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="f9f28-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-386">The device health attestation state.</span></span> <span data-ttu-id="f9f28-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-387">This property is read-only.</span></span> <span data-ttu-id="f9f28-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f9f28-389">subscriberCarrier</span></span>|<span data-ttu-id="f9f28-390">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-390">String</span></span>|<span data-ttu-id="f9f28-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="f9f28-391">Subscriber Carrier.</span></span> <span data-ttu-id="f9f28-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-392">This property is read-only.</span></span> <span data-ttu-id="f9f28-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-394">meid</span><span class="sxs-lookup"><span data-stu-id="f9f28-394">meid</span></span>|<span data-ttu-id="f9f28-395">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-395">String</span></span>|<span data-ttu-id="f9f28-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="f9f28-396">MEID.</span></span> <span data-ttu-id="f9f28-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-397">This property is read-only.</span></span> <span data-ttu-id="f9f28-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f9f28-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="f9f28-400">Int64</span><span class="sxs-lookup"><span data-stu-id="f9f28-400">Int64</span></span>|<span data-ttu-id="f9f28-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="f9f28-401">Total Storage in Bytes.</span></span> <span data-ttu-id="f9f28-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-402">This property is read-only.</span></span> <span data-ttu-id="f9f28-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f9f28-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="f9f28-405">Int64</span><span class="sxs-lookup"><span data-stu-id="f9f28-405">Int64</span></span>|<span data-ttu-id="f9f28-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="f9f28-406">Free Storage in Bytes.</span></span> <span data-ttu-id="f9f28-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-407">This property is read-only.</span></span> <span data-ttu-id="f9f28-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f9f28-409">managedDeviceName</span></span>|<span data-ttu-id="f9f28-410">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-410">String</span></span>|<span data-ttu-id="f9f28-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="f9f28-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f9f28-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="f9f28-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="f9f28-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="f9f28-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="f9f28-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="f9f28-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="f9f28-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-417">Read Only.</span></span> <span data-ttu-id="f9f28-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-418">This property is read-only.</span></span> <span data-ttu-id="f9f28-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9f28-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9f28-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="f9f28-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="f9f28-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-421">retireAfterDateTime</span></span>|<span data-ttu-id="f9f28-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-422">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="f9f28-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="f9f28-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-424">This property is read-only.</span></span> <span data-ttu-id="f9f28-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="f9f28-426">usersLoggedOn</span></span>|<span data-ttu-id="f9f28-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="f9f28-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="f9f28-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-429">This property is read-only.</span></span> <span data-ttu-id="f9f28-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f28-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="f9f28-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-432">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="f9f28-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="f9f28-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="f9f28-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="f9f28-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-435">Read Only.</span></span> <span data-ttu-id="f9f28-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-436">This property is read-only.</span></span> <span data-ttu-id="f9f28-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="f9f28-438">autopilotEnrolled</span></span>|<span data-ttu-id="f9f28-439">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9f28-439">Boolean</span></span>|<span data-ttu-id="f9f28-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="f9f28-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="f9f28-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-441">This property is read-only.</span></span> <span data-ttu-id="f9f28-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="f9f28-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="f9f28-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9f28-444">Boolean</span></span>|<span data-ttu-id="f9f28-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9f28-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="f9f28-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-446">This property is read-only.</span></span> <span data-ttu-id="f9f28-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="f9f28-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="f9f28-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f28-449">DateTimeOffset</span></span>|<span data-ttu-id="f9f28-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f9f28-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="f9f28-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-451">This property is read-only.</span></span> <span data-ttu-id="f9f28-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-453">iccid</span><span class="sxs-lookup"><span data-stu-id="f9f28-453">iccid</span></span>|<span data-ttu-id="f9f28-454">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-454">String</span></span>|<span data-ttu-id="f9f28-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="f9f28-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="f9f28-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-456">This property is read-only.</span></span> <span data-ttu-id="f9f28-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-458">udid</span><span class="sxs-lookup"><span data-stu-id="f9f28-458">udid</span></span>|<span data-ttu-id="f9f28-459">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-459">String</span></span>|<span data-ttu-id="f9f28-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="f9f28-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="f9f28-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-461">This property is read-only.</span></span> <span data-ttu-id="f9f28-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9f28-463">roleScopeTagIds</span></span>|<span data-ttu-id="f9f28-464">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f9f28-464">String collection</span></span>|<span data-ttu-id="f9f28-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9f28-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="f9f28-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f9f28-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="f9f28-468">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f28-468">Int32</span></span>|<span data-ttu-id="f9f28-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="f9f28-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="f9f28-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-470">This property is read-only.</span></span> <span data-ttu-id="f9f28-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f9f28-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="f9f28-473">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f28-473">Int32</span></span>|<span data-ttu-id="f9f28-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="f9f28-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="f9f28-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-475">This property is read-only.</span></span> <span data-ttu-id="f9f28-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-477">notes</span><span class="sxs-lookup"><span data-stu-id="f9f28-477">notes</span></span>|<span data-ttu-id="f9f28-478">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-478">String</span></span>|<span data-ttu-id="f9f28-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f9f28-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="f9f28-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f9f28-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="f9f28-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="f9f28-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="f9f28-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="f9f28-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="f9f28-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9f28-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="f9f28-486">ethernetMacAddress</span></span>|<span data-ttu-id="f9f28-487">String</span><span class="sxs-lookup"><span data-stu-id="f9f28-487">String</span></span>|<span data-ttu-id="f9f28-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="f9f28-488">Ethernet MAC.</span></span> <span data-ttu-id="f9f28-489">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9f28-489">This property is read-only.</span></span> <span data-ttu-id="f9f28-490">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9f28-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f9f28-491">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f28-491">Response</span></span>
<span data-ttu-id="f9f28-492">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f28-492">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f28-493">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9f28-493">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9f28-494">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f28-494">Request</span></span>
<span data-ttu-id="f9f28-495">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9f28-495">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7575

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
  "ethernetMacAddress": "Ethernet Mac Address value"
}
```

### <a name="response"></a><span data-ttu-id="f9f28-496">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f28-496">Response</span></span>
<span data-ttu-id="f9f28-p169">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9f28-p169">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7624

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
  "ethernetMacAddress": "Ethernet Mac Address value"
}
```






