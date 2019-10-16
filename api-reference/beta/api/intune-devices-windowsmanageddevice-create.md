---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 422dcb587a6e63086f82aa137b652f0cb47bbba1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37526859"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="427c4-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="427c4-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="427c4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="427c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="427c4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="427c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="427c4-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="427c4-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="427c4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="427c4-107">Prerequisites</span></span>
<span data-ttu-id="427c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="427c4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="427c4-110">Permission type</span></span>|<span data-ttu-id="427c4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="427c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="427c4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="427c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="427c4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427c4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="427c4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="427c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="427c4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="427c4-115">Not supported.</span></span>|
|<span data-ttu-id="427c4-116">Application</span><span class="sxs-lookup"><span data-stu-id="427c4-116">Application</span></span>|<span data-ttu-id="427c4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427c4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="427c4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="427c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="427c4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="427c4-119">Request headers</span></span>
|<span data-ttu-id="427c4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="427c4-120">Header</span></span>|<span data-ttu-id="427c4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="427c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="427c4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="427c4-122">Authorization</span></span>|<span data-ttu-id="427c4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="427c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="427c4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="427c4-124">Accept</span></span>|<span data-ttu-id="427c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="427c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="427c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="427c4-126">Request body</span></span>
<span data-ttu-id="427c4-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="427c4-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="427c4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="427c4-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="427c4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="427c4-129">Property</span></span>|<span data-ttu-id="427c4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="427c4-130">Type</span></span>|<span data-ttu-id="427c4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="427c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="427c4-132">id</span><span class="sxs-lookup"><span data-stu-id="427c4-132">id</span></span>|<span data-ttu-id="427c4-133">String</span><span class="sxs-lookup"><span data-stu-id="427c4-133">String</span></span>|<span data-ttu-id="427c4-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-134">Unique Identifier for the device.</span></span> <span data-ttu-id="427c4-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-135">This property is read-only.</span></span> <span data-ttu-id="427c4-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-137">userId</span><span class="sxs-lookup"><span data-stu-id="427c4-137">userId</span></span>|<span data-ttu-id="427c4-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-138">String</span></span>|<span data-ttu-id="427c4-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="427c4-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-140">This property is read-only.</span></span> <span data-ttu-id="427c4-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="427c4-142">deviceName</span></span>|<span data-ttu-id="427c4-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-143">String</span></span>|<span data-ttu-id="427c4-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-144">Name of the device.</span></span> <span data-ttu-id="427c4-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-145">This property is read-only.</span></span> <span data-ttu-id="427c4-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="427c4-147">hardwareInformation</span></span>|[<span data-ttu-id="427c4-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="427c4-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="427c4-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-149">The hardward details for the device.</span></span>  <span data-ttu-id="427c4-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="427c4-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="427c4-152">ownerType</span></span>|[<span data-ttu-id="427c4-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="427c4-153">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="427c4-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-154">Ownership of the device.</span></span> <span data-ttu-id="427c4-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="427c4-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="427c4-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="427c4-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="427c4-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="427c4-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="427c4-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-159">Ownership of the device.</span></span> <span data-ttu-id="427c4-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="427c4-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="427c4-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="427c4-162">deviceActionResults</span></span>|<span data-ttu-id="427c4-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="427c4-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="427c4-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="427c4-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-165">This property is read-only.</span></span> <span data-ttu-id="427c4-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="427c4-167">managementState</span></span>|[<span data-ttu-id="427c4-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="427c4-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="427c4-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-169">Management state of the device.</span></span> <span data-ttu-id="427c4-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-170">This property is read-only.</span></span> <span data-ttu-id="427c4-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="427c4-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="427c4-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-173">enrolledDateTime</span></span>|<span data-ttu-id="427c4-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-174">DateTimeOffset</span></span>|<span data-ttu-id="427c4-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-175">Enrollment time of the device.</span></span> <span data-ttu-id="427c4-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-176">This property is read-only.</span></span> <span data-ttu-id="427c4-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-178">lastSyncDateTime</span></span>|<span data-ttu-id="427c4-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-179">DateTimeOffset</span></span>|<span data-ttu-id="427c4-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="427c4-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="427c4-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-181">This property is read-only.</span></span> <span data-ttu-id="427c4-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="427c4-183">chassisType</span></span>|[<span data-ttu-id="427c4-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="427c4-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="427c4-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-185">Chassis type of the device.</span></span> <span data-ttu-id="427c4-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-186">This property is read-only.</span></span> <span data-ttu-id="427c4-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="427c4-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="427c4-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="427c4-189">operatingSystem</span></span>|<span data-ttu-id="427c4-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-190">String</span></span>|<span data-ttu-id="427c4-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-191">Operating system of the device.</span></span> <span data-ttu-id="427c4-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="427c4-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="427c4-194">deviceType</span></span>|[<span data-ttu-id="427c4-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="427c4-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="427c4-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-196">Platform of the device.</span></span> <span data-ttu-id="427c4-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-197">This property is read-only.</span></span> <span data-ttu-id="427c4-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="427c4-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="427c4-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="427c4-200">complianceState</span></span>|[<span data-ttu-id="427c4-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="427c4-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="427c4-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-202">Compliance state of the device.</span></span> <span data-ttu-id="427c4-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-203">This property is read-only.</span></span> <span data-ttu-id="427c4-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="427c4-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="427c4-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="427c4-206">jailBroken</span></span>|<span data-ttu-id="427c4-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-207">String</span></span>|<span data-ttu-id="427c4-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="427c4-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="427c4-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-209">This property is read-only.</span></span> <span data-ttu-id="427c4-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="427c4-211">managementAgent</span></span>|[<span data-ttu-id="427c4-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="427c4-212">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="427c4-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-213">Management channel of the device.</span></span> <span data-ttu-id="427c4-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="427c4-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="427c4-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="427c4-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="427c4-217">osVersion</span></span>|<span data-ttu-id="427c4-218">String</span><span class="sxs-lookup"><span data-stu-id="427c4-218">String</span></span>|<span data-ttu-id="427c4-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-219">Operating system version of the device.</span></span> <span data-ttu-id="427c4-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-220">This property is read-only.</span></span> <span data-ttu-id="427c4-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="427c4-222">easActivated</span></span>|<span data-ttu-id="427c4-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="427c4-223">Boolean</span></span>|<span data-ttu-id="427c4-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="427c4-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="427c4-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-225">This property is read-only.</span></span> <span data-ttu-id="427c4-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="427c4-227">easDeviceId</span></span>|<span data-ttu-id="427c4-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-228">String</span></span>|<span data-ttu-id="427c4-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="427c4-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-230">This property is read-only.</span></span> <span data-ttu-id="427c4-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-232">easActivationDateTime</span></span>|<span data-ttu-id="427c4-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-233">DateTimeOffset</span></span>|<span data-ttu-id="427c4-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="427c4-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-235">This property is read-only.</span></span> <span data-ttu-id="427c4-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="427c4-237">aadRegistered</span></span>|<span data-ttu-id="427c4-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="427c4-238">Boolean</span></span>|<span data-ttu-id="427c4-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="427c4-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="427c4-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-240">This property is read-only.</span></span> <span data-ttu-id="427c4-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="427c4-242">azureADRegistered</span></span>|<span data-ttu-id="427c4-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="427c4-243">Boolean</span></span>|<span data-ttu-id="427c4-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="427c4-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="427c4-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-245">This property is read-only.</span></span> <span data-ttu-id="427c4-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="427c4-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="427c4-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="427c4-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="427c4-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-249">Enrollment type of the device.</span></span> <span data-ttu-id="427c4-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-250">This property is read-only.</span></span> <span data-ttu-id="427c4-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="427c4-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="427c4-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="427c4-253">lostModeState</span></span>|[<span data-ttu-id="427c4-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="427c4-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="427c4-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="427c4-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="427c4-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-256">This property is read-only.</span></span> <span data-ttu-id="427c4-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="427c4-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="427c4-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="427c4-259">activationLockBypassCode</span></span>|<span data-ttu-id="427c4-260">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-260">String</span></span>|<span data-ttu-id="427c4-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="427c4-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="427c4-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-262">This property is read-only.</span></span> <span data-ttu-id="427c4-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="427c4-264">emailAddress</span></span>|<span data-ttu-id="427c4-265">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-265">String</span></span>|<span data-ttu-id="427c4-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="427c4-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-267">This property is read-only.</span></span> <span data-ttu-id="427c4-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="427c4-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="427c4-270">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-270">String</span></span>|<span data-ttu-id="427c4-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="427c4-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="427c4-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-272">Read only.</span></span> <span data-ttu-id="427c4-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-273">This property is read-only.</span></span> <span data-ttu-id="427c4-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="427c4-275">azureADDeviceId</span></span>|<span data-ttu-id="427c4-276">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-276">String</span></span>|<span data-ttu-id="427c4-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="427c4-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="427c4-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-278">Read only.</span></span> <span data-ttu-id="427c4-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-279">This property is read-only.</span></span> <span data-ttu-id="427c4-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="427c4-281">deviceRegistrationState</span></span>|[<span data-ttu-id="427c4-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="427c4-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="427c4-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-283">Device registration state.</span></span> <span data-ttu-id="427c4-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-284">This property is read-only.</span></span> <span data-ttu-id="427c4-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="427c4-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="427c4-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="427c4-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="427c4-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-288">String</span></span>|<span data-ttu-id="427c4-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-289">Device category display name.</span></span> <span data-ttu-id="427c4-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-290">This property is read-only.</span></span> <span data-ttu-id="427c4-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="427c4-292">isSupervised</span></span>|<span data-ttu-id="427c4-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="427c4-293">Boolean</span></span>|<span data-ttu-id="427c4-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-294">Device supervised status.</span></span> <span data-ttu-id="427c4-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-295">This property is read-only.</span></span> <span data-ttu-id="427c4-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="427c4-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-298">DateTimeOffset</span></span>|<span data-ttu-id="427c4-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="427c4-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="427c4-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-300">This property is read-only.</span></span> <span data-ttu-id="427c4-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="427c4-302">exchangeAccessState</span></span>|[<span data-ttu-id="427c4-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="427c4-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="427c4-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="427c4-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="427c4-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-305">This property is read-only.</span></span> <span data-ttu-id="427c4-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="427c4-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="427c4-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="427c4-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="427c4-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="427c4-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="427c4-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="427c4-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="427c4-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-311">This property is read-only.</span></span> <span data-ttu-id="427c4-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="427c4-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="427c4-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="427c4-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="427c4-315">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-315">String</span></span>|<span data-ttu-id="427c4-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="427c4-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-317">This property is read-only.</span></span> <span data-ttu-id="427c4-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="427c4-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="427c4-320">String</span><span class="sxs-lookup"><span data-stu-id="427c4-320">String</span></span>|<span data-ttu-id="427c4-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="427c4-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="427c4-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-322">This property is read-only.</span></span> <span data-ttu-id="427c4-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="427c4-324">isEncrypted</span></span>|<span data-ttu-id="427c4-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="427c4-325">Boolean</span></span>|<span data-ttu-id="427c4-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-326">Device encryption status.</span></span> <span data-ttu-id="427c4-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-327">This property is read-only.</span></span> <span data-ttu-id="427c4-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="427c4-329">userPrincipalName</span></span>|<span data-ttu-id="427c4-330">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-330">String</span></span>|<span data-ttu-id="427c4-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-331">Device user principal name.</span></span> <span data-ttu-id="427c4-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-332">This property is read-only.</span></span> <span data-ttu-id="427c4-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-334">modelo</span><span class="sxs-lookup"><span data-stu-id="427c4-334">model</span></span>|<span data-ttu-id="427c4-335">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-335">String</span></span>|<span data-ttu-id="427c4-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-336">Model of the device.</span></span> <span data-ttu-id="427c4-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-337">This property is read-only.</span></span> <span data-ttu-id="427c4-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="427c4-339">manufacturer</span></span>|<span data-ttu-id="427c4-340">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-340">String</span></span>|<span data-ttu-id="427c4-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-341">Manufacturer of the device.</span></span> <span data-ttu-id="427c4-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-342">This property is read-only.</span></span> <span data-ttu-id="427c4-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-344">imei</span><span class="sxs-lookup"><span data-stu-id="427c4-344">imei</span></span>|<span data-ttu-id="427c4-345">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-345">String</span></span>|<span data-ttu-id="427c4-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="427c4-346">IMEI.</span></span> <span data-ttu-id="427c4-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-347">This property is read-only.</span></span> <span data-ttu-id="427c4-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="427c4-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-350">DateTimeOffset</span></span>|<span data-ttu-id="427c4-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="427c4-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="427c4-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-352">This property is read-only.</span></span> <span data-ttu-id="427c4-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="427c4-354">serialNumber</span></span>|<span data-ttu-id="427c4-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-355">String</span></span>|<span data-ttu-id="427c4-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="427c4-356">SerialNumber.</span></span> <span data-ttu-id="427c4-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-357">This property is read-only.</span></span> <span data-ttu-id="427c4-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="427c4-359">phoneNumber</span></span>|<span data-ttu-id="427c4-360">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-360">String</span></span>|<span data-ttu-id="427c4-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-361">Phone number of the device.</span></span> <span data-ttu-id="427c4-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-362">This property is read-only.</span></span> <span data-ttu-id="427c4-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="427c4-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="427c4-365">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-365">String</span></span>|<span data-ttu-id="427c4-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="427c4-366">Android security patch level.</span></span> <span data-ttu-id="427c4-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-367">This property is read-only.</span></span> <span data-ttu-id="427c4-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="427c4-369">userDisplayName</span></span>|<span data-ttu-id="427c4-370">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-370">String</span></span>|<span data-ttu-id="427c4-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="427c4-371">User display name.</span></span> <span data-ttu-id="427c4-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-372">This property is read-only.</span></span> <span data-ttu-id="427c4-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="427c4-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="427c4-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="427c4-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="427c4-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="427c4-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="427c4-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-377">This property is read-only.</span></span> <span data-ttu-id="427c4-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="427c4-379">wiFiMacAddress</span></span>|<span data-ttu-id="427c4-380">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-380">String</span></span>|<span data-ttu-id="427c4-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="427c4-381">Wi-Fi MAC.</span></span> <span data-ttu-id="427c4-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-382">This property is read-only.</span></span> <span data-ttu-id="427c4-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="427c4-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="427c4-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="427c4-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="427c4-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-386">The device health attestation state.</span></span> <span data-ttu-id="427c4-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-387">This property is read-only.</span></span> <span data-ttu-id="427c4-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="427c4-389">subscriberCarrier</span></span>|<span data-ttu-id="427c4-390">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-390">String</span></span>|<span data-ttu-id="427c4-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="427c4-391">Subscriber Carrier.</span></span> <span data-ttu-id="427c4-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-392">This property is read-only.</span></span> <span data-ttu-id="427c4-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-394">meid</span><span class="sxs-lookup"><span data-stu-id="427c4-394">meid</span></span>|<span data-ttu-id="427c4-395">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-395">String</span></span>|<span data-ttu-id="427c4-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="427c4-396">MEID.</span></span> <span data-ttu-id="427c4-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-397">This property is read-only.</span></span> <span data-ttu-id="427c4-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="427c4-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="427c4-400">Int64</span><span class="sxs-lookup"><span data-stu-id="427c4-400">Int64</span></span>|<span data-ttu-id="427c4-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="427c4-401">Total Storage in Bytes.</span></span> <span data-ttu-id="427c4-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-402">This property is read-only.</span></span> <span data-ttu-id="427c4-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="427c4-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="427c4-405">Int64</span><span class="sxs-lookup"><span data-stu-id="427c4-405">Int64</span></span>|<span data-ttu-id="427c4-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="427c4-406">Free Storage in Bytes.</span></span> <span data-ttu-id="427c4-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-407">This property is read-only.</span></span> <span data-ttu-id="427c4-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="427c4-409">managedDeviceName</span></span>|<span data-ttu-id="427c4-410">String</span><span class="sxs-lookup"><span data-stu-id="427c4-410">String</span></span>|<span data-ttu-id="427c4-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="427c4-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="427c4-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="427c4-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="427c4-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="427c4-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="427c4-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="427c4-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="427c4-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-417">Read Only.</span></span> <span data-ttu-id="427c4-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-418">This property is read-only.</span></span> <span data-ttu-id="427c4-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="427c4-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="427c4-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="427c4-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="427c4-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-421">retireAfterDateTime</span></span>|<span data-ttu-id="427c4-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-422">DateTimeOffset</span></span>|<span data-ttu-id="427c4-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="427c4-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="427c4-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-424">This property is read-only.</span></span> <span data-ttu-id="427c4-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="427c4-426">usersLoggedOn</span></span>|<span data-ttu-id="427c4-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="427c4-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="427c4-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-429">This property is read-only.</span></span> <span data-ttu-id="427c4-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="427c4-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="427c4-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-432">DateTimeOffset</span></span>|<span data-ttu-id="427c4-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="427c4-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="427c4-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="427c4-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="427c4-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-435">Read Only.</span></span> <span data-ttu-id="427c4-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-436">This property is read-only.</span></span> <span data-ttu-id="427c4-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="427c4-438">autopilotEnrolled</span></span>|<span data-ttu-id="427c4-439">Booliano</span><span class="sxs-lookup"><span data-stu-id="427c4-439">Boolean</span></span>|<span data-ttu-id="427c4-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="427c4-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="427c4-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-441">This property is read-only.</span></span> <span data-ttu-id="427c4-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="427c4-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="427c4-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="427c4-444">Boolean</span></span>|<span data-ttu-id="427c4-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="427c4-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="427c4-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-446">This property is read-only.</span></span> <span data-ttu-id="427c4-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="427c4-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="427c4-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="427c4-449">DateTimeOffset</span></span>|<span data-ttu-id="427c4-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="427c4-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="427c4-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-451">This property is read-only.</span></span> <span data-ttu-id="427c4-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-453">iccid</span><span class="sxs-lookup"><span data-stu-id="427c4-453">iccid</span></span>|<span data-ttu-id="427c4-454">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-454">String</span></span>|<span data-ttu-id="427c4-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="427c4-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="427c4-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-456">This property is read-only.</span></span> <span data-ttu-id="427c4-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-458">udid</span><span class="sxs-lookup"><span data-stu-id="427c4-458">udid</span></span>|<span data-ttu-id="427c4-459">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="427c4-459">String</span></span>|<span data-ttu-id="427c4-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="427c4-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="427c4-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-461">This property is read-only.</span></span> <span data-ttu-id="427c4-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="427c4-463">roleScopeTagIds</span></span>|<span data-ttu-id="427c4-464">String collection</span><span class="sxs-lookup"><span data-stu-id="427c4-464">String collection</span></span>|<span data-ttu-id="427c4-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="427c4-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="427c4-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="427c4-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="427c4-468">Int32</span><span class="sxs-lookup"><span data-stu-id="427c4-468">Int32</span></span>|<span data-ttu-id="427c4-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="427c4-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="427c4-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-470">This property is read-only.</span></span> <span data-ttu-id="427c4-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="427c4-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="427c4-473">Int32</span><span class="sxs-lookup"><span data-stu-id="427c4-473">Int32</span></span>|<span data-ttu-id="427c4-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="427c4-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="427c4-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="427c4-475">This property is read-only.</span></span> <span data-ttu-id="427c4-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-477">notes</span><span class="sxs-lookup"><span data-stu-id="427c4-477">notes</span></span>|<span data-ttu-id="427c4-478">String</span><span class="sxs-lookup"><span data-stu-id="427c4-478">String</span></span>|<span data-ttu-id="427c4-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="427c4-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="427c4-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="427c4-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="427c4-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="427c4-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="427c4-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="427c4-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="427c4-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="427c4-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="427c4-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="427c4-486">Resposta</span><span class="sxs-lookup"><span data-stu-id="427c4-486">Response</span></span>
<span data-ttu-id="427c4-487">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="427c4-487">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="427c4-488">Exemplo</span><span class="sxs-lookup"><span data-stu-id="427c4-488">Example</span></span>

### <a name="request"></a><span data-ttu-id="427c4-489">Solicitação</span><span class="sxs-lookup"><span data-stu-id="427c4-489">Request</span></span>
<span data-ttu-id="427c4-490">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="427c4-490">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="427c4-491">Resposta</span><span class="sxs-lookup"><span data-stu-id="427c4-491">Response</span></span>
<span data-ttu-id="427c4-p168">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="427c4-p168">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






