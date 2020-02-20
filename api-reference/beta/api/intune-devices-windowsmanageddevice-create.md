---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54529818fe408a4ded8109ae533f13c5c53c1a95
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161847"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="f9d13-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="f9d13-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="f9d13-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9d13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9d13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9d13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9d13-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="f9d13-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9d13-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9d13-107">Prerequisites</span></span>
<span data-ttu-id="f9d13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9d13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9d13-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9d13-110">Permission type</span></span>|<span data-ttu-id="f9d13-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9d13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9d13-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9d13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9d13-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d13-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9d13-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9d13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9d13-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9d13-115">Not supported.</span></span>|
|<span data-ttu-id="f9d13-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9d13-116">Application</span></span>|<span data-ttu-id="f9d13-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d13-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9d13-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9d13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="f9d13-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9d13-119">Request headers</span></span>
|<span data-ttu-id="f9d13-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9d13-120">Header</span></span>|<span data-ttu-id="f9d13-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9d13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9d13-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9d13-122">Authorization</span></span>|<span data-ttu-id="f9d13-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9d13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9d13-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9d13-124">Accept</span></span>|<span data-ttu-id="f9d13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9d13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9d13-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9d13-126">Request body</span></span>
<span data-ttu-id="f9d13-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="f9d13-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="f9d13-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="f9d13-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="f9d13-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9d13-129">Property</span></span>|<span data-ttu-id="f9d13-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9d13-130">Type</span></span>|<span data-ttu-id="f9d13-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9d13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9d13-132">id</span><span class="sxs-lookup"><span data-stu-id="f9d13-132">id</span></span>|<span data-ttu-id="f9d13-133">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-133">String</span></span>|<span data-ttu-id="f9d13-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-134">Unique Identifier for the device.</span></span> <span data-ttu-id="f9d13-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-135">This property is read-only.</span></span> <span data-ttu-id="f9d13-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-137">userId</span><span class="sxs-lookup"><span data-stu-id="f9d13-137">userId</span></span>|<span data-ttu-id="f9d13-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9d13-138">String</span></span>|<span data-ttu-id="f9d13-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="f9d13-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-140">This property is read-only.</span></span> <span data-ttu-id="f9d13-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="f9d13-142">deviceName</span></span>|<span data-ttu-id="f9d13-143">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-143">String</span></span>|<span data-ttu-id="f9d13-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-144">Name of the device.</span></span> <span data-ttu-id="f9d13-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-145">This property is read-only.</span></span> <span data-ttu-id="f9d13-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f9d13-147">hardwareInformation</span></span>|[<span data-ttu-id="f9d13-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f9d13-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="f9d13-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-149">The hardward details for the device.</span></span>  <span data-ttu-id="f9d13-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="f9d13-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="f9d13-152">ownerType</span></span>|[<span data-ttu-id="f9d13-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="f9d13-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="f9d13-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-154">Ownership of the device.</span></span> <span data-ttu-id="f9d13-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f9d13-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f9d13-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="f9d13-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f9d13-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="f9d13-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-159">Ownership of the device.</span></span> <span data-ttu-id="f9d13-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f9d13-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="f9d13-162">deviceActionResults</span></span>|<span data-ttu-id="f9d13-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="f9d13-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="f9d13-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="f9d13-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-165">This property is read-only.</span></span> <span data-ttu-id="f9d13-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="f9d13-167">managementState</span></span>|[<span data-ttu-id="f9d13-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="f9d13-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="f9d13-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-169">Management state of the device.</span></span> <span data-ttu-id="f9d13-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-170">This property is read-only.</span></span> <span data-ttu-id="f9d13-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="f9d13-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-173">enrolledDateTime</span></span>|<span data-ttu-id="f9d13-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-174">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-175">Enrollment time of the device.</span></span> <span data-ttu-id="f9d13-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-176">This property is read-only.</span></span> <span data-ttu-id="f9d13-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-178">lastSyncDateTime</span></span>|<span data-ttu-id="f9d13-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-179">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="f9d13-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="f9d13-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-181">This property is read-only.</span></span> <span data-ttu-id="f9d13-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="f9d13-183">chassisType</span></span>|[<span data-ttu-id="f9d13-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="f9d13-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="f9d13-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-185">Chassis type of the device.</span></span> <span data-ttu-id="f9d13-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-186">This property is read-only.</span></span> <span data-ttu-id="f9d13-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="f9d13-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f9d13-189">operatingSystem</span></span>|<span data-ttu-id="f9d13-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9d13-190">String</span></span>|<span data-ttu-id="f9d13-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-191">Operating system of the device.</span></span> <span data-ttu-id="f9d13-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="f9d13-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="f9d13-194">deviceType</span></span>|[<span data-ttu-id="f9d13-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="f9d13-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f9d13-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-196">Platform of the device.</span></span> <span data-ttu-id="f9d13-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-197">This property is read-only.</span></span> <span data-ttu-id="f9d13-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="f9d13-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f9d13-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="f9d13-200">complianceState</span></span>|[<span data-ttu-id="f9d13-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="f9d13-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="f9d13-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-202">Compliance state of the device.</span></span> <span data-ttu-id="f9d13-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-203">This property is read-only.</span></span> <span data-ttu-id="f9d13-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="f9d13-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="f9d13-206">jailBroken</span></span>|<span data-ttu-id="f9d13-207">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-207">String</span></span>|<span data-ttu-id="f9d13-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="f9d13-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="f9d13-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-209">This property is read-only.</span></span> <span data-ttu-id="f9d13-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="f9d13-211">managementAgent</span></span>|[<span data-ttu-id="f9d13-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="f9d13-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="f9d13-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-213">Management channel of the device.</span></span> <span data-ttu-id="f9d13-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="f9d13-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="f9d13-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="f9d13-217">osVersion</span></span>|<span data-ttu-id="f9d13-218">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-218">String</span></span>|<span data-ttu-id="f9d13-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-219">Operating system version of the device.</span></span> <span data-ttu-id="f9d13-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-220">This property is read-only.</span></span> <span data-ttu-id="f9d13-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="f9d13-222">easActivated</span></span>|<span data-ttu-id="f9d13-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d13-223">Boolean</span></span>|<span data-ttu-id="f9d13-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f9d13-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="f9d13-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-225">This property is read-only.</span></span> <span data-ttu-id="f9d13-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="f9d13-227">easDeviceId</span></span>|<span data-ttu-id="f9d13-228">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-228">String</span></span>|<span data-ttu-id="f9d13-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="f9d13-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-230">This property is read-only.</span></span> <span data-ttu-id="f9d13-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-232">easActivationDateTime</span></span>|<span data-ttu-id="f9d13-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-233">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="f9d13-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-235">This property is read-only.</span></span> <span data-ttu-id="f9d13-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="f9d13-237">aadRegistered</span></span>|<span data-ttu-id="f9d13-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d13-238">Boolean</span></span>|<span data-ttu-id="f9d13-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9d13-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="f9d13-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-240">This property is read-only.</span></span> <span data-ttu-id="f9d13-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="f9d13-242">azureADRegistered</span></span>|<span data-ttu-id="f9d13-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d13-243">Boolean</span></span>|<span data-ttu-id="f9d13-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9d13-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="f9d13-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-245">This property is read-only.</span></span> <span data-ttu-id="f9d13-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f9d13-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="f9d13-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f9d13-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f9d13-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-249">Enrollment type of the device.</span></span> <span data-ttu-id="f9d13-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-250">This property is read-only.</span></span> <span data-ttu-id="f9d13-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="f9d13-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f9d13-253">lostModeState</span></span>|[<span data-ttu-id="f9d13-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f9d13-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="f9d13-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f9d13-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="f9d13-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-256">This property is read-only.</span></span> <span data-ttu-id="f9d13-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f9d13-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="f9d13-259">activationLockBypassCode</span></span>|<span data-ttu-id="f9d13-260">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-260">String</span></span>|<span data-ttu-id="f9d13-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="f9d13-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="f9d13-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-262">This property is read-only.</span></span> <span data-ttu-id="f9d13-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f9d13-264">emailAddress</span></span>|<span data-ttu-id="f9d13-265">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-265">String</span></span>|<span data-ttu-id="f9d13-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="f9d13-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-267">This property is read-only.</span></span> <span data-ttu-id="f9d13-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="f9d13-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f9d13-270">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-270">String</span></span>|<span data-ttu-id="f9d13-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9d13-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f9d13-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-272">Read only.</span></span> <span data-ttu-id="f9d13-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-273">This property is read-only.</span></span> <span data-ttu-id="f9d13-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f9d13-275">azureADDeviceId</span></span>|<span data-ttu-id="f9d13-276">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-276">String</span></span>|<span data-ttu-id="f9d13-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9d13-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f9d13-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-278">Read only.</span></span> <span data-ttu-id="f9d13-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-279">This property is read-only.</span></span> <span data-ttu-id="f9d13-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f9d13-281">deviceRegistrationState</span></span>|[<span data-ttu-id="f9d13-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f9d13-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="f9d13-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-283">Device registration state.</span></span> <span data-ttu-id="f9d13-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-284">This property is read-only.</span></span> <span data-ttu-id="f9d13-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="f9d13-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9d13-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="f9d13-288">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-288">String</span></span>|<span data-ttu-id="f9d13-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-289">Device category display name.</span></span> <span data-ttu-id="f9d13-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-290">This property is read-only.</span></span> <span data-ttu-id="f9d13-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f9d13-292">isSupervised</span></span>|<span data-ttu-id="f9d13-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d13-293">Boolean</span></span>|<span data-ttu-id="f9d13-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-294">Device supervised status.</span></span> <span data-ttu-id="f9d13-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-295">This property is read-only.</span></span> <span data-ttu-id="f9d13-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f9d13-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-298">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9d13-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="f9d13-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-300">This property is read-only.</span></span> <span data-ttu-id="f9d13-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f9d13-302">exchangeAccessState</span></span>|[<span data-ttu-id="f9d13-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f9d13-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="f9d13-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9d13-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="f9d13-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-305">This property is read-only.</span></span> <span data-ttu-id="f9d13-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="f9d13-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f9d13-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="f9d13-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f9d13-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="f9d13-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9d13-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="f9d13-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-311">This property is read-only.</span></span> <span data-ttu-id="f9d13-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="f9d13-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="f9d13-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="f9d13-315">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-315">String</span></span>|<span data-ttu-id="f9d13-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="f9d13-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-317">This property is read-only.</span></span> <span data-ttu-id="f9d13-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f9d13-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="f9d13-320">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-320">String</span></span>|<span data-ttu-id="f9d13-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="f9d13-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="f9d13-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-322">This property is read-only.</span></span> <span data-ttu-id="f9d13-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f9d13-324">isEncrypted</span></span>|<span data-ttu-id="f9d13-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d13-325">Boolean</span></span>|<span data-ttu-id="f9d13-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-326">Device encryption status.</span></span> <span data-ttu-id="f9d13-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-327">This property is read-only.</span></span> <span data-ttu-id="f9d13-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9d13-329">userPrincipalName</span></span>|<span data-ttu-id="f9d13-330">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-330">String</span></span>|<span data-ttu-id="f9d13-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-331">Device user principal name.</span></span> <span data-ttu-id="f9d13-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-332">This property is read-only.</span></span> <span data-ttu-id="f9d13-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-334">modelo</span><span class="sxs-lookup"><span data-stu-id="f9d13-334">model</span></span>|<span data-ttu-id="f9d13-335">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-335">String</span></span>|<span data-ttu-id="f9d13-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-336">Model of the device.</span></span> <span data-ttu-id="f9d13-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-337">This property is read-only.</span></span> <span data-ttu-id="f9d13-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="f9d13-339">manufacturer</span></span>|<span data-ttu-id="f9d13-340">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-340">String</span></span>|<span data-ttu-id="f9d13-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-341">Manufacturer of the device.</span></span> <span data-ttu-id="f9d13-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-342">This property is read-only.</span></span> <span data-ttu-id="f9d13-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-344">imei</span><span class="sxs-lookup"><span data-stu-id="f9d13-344">imei</span></span>|<span data-ttu-id="f9d13-345">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-345">String</span></span>|<span data-ttu-id="f9d13-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="f9d13-346">IMEI.</span></span> <span data-ttu-id="f9d13-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-347">This property is read-only.</span></span> <span data-ttu-id="f9d13-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f9d13-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-350">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="f9d13-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="f9d13-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-352">This property is read-only.</span></span> <span data-ttu-id="f9d13-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f9d13-354">serialNumber</span></span>|<span data-ttu-id="f9d13-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9d13-355">String</span></span>|<span data-ttu-id="f9d13-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="f9d13-356">SerialNumber.</span></span> <span data-ttu-id="f9d13-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-357">This property is read-only.</span></span> <span data-ttu-id="f9d13-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f9d13-359">phoneNumber</span></span>|<span data-ttu-id="f9d13-360">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-360">String</span></span>|<span data-ttu-id="f9d13-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-361">Phone number of the device.</span></span> <span data-ttu-id="f9d13-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-362">This property is read-only.</span></span> <span data-ttu-id="f9d13-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f9d13-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="f9d13-365">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-365">String</span></span>|<span data-ttu-id="f9d13-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="f9d13-366">Android security patch level.</span></span> <span data-ttu-id="f9d13-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-367">This property is read-only.</span></span> <span data-ttu-id="f9d13-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9d13-369">userDisplayName</span></span>|<span data-ttu-id="f9d13-370">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-370">String</span></span>|<span data-ttu-id="f9d13-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9d13-371">User display name.</span></span> <span data-ttu-id="f9d13-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-372">This property is read-only.</span></span> <span data-ttu-id="f9d13-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f9d13-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="f9d13-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f9d13-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="f9d13-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="f9d13-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="f9d13-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-377">This property is read-only.</span></span> <span data-ttu-id="f9d13-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="f9d13-379">wiFiMacAddress</span></span>|<span data-ttu-id="f9d13-380">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-380">String</span></span>|<span data-ttu-id="f9d13-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f9d13-381">Wi-Fi MAC.</span></span> <span data-ttu-id="f9d13-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-382">This property is read-only.</span></span> <span data-ttu-id="f9d13-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f9d13-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="f9d13-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f9d13-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="f9d13-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-386">The device health attestation state.</span></span> <span data-ttu-id="f9d13-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-387">This property is read-only.</span></span> <span data-ttu-id="f9d13-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f9d13-389">subscriberCarrier</span></span>|<span data-ttu-id="f9d13-390">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-390">String</span></span>|<span data-ttu-id="f9d13-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="f9d13-391">Subscriber Carrier.</span></span> <span data-ttu-id="f9d13-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-392">This property is read-only.</span></span> <span data-ttu-id="f9d13-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-394">meid</span><span class="sxs-lookup"><span data-stu-id="f9d13-394">meid</span></span>|<span data-ttu-id="f9d13-395">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-395">String</span></span>|<span data-ttu-id="f9d13-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="f9d13-396">MEID.</span></span> <span data-ttu-id="f9d13-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-397">This property is read-only.</span></span> <span data-ttu-id="f9d13-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f9d13-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="f9d13-400">Int64</span><span class="sxs-lookup"><span data-stu-id="f9d13-400">Int64</span></span>|<span data-ttu-id="f9d13-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="f9d13-401">Total Storage in Bytes.</span></span> <span data-ttu-id="f9d13-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-402">This property is read-only.</span></span> <span data-ttu-id="f9d13-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f9d13-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="f9d13-405">Int64</span><span class="sxs-lookup"><span data-stu-id="f9d13-405">Int64</span></span>|<span data-ttu-id="f9d13-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="f9d13-406">Free Storage in Bytes.</span></span> <span data-ttu-id="f9d13-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-407">This property is read-only.</span></span> <span data-ttu-id="f9d13-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f9d13-409">managedDeviceName</span></span>|<span data-ttu-id="f9d13-410">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-410">String</span></span>|<span data-ttu-id="f9d13-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="f9d13-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f9d13-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="f9d13-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="f9d13-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="f9d13-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="f9d13-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="f9d13-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="f9d13-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-417">Read Only.</span></span> <span data-ttu-id="f9d13-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-418">This property is read-only.</span></span> <span data-ttu-id="f9d13-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="f9d13-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-421">retireAfterDateTime</span></span>|<span data-ttu-id="f9d13-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-422">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="f9d13-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="f9d13-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-424">This property is read-only.</span></span> <span data-ttu-id="f9d13-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="f9d13-426">usersLoggedOn</span></span>|<span data-ttu-id="f9d13-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="f9d13-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="f9d13-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-429">This property is read-only.</span></span> <span data-ttu-id="f9d13-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d13-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="f9d13-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-432">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="f9d13-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="f9d13-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="f9d13-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="f9d13-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-435">Read Only.</span></span> <span data-ttu-id="f9d13-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-436">This property is read-only.</span></span> <span data-ttu-id="f9d13-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="f9d13-438">autopilotEnrolled</span></span>|<span data-ttu-id="f9d13-439">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d13-439">Boolean</span></span>|<span data-ttu-id="f9d13-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="f9d13-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="f9d13-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-441">This property is read-only.</span></span> <span data-ttu-id="f9d13-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="f9d13-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="f9d13-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d13-444">Boolean</span></span>|<span data-ttu-id="f9d13-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9d13-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="f9d13-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-446">This property is read-only.</span></span> <span data-ttu-id="f9d13-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="f9d13-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="f9d13-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d13-449">DateTimeOffset</span></span>|<span data-ttu-id="f9d13-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f9d13-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="f9d13-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-451">This property is read-only.</span></span> <span data-ttu-id="f9d13-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-453">iccid</span><span class="sxs-lookup"><span data-stu-id="f9d13-453">iccid</span></span>|<span data-ttu-id="f9d13-454">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-454">String</span></span>|<span data-ttu-id="f9d13-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="f9d13-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="f9d13-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-456">This property is read-only.</span></span> <span data-ttu-id="f9d13-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-458">udid</span><span class="sxs-lookup"><span data-stu-id="f9d13-458">udid</span></span>|<span data-ttu-id="f9d13-459">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-459">String</span></span>|<span data-ttu-id="f9d13-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="f9d13-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="f9d13-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-461">This property is read-only.</span></span> <span data-ttu-id="f9d13-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9d13-463">roleScopeTagIds</span></span>|<span data-ttu-id="f9d13-464">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9d13-464">String collection</span></span>|<span data-ttu-id="f9d13-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9d13-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="f9d13-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f9d13-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="f9d13-468">Int32</span><span class="sxs-lookup"><span data-stu-id="f9d13-468">Int32</span></span>|<span data-ttu-id="f9d13-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="f9d13-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="f9d13-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-470">This property is read-only.</span></span> <span data-ttu-id="f9d13-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f9d13-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="f9d13-473">Int32</span><span class="sxs-lookup"><span data-stu-id="f9d13-473">Int32</span></span>|<span data-ttu-id="f9d13-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="f9d13-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="f9d13-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-475">This property is read-only.</span></span> <span data-ttu-id="f9d13-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-477">notes</span><span class="sxs-lookup"><span data-stu-id="f9d13-477">notes</span></span>|<span data-ttu-id="f9d13-478">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-478">String</span></span>|<span data-ttu-id="f9d13-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f9d13-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="f9d13-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f9d13-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="f9d13-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="f9d13-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="f9d13-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="f9d13-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="f9d13-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="f9d13-486">ethernetMacAddress</span></span>|<span data-ttu-id="f9d13-487">String</span><span class="sxs-lookup"><span data-stu-id="f9d13-487">String</span></span>|<span data-ttu-id="f9d13-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="f9d13-488">Ethernet MAC.</span></span> <span data-ttu-id="f9d13-489">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-489">This property is read-only.</span></span> <span data-ttu-id="f9d13-490">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-491">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="f9d13-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="f9d13-492">Int64</span><span class="sxs-lookup"><span data-stu-id="f9d13-492">Int64</span></span>|<span data-ttu-id="f9d13-493">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="f9d13-493">Total Memory in Bytes.</span></span> <span data-ttu-id="f9d13-494">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-494">This property is read-only.</span></span> <span data-ttu-id="f9d13-495">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="f9d13-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="f9d13-496">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="f9d13-496">processorArchitecture</span></span>|[<span data-ttu-id="f9d13-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="f9d13-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="f9d13-498">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="f9d13-498">Processor architecture.</span></span> <span data-ttu-id="f9d13-499">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9d13-499">This property is read-only.</span></span> <span data-ttu-id="f9d13-500">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9d13-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="f9d13-501">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="f9d13-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="f9d13-502">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9d13-502">Response</span></span>
<span data-ttu-id="f9d13-503">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9d13-503">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9d13-504">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9d13-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9d13-505">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9d13-505">Request</span></span>
<span data-ttu-id="f9d13-506">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9d13-506">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
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

### <a name="response"></a><span data-ttu-id="f9d13-507">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9d13-507">Response</span></span>
<span data-ttu-id="f9d13-p171">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9d13-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





