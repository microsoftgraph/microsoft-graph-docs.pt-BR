---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75f6393938d8dfb72fffd4d5afe2698a0fa787fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813667"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="efa21-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="efa21-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="efa21-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="efa21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efa21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa21-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="efa21-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efa21-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efa21-107">Prerequisites</span></span>
<span data-ttu-id="efa21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efa21-110">Permission type</span></span>|<span data-ttu-id="efa21-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efa21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efa21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efa21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efa21-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa21-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="efa21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efa21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efa21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efa21-115">Not supported.</span></span>|
|<span data-ttu-id="efa21-116">Application</span><span class="sxs-lookup"><span data-stu-id="efa21-116">Application</span></span>|<span data-ttu-id="efa21-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa21-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efa21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efa21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="efa21-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efa21-119">Request headers</span></span>
|<span data-ttu-id="efa21-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efa21-120">Header</span></span>|<span data-ttu-id="efa21-121">Valor</span><span class="sxs-lookup"><span data-stu-id="efa21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efa21-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="efa21-122">Authorization</span></span>|<span data-ttu-id="efa21-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efa21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efa21-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efa21-124">Accept</span></span>|<span data-ttu-id="efa21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efa21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa21-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efa21-126">Request body</span></span>
<span data-ttu-id="efa21-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="efa21-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="efa21-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="efa21-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="efa21-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efa21-129">Property</span></span>|<span data-ttu-id="efa21-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa21-130">Type</span></span>|<span data-ttu-id="efa21-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa21-132">id</span><span class="sxs-lookup"><span data-stu-id="efa21-132">id</span></span>|<span data-ttu-id="efa21-133">String</span><span class="sxs-lookup"><span data-stu-id="efa21-133">String</span></span>|<span data-ttu-id="efa21-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-134">Unique Identifier for the device.</span></span> <span data-ttu-id="efa21-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-135">This property is read-only.</span></span> <span data-ttu-id="efa21-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-137">userId</span><span class="sxs-lookup"><span data-stu-id="efa21-137">userId</span></span>|<span data-ttu-id="efa21-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa21-138">String</span></span>|<span data-ttu-id="efa21-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="efa21-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-140">This property is read-only.</span></span> <span data-ttu-id="efa21-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="efa21-142">deviceName</span></span>|<span data-ttu-id="efa21-143">String</span><span class="sxs-lookup"><span data-stu-id="efa21-143">String</span></span>|<span data-ttu-id="efa21-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-144">Name of the device.</span></span> <span data-ttu-id="efa21-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-145">This property is read-only.</span></span> <span data-ttu-id="efa21-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="efa21-147">hardwareInformation</span></span>|[<span data-ttu-id="efa21-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="efa21-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="efa21-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-149">The hardward details for the device.</span></span>  <span data-ttu-id="efa21-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="efa21-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="efa21-152">ownerType</span></span>|[<span data-ttu-id="efa21-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="efa21-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="efa21-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-154">Ownership of the device.</span></span> <span data-ttu-id="efa21-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="efa21-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="efa21-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="efa21-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="efa21-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="efa21-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="efa21-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-159">Ownership of the device.</span></span> <span data-ttu-id="efa21-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="efa21-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="efa21-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="efa21-162">deviceActionResults</span></span>|<span data-ttu-id="efa21-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="efa21-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="efa21-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="efa21-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-165">This property is read-only.</span></span> <span data-ttu-id="efa21-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="efa21-167">managementState</span></span>|[<span data-ttu-id="efa21-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="efa21-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="efa21-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-169">Management state of the device.</span></span> <span data-ttu-id="efa21-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-170">This property is read-only.</span></span> <span data-ttu-id="efa21-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="efa21-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="efa21-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-173">enrolledDateTime</span></span>|<span data-ttu-id="efa21-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-174">DateTimeOffset</span></span>|<span data-ttu-id="efa21-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-175">Enrollment time of the device.</span></span> <span data-ttu-id="efa21-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-176">This property is read-only.</span></span> <span data-ttu-id="efa21-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-178">lastSyncDateTime</span></span>|<span data-ttu-id="efa21-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-179">DateTimeOffset</span></span>|<span data-ttu-id="efa21-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="efa21-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="efa21-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-181">This property is read-only.</span></span> <span data-ttu-id="efa21-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="efa21-183">chassisType</span></span>|[<span data-ttu-id="efa21-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="efa21-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="efa21-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-185">Chassis type of the device.</span></span> <span data-ttu-id="efa21-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-186">This property is read-only.</span></span> <span data-ttu-id="efa21-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="efa21-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="efa21-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="efa21-189">operatingSystem</span></span>|<span data-ttu-id="efa21-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa21-190">String</span></span>|<span data-ttu-id="efa21-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-191">Operating system of the device.</span></span> <span data-ttu-id="efa21-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="efa21-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="efa21-194">deviceType</span></span>|[<span data-ttu-id="efa21-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="efa21-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="efa21-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-196">Platform of the device.</span></span> <span data-ttu-id="efa21-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-197">This property is read-only.</span></span> <span data-ttu-id="efa21-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="efa21-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="efa21-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="efa21-200">complianceState</span></span>|[<span data-ttu-id="efa21-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="efa21-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="efa21-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-202">Compliance state of the device.</span></span> <span data-ttu-id="efa21-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-203">This property is read-only.</span></span> <span data-ttu-id="efa21-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="efa21-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="efa21-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="efa21-206">jailBroken</span></span>|<span data-ttu-id="efa21-207">String</span><span class="sxs-lookup"><span data-stu-id="efa21-207">String</span></span>|<span data-ttu-id="efa21-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="efa21-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="efa21-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-209">This property is read-only.</span></span> <span data-ttu-id="efa21-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="efa21-211">managementAgent</span></span>|[<span data-ttu-id="efa21-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="efa21-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="efa21-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-213">Management channel of the device.</span></span> <span data-ttu-id="efa21-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="efa21-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="efa21-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="efa21-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="efa21-217">osVersion</span></span>|<span data-ttu-id="efa21-218">String</span><span class="sxs-lookup"><span data-stu-id="efa21-218">String</span></span>|<span data-ttu-id="efa21-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-219">Operating system version of the device.</span></span> <span data-ttu-id="efa21-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-220">This property is read-only.</span></span> <span data-ttu-id="efa21-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="efa21-222">easActivated</span></span>|<span data-ttu-id="efa21-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-223">Boolean</span></span>|<span data-ttu-id="efa21-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="efa21-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="efa21-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-225">This property is read-only.</span></span> <span data-ttu-id="efa21-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="efa21-227">easDeviceId</span></span>|<span data-ttu-id="efa21-228">String</span><span class="sxs-lookup"><span data-stu-id="efa21-228">String</span></span>|<span data-ttu-id="efa21-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="efa21-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-230">This property is read-only.</span></span> <span data-ttu-id="efa21-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-232">easActivationDateTime</span></span>|<span data-ttu-id="efa21-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-233">DateTimeOffset</span></span>|<span data-ttu-id="efa21-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="efa21-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-235">This property is read-only.</span></span> <span data-ttu-id="efa21-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="efa21-237">aadRegistered</span></span>|<span data-ttu-id="efa21-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-238">Boolean</span></span>|<span data-ttu-id="efa21-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="efa21-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="efa21-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-240">This property is read-only.</span></span> <span data-ttu-id="efa21-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="efa21-242">azureADRegistered</span></span>|<span data-ttu-id="efa21-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-243">Boolean</span></span>|<span data-ttu-id="efa21-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="efa21-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="efa21-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-245">This property is read-only.</span></span> <span data-ttu-id="efa21-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="efa21-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="efa21-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="efa21-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="efa21-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-249">Enrollment type of the device.</span></span> <span data-ttu-id="efa21-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-250">This property is read-only.</span></span> <span data-ttu-id="efa21-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="efa21-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="efa21-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="efa21-253">lostModeState</span></span>|[<span data-ttu-id="efa21-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="efa21-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="efa21-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="efa21-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="efa21-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-256">This property is read-only.</span></span> <span data-ttu-id="efa21-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="efa21-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="efa21-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="efa21-259">activationLockBypassCode</span></span>|<span data-ttu-id="efa21-260">String</span><span class="sxs-lookup"><span data-stu-id="efa21-260">String</span></span>|<span data-ttu-id="efa21-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="efa21-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="efa21-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-262">This property is read-only.</span></span> <span data-ttu-id="efa21-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="efa21-264">emailAddress</span></span>|<span data-ttu-id="efa21-265">String</span><span class="sxs-lookup"><span data-stu-id="efa21-265">String</span></span>|<span data-ttu-id="efa21-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="efa21-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-267">This property is read-only.</span></span> <span data-ttu-id="efa21-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="efa21-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="efa21-270">String</span><span class="sxs-lookup"><span data-stu-id="efa21-270">String</span></span>|<span data-ttu-id="efa21-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="efa21-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="efa21-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-272">Read only.</span></span> <span data-ttu-id="efa21-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-273">This property is read-only.</span></span> <span data-ttu-id="efa21-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="efa21-275">azureADDeviceId</span></span>|<span data-ttu-id="efa21-276">String</span><span class="sxs-lookup"><span data-stu-id="efa21-276">String</span></span>|<span data-ttu-id="efa21-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="efa21-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="efa21-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-278">Read only.</span></span> <span data-ttu-id="efa21-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-279">This property is read-only.</span></span> <span data-ttu-id="efa21-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="efa21-281">deviceRegistrationState</span></span>|[<span data-ttu-id="efa21-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="efa21-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="efa21-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-283">Device registration state.</span></span> <span data-ttu-id="efa21-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-284">This property is read-only.</span></span> <span data-ttu-id="efa21-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="efa21-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="efa21-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="efa21-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="efa21-288">String</span><span class="sxs-lookup"><span data-stu-id="efa21-288">String</span></span>|<span data-ttu-id="efa21-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-289">Device category display name.</span></span> <span data-ttu-id="efa21-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-290">This property is read-only.</span></span> <span data-ttu-id="efa21-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="efa21-292">isSupervised</span></span>|<span data-ttu-id="efa21-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-293">Boolean</span></span>|<span data-ttu-id="efa21-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-294">Device supervised status.</span></span> <span data-ttu-id="efa21-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-295">This property is read-only.</span></span> <span data-ttu-id="efa21-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="efa21-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-298">DateTimeOffset</span></span>|<span data-ttu-id="efa21-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="efa21-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="efa21-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-300">This property is read-only.</span></span> <span data-ttu-id="efa21-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="efa21-302">exchangeAccessState</span></span>|[<span data-ttu-id="efa21-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="efa21-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="efa21-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="efa21-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="efa21-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-305">This property is read-only.</span></span> <span data-ttu-id="efa21-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="efa21-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="efa21-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="efa21-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="efa21-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="efa21-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="efa21-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="efa21-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="efa21-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-311">This property is read-only.</span></span> <span data-ttu-id="efa21-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="efa21-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="efa21-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="efa21-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="efa21-315">String</span><span class="sxs-lookup"><span data-stu-id="efa21-315">String</span></span>|<span data-ttu-id="efa21-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="efa21-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-317">This property is read-only.</span></span> <span data-ttu-id="efa21-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="efa21-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="efa21-320">String</span><span class="sxs-lookup"><span data-stu-id="efa21-320">String</span></span>|<span data-ttu-id="efa21-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="efa21-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="efa21-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-322">This property is read-only.</span></span> <span data-ttu-id="efa21-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="efa21-324">isEncrypted</span></span>|<span data-ttu-id="efa21-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-325">Boolean</span></span>|<span data-ttu-id="efa21-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-326">Device encryption status.</span></span> <span data-ttu-id="efa21-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-327">This property is read-only.</span></span> <span data-ttu-id="efa21-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="efa21-329">userPrincipalName</span></span>|<span data-ttu-id="efa21-330">String</span><span class="sxs-lookup"><span data-stu-id="efa21-330">String</span></span>|<span data-ttu-id="efa21-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-331">Device user principal name.</span></span> <span data-ttu-id="efa21-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-332">This property is read-only.</span></span> <span data-ttu-id="efa21-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-334">modelo</span><span class="sxs-lookup"><span data-stu-id="efa21-334">model</span></span>|<span data-ttu-id="efa21-335">String</span><span class="sxs-lookup"><span data-stu-id="efa21-335">String</span></span>|<span data-ttu-id="efa21-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-336">Model of the device.</span></span> <span data-ttu-id="efa21-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-337">This property is read-only.</span></span> <span data-ttu-id="efa21-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="efa21-339">manufacturer</span></span>|<span data-ttu-id="efa21-340">String</span><span class="sxs-lookup"><span data-stu-id="efa21-340">String</span></span>|<span data-ttu-id="efa21-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-341">Manufacturer of the device.</span></span> <span data-ttu-id="efa21-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-342">This property is read-only.</span></span> <span data-ttu-id="efa21-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-344">imei</span><span class="sxs-lookup"><span data-stu-id="efa21-344">imei</span></span>|<span data-ttu-id="efa21-345">String</span><span class="sxs-lookup"><span data-stu-id="efa21-345">String</span></span>|<span data-ttu-id="efa21-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="efa21-346">IMEI.</span></span> <span data-ttu-id="efa21-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-347">This property is read-only.</span></span> <span data-ttu-id="efa21-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="efa21-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-350">DateTimeOffset</span></span>|<span data-ttu-id="efa21-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="efa21-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="efa21-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-352">This property is read-only.</span></span> <span data-ttu-id="efa21-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="efa21-354">serialNumber</span></span>|<span data-ttu-id="efa21-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa21-355">String</span></span>|<span data-ttu-id="efa21-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="efa21-356">SerialNumber.</span></span> <span data-ttu-id="efa21-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-357">This property is read-only.</span></span> <span data-ttu-id="efa21-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="efa21-359">phoneNumber</span></span>|<span data-ttu-id="efa21-360">String</span><span class="sxs-lookup"><span data-stu-id="efa21-360">String</span></span>|<span data-ttu-id="efa21-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-361">Phone number of the device.</span></span> <span data-ttu-id="efa21-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-362">This property is read-only.</span></span> <span data-ttu-id="efa21-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="efa21-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="efa21-365">String</span><span class="sxs-lookup"><span data-stu-id="efa21-365">String</span></span>|<span data-ttu-id="efa21-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="efa21-366">Android security patch level.</span></span> <span data-ttu-id="efa21-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-367">This property is read-only.</span></span> <span data-ttu-id="efa21-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="efa21-369">userDisplayName</span></span>|<span data-ttu-id="efa21-370">String</span><span class="sxs-lookup"><span data-stu-id="efa21-370">String</span></span>|<span data-ttu-id="efa21-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="efa21-371">User display name.</span></span> <span data-ttu-id="efa21-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-372">This property is read-only.</span></span> <span data-ttu-id="efa21-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="efa21-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="efa21-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="efa21-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="efa21-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="efa21-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="efa21-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-377">This property is read-only.</span></span> <span data-ttu-id="efa21-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="efa21-379">wiFiMacAddress</span></span>|<span data-ttu-id="efa21-380">String</span><span class="sxs-lookup"><span data-stu-id="efa21-380">String</span></span>|<span data-ttu-id="efa21-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="efa21-381">Wi-Fi MAC.</span></span> <span data-ttu-id="efa21-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-382">This property is read-only.</span></span> <span data-ttu-id="efa21-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="efa21-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="efa21-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="efa21-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="efa21-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-386">The device health attestation state.</span></span> <span data-ttu-id="efa21-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-387">This property is read-only.</span></span> <span data-ttu-id="efa21-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="efa21-389">subscriberCarrier</span></span>|<span data-ttu-id="efa21-390">String</span><span class="sxs-lookup"><span data-stu-id="efa21-390">String</span></span>|<span data-ttu-id="efa21-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="efa21-391">Subscriber Carrier.</span></span> <span data-ttu-id="efa21-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-392">This property is read-only.</span></span> <span data-ttu-id="efa21-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-394">meid</span><span class="sxs-lookup"><span data-stu-id="efa21-394">meid</span></span>|<span data-ttu-id="efa21-395">String</span><span class="sxs-lookup"><span data-stu-id="efa21-395">String</span></span>|<span data-ttu-id="efa21-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="efa21-396">MEID.</span></span> <span data-ttu-id="efa21-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-397">This property is read-only.</span></span> <span data-ttu-id="efa21-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="efa21-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="efa21-400">Int64</span><span class="sxs-lookup"><span data-stu-id="efa21-400">Int64</span></span>|<span data-ttu-id="efa21-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="efa21-401">Total Storage in Bytes.</span></span> <span data-ttu-id="efa21-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-402">This property is read-only.</span></span> <span data-ttu-id="efa21-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="efa21-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="efa21-405">Int64</span><span class="sxs-lookup"><span data-stu-id="efa21-405">Int64</span></span>|<span data-ttu-id="efa21-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="efa21-406">Free Storage in Bytes.</span></span> <span data-ttu-id="efa21-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-407">This property is read-only.</span></span> <span data-ttu-id="efa21-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="efa21-409">managedDeviceName</span></span>|<span data-ttu-id="efa21-410">String</span><span class="sxs-lookup"><span data-stu-id="efa21-410">String</span></span>|<span data-ttu-id="efa21-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="efa21-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="efa21-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="efa21-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="efa21-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="efa21-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="efa21-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="efa21-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="efa21-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-417">Read Only.</span></span> <span data-ttu-id="efa21-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-418">This property is read-only.</span></span> <span data-ttu-id="efa21-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="efa21-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="efa21-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-421">retireAfterDateTime</span></span>|<span data-ttu-id="efa21-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-422">DateTimeOffset</span></span>|<span data-ttu-id="efa21-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="efa21-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="efa21-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-424">This property is read-only.</span></span> <span data-ttu-id="efa21-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="efa21-426">usersLoggedOn</span></span>|<span data-ttu-id="efa21-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="efa21-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="efa21-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-429">This property is read-only.</span></span> <span data-ttu-id="efa21-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="efa21-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="efa21-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-432">DateTimeOffset</span></span>|<span data-ttu-id="efa21-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="efa21-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="efa21-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="efa21-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="efa21-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-435">Read Only.</span></span> <span data-ttu-id="efa21-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-436">This property is read-only.</span></span> <span data-ttu-id="efa21-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="efa21-438">autopilotEnrolled</span></span>|<span data-ttu-id="efa21-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-439">Boolean</span></span>|<span data-ttu-id="efa21-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="efa21-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="efa21-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-441">This property is read-only.</span></span> <span data-ttu-id="efa21-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="efa21-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="efa21-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="efa21-444">Boolean</span></span>|<span data-ttu-id="efa21-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="efa21-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="efa21-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-446">This property is read-only.</span></span> <span data-ttu-id="efa21-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="efa21-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="efa21-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efa21-449">DateTimeOffset</span></span>|<span data-ttu-id="efa21-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="efa21-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="efa21-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-451">This property is read-only.</span></span> <span data-ttu-id="efa21-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-453">iccid</span><span class="sxs-lookup"><span data-stu-id="efa21-453">iccid</span></span>|<span data-ttu-id="efa21-454">String</span><span class="sxs-lookup"><span data-stu-id="efa21-454">String</span></span>|<span data-ttu-id="efa21-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="efa21-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="efa21-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-456">This property is read-only.</span></span> <span data-ttu-id="efa21-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-458">udid</span><span class="sxs-lookup"><span data-stu-id="efa21-458">udid</span></span>|<span data-ttu-id="efa21-459">String</span><span class="sxs-lookup"><span data-stu-id="efa21-459">String</span></span>|<span data-ttu-id="efa21-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="efa21-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="efa21-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-461">This property is read-only.</span></span> <span data-ttu-id="efa21-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efa21-463">roleScopeTagIds</span></span>|<span data-ttu-id="efa21-464">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="efa21-464">String collection</span></span>|<span data-ttu-id="efa21-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efa21-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="efa21-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="efa21-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="efa21-468">Int32</span><span class="sxs-lookup"><span data-stu-id="efa21-468">Int32</span></span>|<span data-ttu-id="efa21-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="efa21-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="efa21-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-470">This property is read-only.</span></span> <span data-ttu-id="efa21-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="efa21-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="efa21-473">Int32</span><span class="sxs-lookup"><span data-stu-id="efa21-473">Int32</span></span>|<span data-ttu-id="efa21-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="efa21-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="efa21-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-475">This property is read-only.</span></span> <span data-ttu-id="efa21-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-477">notes</span><span class="sxs-lookup"><span data-stu-id="efa21-477">notes</span></span>|<span data-ttu-id="efa21-478">String</span><span class="sxs-lookup"><span data-stu-id="efa21-478">String</span></span>|<span data-ttu-id="efa21-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="efa21-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="efa21-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="efa21-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="efa21-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="efa21-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="efa21-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="efa21-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="efa21-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="efa21-486">ethernetMacAddress</span></span>|<span data-ttu-id="efa21-487">String</span><span class="sxs-lookup"><span data-stu-id="efa21-487">String</span></span>|<span data-ttu-id="efa21-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="efa21-488">Ethernet MAC.</span></span> <span data-ttu-id="efa21-489">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-489">This property is read-only.</span></span> <span data-ttu-id="efa21-490">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-491">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="efa21-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="efa21-492">Int64</span><span class="sxs-lookup"><span data-stu-id="efa21-492">Int64</span></span>|<span data-ttu-id="efa21-493">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="efa21-493">Total Memory in Bytes.</span></span> <span data-ttu-id="efa21-494">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-494">This property is read-only.</span></span> <span data-ttu-id="efa21-495">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="efa21-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="efa21-496">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="efa21-496">processorArchitecture</span></span>|[<span data-ttu-id="efa21-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="efa21-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="efa21-498">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="efa21-498">Processor architecture.</span></span> <span data-ttu-id="efa21-499">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efa21-499">This property is read-only.</span></span> <span data-ttu-id="efa21-500">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="efa21-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="efa21-501">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="efa21-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="efa21-502">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa21-502">Response</span></span>
<span data-ttu-id="efa21-503">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efa21-503">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efa21-504">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efa21-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="efa21-505">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efa21-505">Request</span></span>
<span data-ttu-id="efa21-506">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efa21-506">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 7665

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
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```

### <a name="response"></a><span data-ttu-id="efa21-507">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa21-507">Response</span></span>
<span data-ttu-id="efa21-p171">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efa21-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7714

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
    "clientIdentifier": "Client Identifier value",
    "isBlocked": true
  },
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5,
  "processorArchitecture": "x86"
}
```




