---
title: Atualizar windowsManagedDevice
description: Atualiza as propriedades de um objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73898965523a71d9ee9544922c56f7d7f3abaa63
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467764"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="31de0-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="31de0-103">Update windowsManagedDevice</span></span>

<span data-ttu-id="31de0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31de0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31de0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31de0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31de0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31de0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31de0-107">Atualiza as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="31de0-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31de0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31de0-108">Prerequisites</span></span>
<span data-ttu-id="31de0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31de0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31de0-111">Permission type</span></span>|<span data-ttu-id="31de0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31de0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31de0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31de0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31de0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31de0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="31de0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31de0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31de0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31de0-116">Not supported.</span></span>|
|<span data-ttu-id="31de0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31de0-117">Application</span></span>|<span data-ttu-id="31de0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31de0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31de0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31de0-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="31de0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31de0-120">Request headers</span></span>
|<span data-ttu-id="31de0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31de0-121">Header</span></span>|<span data-ttu-id="31de0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31de0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31de0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31de0-123">Authorization</span></span>|<span data-ttu-id="31de0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31de0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31de0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31de0-125">Accept</span></span>|<span data-ttu-id="31de0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31de0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31de0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31de0-127">Request body</span></span>
<span data-ttu-id="31de0-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="31de0-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="31de0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="31de0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31de0-130">Property</span></span>|<span data-ttu-id="31de0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31de0-131">Type</span></span>|<span data-ttu-id="31de0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31de0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31de0-133">id</span><span class="sxs-lookup"><span data-stu-id="31de0-133">id</span></span>|<span data-ttu-id="31de0-134">String</span><span class="sxs-lookup"><span data-stu-id="31de0-134">String</span></span>|<span data-ttu-id="31de0-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-135">Unique Identifier for the device.</span></span> <span data-ttu-id="31de0-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-136">This property is read-only.</span></span> <span data-ttu-id="31de0-137">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-138">userId</span><span class="sxs-lookup"><span data-stu-id="31de0-138">userId</span></span>|<span data-ttu-id="31de0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31de0-139">String</span></span>|<span data-ttu-id="31de0-140">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="31de0-141">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-141">This property is read-only.</span></span> <span data-ttu-id="31de0-142">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="31de0-143">deviceName</span></span>|<span data-ttu-id="31de0-144">String</span><span class="sxs-lookup"><span data-stu-id="31de0-144">String</span></span>|<span data-ttu-id="31de0-145">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-145">Name of the device.</span></span> <span data-ttu-id="31de0-146">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-146">This property is read-only.</span></span> <span data-ttu-id="31de0-147">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="31de0-148">hardwareInformation</span></span>|[<span data-ttu-id="31de0-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="31de0-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="31de0-150">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-150">The hardward details for the device.</span></span>  <span data-ttu-id="31de0-151">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="31de0-152">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="31de0-153">ownerType</span></span>|[<span data-ttu-id="31de0-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="31de0-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="31de0-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-155">Ownership of the device.</span></span> <span data-ttu-id="31de0-156">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="31de0-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="31de0-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="31de0-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="31de0-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="31de0-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="31de0-160">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-160">Ownership of the device.</span></span> <span data-ttu-id="31de0-161">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-162">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="31de0-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="31de0-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="31de0-163">deviceActionResults</span></span>|<span data-ttu-id="31de0-164">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="31de0-165">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="31de0-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="31de0-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-166">This property is read-only.</span></span> <span data-ttu-id="31de0-167">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="31de0-168">managementState</span></span>|[<span data-ttu-id="31de0-169">ManagementState</span><span class="sxs-lookup"><span data-stu-id="31de0-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="31de0-170">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-170">Management state of the device.</span></span> <span data-ttu-id="31de0-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-171">This property is read-only.</span></span> <span data-ttu-id="31de0-172">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-173">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="31de0-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="31de0-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-174">enrolledDateTime</span></span>|<span data-ttu-id="31de0-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-175">DateTimeOffset</span></span>|<span data-ttu-id="31de0-176">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-176">Enrollment time of the device.</span></span> <span data-ttu-id="31de0-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-177">This property is read-only.</span></span> <span data-ttu-id="31de0-178">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-179">lastSyncDateTime</span></span>|<span data-ttu-id="31de0-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-180">DateTimeOffset</span></span>|<span data-ttu-id="31de0-181">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="31de0-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="31de0-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-182">This property is read-only.</span></span> <span data-ttu-id="31de0-183">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="31de0-184">chassisType</span></span>|[<span data-ttu-id="31de0-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="31de0-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="31de0-186">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-186">Chassis type of the device.</span></span> <span data-ttu-id="31de0-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-187">This property is read-only.</span></span> <span data-ttu-id="31de0-188">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-189">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="31de0-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="31de0-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="31de0-190">operatingSystem</span></span>|<span data-ttu-id="31de0-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31de0-191">String</span></span>|<span data-ttu-id="31de0-192">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-192">Operating system of the device.</span></span> <span data-ttu-id="31de0-193">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="31de0-194">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="31de0-195">deviceType</span></span>|[<span data-ttu-id="31de0-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="31de0-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="31de0-197">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-197">Platform of the device.</span></span> <span data-ttu-id="31de0-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-198">This property is read-only.</span></span> <span data-ttu-id="31de0-199">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-200">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="31de0-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="31de0-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="31de0-201">complianceState</span></span>|[<span data-ttu-id="31de0-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="31de0-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="31de0-203">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-203">Compliance state of the device.</span></span> <span data-ttu-id="31de0-204">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-204">This property is read-only.</span></span> <span data-ttu-id="31de0-205">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-206">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="31de0-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="31de0-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="31de0-207">jailBroken</span></span>|<span data-ttu-id="31de0-208">String</span><span class="sxs-lookup"><span data-stu-id="31de0-208">String</span></span>|<span data-ttu-id="31de0-209">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="31de0-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="31de0-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-210">This property is read-only.</span></span> <span data-ttu-id="31de0-211">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="31de0-212">managementAgent</span></span>|[<span data-ttu-id="31de0-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="31de0-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="31de0-214">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-214">Management channel of the device.</span></span> <span data-ttu-id="31de0-215">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="31de0-216">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-217">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="31de0-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="31de0-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="31de0-218">osVersion</span></span>|<span data-ttu-id="31de0-219">String</span><span class="sxs-lookup"><span data-stu-id="31de0-219">String</span></span>|<span data-ttu-id="31de0-220">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-220">Operating system version of the device.</span></span> <span data-ttu-id="31de0-221">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-221">This property is read-only.</span></span> <span data-ttu-id="31de0-222">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="31de0-223">easActivated</span></span>|<span data-ttu-id="31de0-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-224">Boolean</span></span>|<span data-ttu-id="31de0-225">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="31de0-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="31de0-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-226">This property is read-only.</span></span> <span data-ttu-id="31de0-227">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="31de0-228">easDeviceId</span></span>|<span data-ttu-id="31de0-229">String</span><span class="sxs-lookup"><span data-stu-id="31de0-229">String</span></span>|<span data-ttu-id="31de0-230">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="31de0-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-231">This property is read-only.</span></span> <span data-ttu-id="31de0-232">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-233">easActivationDateTime</span></span>|<span data-ttu-id="31de0-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-234">DateTimeOffset</span></span>|<span data-ttu-id="31de0-235">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="31de0-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-236">This property is read-only.</span></span> <span data-ttu-id="31de0-237">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="31de0-238">aadRegistered</span></span>|<span data-ttu-id="31de0-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-239">Boolean</span></span>|<span data-ttu-id="31de0-240">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31de0-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="31de0-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-241">This property is read-only.</span></span> <span data-ttu-id="31de0-242">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="31de0-243">azureADRegistered</span></span>|<span data-ttu-id="31de0-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-244">Boolean</span></span>|<span data-ttu-id="31de0-245">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31de0-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="31de0-246">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-246">This property is read-only.</span></span> <span data-ttu-id="31de0-247">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="31de0-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="31de0-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="31de0-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="31de0-250">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-250">Enrollment type of the device.</span></span> <span data-ttu-id="31de0-251">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-251">This property is read-only.</span></span> <span data-ttu-id="31de0-252">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-253">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="31de0-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="31de0-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="31de0-254">lostModeState</span></span>|[<span data-ttu-id="31de0-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="31de0-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="31de0-256">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="31de0-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="31de0-257">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-257">This property is read-only.</span></span> <span data-ttu-id="31de0-258">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-259">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="31de0-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="31de0-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="31de0-260">activationLockBypassCode</span></span>|<span data-ttu-id="31de0-261">String</span><span class="sxs-lookup"><span data-stu-id="31de0-261">String</span></span>|<span data-ttu-id="31de0-262">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="31de0-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="31de0-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-263">This property is read-only.</span></span> <span data-ttu-id="31de0-264">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="31de0-265">emailAddress</span></span>|<span data-ttu-id="31de0-266">String</span><span class="sxs-lookup"><span data-stu-id="31de0-266">String</span></span>|<span data-ttu-id="31de0-267">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="31de0-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-268">This property is read-only.</span></span> <span data-ttu-id="31de0-269">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="31de0-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="31de0-271">String</span><span class="sxs-lookup"><span data-stu-id="31de0-271">String</span></span>|<span data-ttu-id="31de0-272">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31de0-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="31de0-273">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-273">Read only.</span></span> <span data-ttu-id="31de0-274">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-274">This property is read-only.</span></span> <span data-ttu-id="31de0-275">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="31de0-276">azureADDeviceId</span></span>|<span data-ttu-id="31de0-277">String</span><span class="sxs-lookup"><span data-stu-id="31de0-277">String</span></span>|<span data-ttu-id="31de0-278">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31de0-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="31de0-279">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-279">Read only.</span></span> <span data-ttu-id="31de0-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-280">This property is read-only.</span></span> <span data-ttu-id="31de0-281">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="31de0-282">deviceRegistrationState</span></span>|[<span data-ttu-id="31de0-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="31de0-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="31de0-284">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-284">Device registration state.</span></span> <span data-ttu-id="31de0-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-285">This property is read-only.</span></span> <span data-ttu-id="31de0-286">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-287">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="31de0-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="31de0-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="31de0-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="31de0-289">String</span><span class="sxs-lookup"><span data-stu-id="31de0-289">String</span></span>|<span data-ttu-id="31de0-290">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-290">Device category display name.</span></span> <span data-ttu-id="31de0-291">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-291">This property is read-only.</span></span> <span data-ttu-id="31de0-292">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="31de0-293">isSupervised</span></span>|<span data-ttu-id="31de0-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-294">Boolean</span></span>|<span data-ttu-id="31de0-295">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-295">Device supervised status.</span></span> <span data-ttu-id="31de0-296">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-296">This property is read-only.</span></span> <span data-ttu-id="31de0-297">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="31de0-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-299">DateTimeOffset</span></span>|<span data-ttu-id="31de0-300">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="31de0-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="31de0-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-301">This property is read-only.</span></span> <span data-ttu-id="31de0-302">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="31de0-303">exchangeAccessState</span></span>|[<span data-ttu-id="31de0-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="31de0-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="31de0-305">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="31de0-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="31de0-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-306">This property is read-only.</span></span> <span data-ttu-id="31de0-307">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-308">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="31de0-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="31de0-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="31de0-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="31de0-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="31de0-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="31de0-311">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="31de0-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="31de0-312">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-312">This property is read-only.</span></span> <span data-ttu-id="31de0-313">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-314">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="31de0-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="31de0-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="31de0-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="31de0-316">String</span><span class="sxs-lookup"><span data-stu-id="31de0-316">String</span></span>|<span data-ttu-id="31de0-317">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="31de0-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-318">This property is read-only.</span></span> <span data-ttu-id="31de0-319">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="31de0-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="31de0-321">String</span><span class="sxs-lookup"><span data-stu-id="31de0-321">String</span></span>|<span data-ttu-id="31de0-322">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="31de0-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="31de0-323">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-323">This property is read-only.</span></span> <span data-ttu-id="31de0-324">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="31de0-325">isEncrypted</span></span>|<span data-ttu-id="31de0-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-326">Boolean</span></span>|<span data-ttu-id="31de0-327">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-327">Device encryption status.</span></span> <span data-ttu-id="31de0-328">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-328">This property is read-only.</span></span> <span data-ttu-id="31de0-329">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="31de0-330">userPrincipalName</span></span>|<span data-ttu-id="31de0-331">String</span><span class="sxs-lookup"><span data-stu-id="31de0-331">String</span></span>|<span data-ttu-id="31de0-332">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-332">Device user principal name.</span></span> <span data-ttu-id="31de0-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-333">This property is read-only.</span></span> <span data-ttu-id="31de0-334">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-335">modelo</span><span class="sxs-lookup"><span data-stu-id="31de0-335">model</span></span>|<span data-ttu-id="31de0-336">String</span><span class="sxs-lookup"><span data-stu-id="31de0-336">String</span></span>|<span data-ttu-id="31de0-337">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-337">Model of the device.</span></span> <span data-ttu-id="31de0-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-338">This property is read-only.</span></span> <span data-ttu-id="31de0-339">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-340">fabricante</span><span class="sxs-lookup"><span data-stu-id="31de0-340">manufacturer</span></span>|<span data-ttu-id="31de0-341">String</span><span class="sxs-lookup"><span data-stu-id="31de0-341">String</span></span>|<span data-ttu-id="31de0-342">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-342">Manufacturer of the device.</span></span> <span data-ttu-id="31de0-343">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-343">This property is read-only.</span></span> <span data-ttu-id="31de0-344">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-345">imei</span><span class="sxs-lookup"><span data-stu-id="31de0-345">imei</span></span>|<span data-ttu-id="31de0-346">String</span><span class="sxs-lookup"><span data-stu-id="31de0-346">String</span></span>|<span data-ttu-id="31de0-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="31de0-347">IMEI.</span></span> <span data-ttu-id="31de0-348">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-348">This property is read-only.</span></span> <span data-ttu-id="31de0-349">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="31de0-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-351">DateTimeOffset</span></span>|<span data-ttu-id="31de0-352">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="31de0-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="31de0-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-353">This property is read-only.</span></span> <span data-ttu-id="31de0-354">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="31de0-355">serialNumber</span></span>|<span data-ttu-id="31de0-356">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31de0-356">String</span></span>|<span data-ttu-id="31de0-357">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="31de0-357">SerialNumber.</span></span> <span data-ttu-id="31de0-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-358">This property is read-only.</span></span> <span data-ttu-id="31de0-359">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="31de0-360">phoneNumber</span></span>|<span data-ttu-id="31de0-361">String</span><span class="sxs-lookup"><span data-stu-id="31de0-361">String</span></span>|<span data-ttu-id="31de0-362">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-362">Phone number of the device.</span></span> <span data-ttu-id="31de0-363">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-363">This property is read-only.</span></span> <span data-ttu-id="31de0-364">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="31de0-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="31de0-366">String</span><span class="sxs-lookup"><span data-stu-id="31de0-366">String</span></span>|<span data-ttu-id="31de0-367">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="31de0-367">Android security patch level.</span></span> <span data-ttu-id="31de0-368">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-368">This property is read-only.</span></span> <span data-ttu-id="31de0-369">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="31de0-370">userDisplayName</span></span>|<span data-ttu-id="31de0-371">String</span><span class="sxs-lookup"><span data-stu-id="31de0-371">String</span></span>|<span data-ttu-id="31de0-372">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="31de0-372">User display name.</span></span> <span data-ttu-id="31de0-373">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-373">This property is read-only.</span></span> <span data-ttu-id="31de0-374">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="31de0-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="31de0-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="31de0-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="31de0-377">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="31de0-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="31de0-378">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-378">This property is read-only.</span></span> <span data-ttu-id="31de0-379">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="31de0-380">wiFiMacAddress</span></span>|<span data-ttu-id="31de0-381">String</span><span class="sxs-lookup"><span data-stu-id="31de0-381">String</span></span>|<span data-ttu-id="31de0-382">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="31de0-382">Wi-Fi MAC.</span></span> <span data-ttu-id="31de0-383">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-383">This property is read-only.</span></span> <span data-ttu-id="31de0-384">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="31de0-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="31de0-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="31de0-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="31de0-387">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-387">The device health attestation state.</span></span> <span data-ttu-id="31de0-388">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-388">This property is read-only.</span></span> <span data-ttu-id="31de0-389">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="31de0-390">subscriberCarrier</span></span>|<span data-ttu-id="31de0-391">String</span><span class="sxs-lookup"><span data-stu-id="31de0-391">String</span></span>|<span data-ttu-id="31de0-392">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="31de0-392">Subscriber Carrier.</span></span> <span data-ttu-id="31de0-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-393">This property is read-only.</span></span> <span data-ttu-id="31de0-394">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-395">meid</span><span class="sxs-lookup"><span data-stu-id="31de0-395">meid</span></span>|<span data-ttu-id="31de0-396">String</span><span class="sxs-lookup"><span data-stu-id="31de0-396">String</span></span>|<span data-ttu-id="31de0-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="31de0-397">MEID.</span></span> <span data-ttu-id="31de0-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-398">This property is read-only.</span></span> <span data-ttu-id="31de0-399">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="31de0-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="31de0-401">Int64</span><span class="sxs-lookup"><span data-stu-id="31de0-401">Int64</span></span>|<span data-ttu-id="31de0-402">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="31de0-402">Total Storage in Bytes.</span></span> <span data-ttu-id="31de0-403">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-403">This property is read-only.</span></span> <span data-ttu-id="31de0-404">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="31de0-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="31de0-406">Int64</span><span class="sxs-lookup"><span data-stu-id="31de0-406">Int64</span></span>|<span data-ttu-id="31de0-407">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="31de0-407">Free Storage in Bytes.</span></span> <span data-ttu-id="31de0-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-408">This property is read-only.</span></span> <span data-ttu-id="31de0-409">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="31de0-410">managedDeviceName</span></span>|<span data-ttu-id="31de0-411">String</span><span class="sxs-lookup"><span data-stu-id="31de0-411">String</span></span>|<span data-ttu-id="31de0-412">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="31de0-413">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="31de0-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="31de0-414">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="31de0-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="31de0-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="31de0-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="31de0-417">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="31de0-418">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-418">Read Only.</span></span> <span data-ttu-id="31de0-419">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-419">This property is read-only.</span></span> <span data-ttu-id="31de0-420">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-421">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="31de0-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="31de0-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-422">retireAfterDateTime</span></span>|<span data-ttu-id="31de0-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-423">DateTimeOffset</span></span>|<span data-ttu-id="31de0-424">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="31de0-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="31de0-425">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-425">This property is read-only.</span></span> <span data-ttu-id="31de0-426">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="31de0-427">usersLoggedOn</span></span>|<span data-ttu-id="31de0-428">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="31de0-429">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="31de0-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-430">This property is read-only.</span></span> <span data-ttu-id="31de0-431">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="31de0-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="31de0-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-433">DateTimeOffset</span></span>|<span data-ttu-id="31de0-434">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="31de0-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="31de0-435">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="31de0-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="31de0-436">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-436">Read Only.</span></span> <span data-ttu-id="31de0-437">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-437">This property is read-only.</span></span> <span data-ttu-id="31de0-438">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="31de0-439">autopilotEnrolled</span></span>|<span data-ttu-id="31de0-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-440">Boolean</span></span>|<span data-ttu-id="31de0-441">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="31de0-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="31de0-442">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-442">This property is read-only.</span></span> <span data-ttu-id="31de0-443">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="31de0-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="31de0-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="31de0-445">Boolean</span></span>|<span data-ttu-id="31de0-446">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="31de0-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="31de0-447">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-447">This property is read-only.</span></span> <span data-ttu-id="31de0-448">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="31de0-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="31de0-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31de0-450">DateTimeOffset</span></span>|<span data-ttu-id="31de0-451">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31de0-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="31de0-452">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-452">This property is read-only.</span></span> <span data-ttu-id="31de0-453">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-454">iccid</span><span class="sxs-lookup"><span data-stu-id="31de0-454">iccid</span></span>|<span data-ttu-id="31de0-455">String</span><span class="sxs-lookup"><span data-stu-id="31de0-455">String</span></span>|<span data-ttu-id="31de0-456">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="31de0-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="31de0-457">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-457">This property is read-only.</span></span> <span data-ttu-id="31de0-458">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-459">udid</span><span class="sxs-lookup"><span data-stu-id="31de0-459">udid</span></span>|<span data-ttu-id="31de0-460">String</span><span class="sxs-lookup"><span data-stu-id="31de0-460">String</span></span>|<span data-ttu-id="31de0-461">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="31de0-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="31de0-462">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-462">This property is read-only.</span></span> <span data-ttu-id="31de0-463">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31de0-464">roleScopeTagIds</span></span>|<span data-ttu-id="31de0-465">String collection</span><span class="sxs-lookup"><span data-stu-id="31de0-465">String collection</span></span>|<span data-ttu-id="31de0-466">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31de0-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="31de0-467">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="31de0-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="31de0-469">Int32</span><span class="sxs-lookup"><span data-stu-id="31de0-469">Int32</span></span>|<span data-ttu-id="31de0-470">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="31de0-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="31de0-471">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-471">This property is read-only.</span></span> <span data-ttu-id="31de0-472">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="31de0-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="31de0-474">Int32</span><span class="sxs-lookup"><span data-stu-id="31de0-474">Int32</span></span>|<span data-ttu-id="31de0-475">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="31de0-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="31de0-476">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-476">This property is read-only.</span></span> <span data-ttu-id="31de0-477">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-478">notes</span><span class="sxs-lookup"><span data-stu-id="31de0-478">notes</span></span>|<span data-ttu-id="31de0-479">String</span><span class="sxs-lookup"><span data-stu-id="31de0-479">String</span></span>|<span data-ttu-id="31de0-480">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="31de0-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="31de0-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="31de0-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="31de0-483">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="31de0-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="31de0-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="31de0-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="31de0-486">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="31de0-487">ethernetMacAddress</span></span>|<span data-ttu-id="31de0-488">String</span><span class="sxs-lookup"><span data-stu-id="31de0-488">String</span></span>|<span data-ttu-id="31de0-489">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="31de0-489">Ethernet MAC.</span></span> <span data-ttu-id="31de0-490">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-490">This property is read-only.</span></span> <span data-ttu-id="31de0-491">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="31de0-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="31de0-493">Int64</span><span class="sxs-lookup"><span data-stu-id="31de0-493">Int64</span></span>|<span data-ttu-id="31de0-494">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="31de0-494">Total Memory in Bytes.</span></span> <span data-ttu-id="31de0-495">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-495">This property is read-only.</span></span> <span data-ttu-id="31de0-496">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="31de0-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="31de0-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="31de0-497">processorArchitecture</span></span>|[<span data-ttu-id="31de0-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="31de0-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="31de0-499">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="31de0-499">Processor architecture.</span></span> <span data-ttu-id="31de0-500">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31de0-500">This property is read-only.</span></span> <span data-ttu-id="31de0-501">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="31de0-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="31de0-502">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="31de0-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="31de0-503">Resposta</span><span class="sxs-lookup"><span data-stu-id="31de0-503">Response</span></span>
<span data-ttu-id="31de0-504">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31de0-504">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31de0-505">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31de0-505">Example</span></span>

### <a name="request"></a><span data-ttu-id="31de0-506">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31de0-506">Request</span></span>
<span data-ttu-id="31de0-507">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31de0-507">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="31de0-508">Resposta</span><span class="sxs-lookup"><span data-stu-id="31de0-508">Response</span></span>
<span data-ttu-id="31de0-p171">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31de0-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





