---
title: Criar windowsManagedDevice
description: Criar um novo objeto windowsManagedDevice.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e410bc5dbda16c30a4f9bed9e95aa85ffc1dfd05
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944290"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="42b8c-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="42b8c-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="42b8c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42b8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42b8c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42b8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42b8c-106">Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="42b8c-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42b8c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42b8c-107">Prerequisites</span></span>
<span data-ttu-id="42b8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42b8c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42b8c-110">Permission type</span></span>|<span data-ttu-id="42b8c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42b8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42b8c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42b8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42b8c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42b8c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42b8c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42b8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42b8c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42b8c-115">Not supported.</span></span>|
|<span data-ttu-id="42b8c-116">Application</span><span class="sxs-lookup"><span data-stu-id="42b8c-116">Application</span></span>|<span data-ttu-id="42b8c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42b8c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42b8c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42b8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="42b8c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42b8c-119">Request headers</span></span>
|<span data-ttu-id="42b8c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42b8c-120">Header</span></span>|<span data-ttu-id="42b8c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="42b8c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42b8c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42b8c-122">Authorization</span></span>|<span data-ttu-id="42b8c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42b8c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42b8c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42b8c-124">Accept</span></span>|<span data-ttu-id="42b8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42b8c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42b8c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42b8c-126">Request body</span></span>
<span data-ttu-id="42b8c-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="42b8c-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="42b8c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="42b8c-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="42b8c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42b8c-129">Property</span></span>|<span data-ttu-id="42b8c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="42b8c-130">Type</span></span>|<span data-ttu-id="42b8c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="42b8c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42b8c-132">id</span><span class="sxs-lookup"><span data-stu-id="42b8c-132">id</span></span>|<span data-ttu-id="42b8c-133">String</span><span class="sxs-lookup"><span data-stu-id="42b8c-133">String</span></span>|<span data-ttu-id="42b8c-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-134">Unique Identifier for the device.</span></span> <span data-ttu-id="42b8c-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-135">This property is read-only.</span></span> <span data-ttu-id="42b8c-136">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-136">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-137">userId</span><span class="sxs-lookup"><span data-stu-id="42b8c-137">userId</span></span>|<span data-ttu-id="42b8c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-138">String</span></span>|<span data-ttu-id="42b8c-139">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-139">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="42b8c-140">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-140">This property is read-only.</span></span> <span data-ttu-id="42b8c-141">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-141">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="42b8c-142">deviceName</span></span>|<span data-ttu-id="42b8c-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-143">String</span></span>|<span data-ttu-id="42b8c-144">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-144">Name of the device.</span></span> <span data-ttu-id="42b8c-145">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-145">This property is read-only.</span></span> <span data-ttu-id="42b8c-146">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-146">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-147">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="42b8c-147">hardwareInformation</span></span>|[<span data-ttu-id="42b8c-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="42b8c-148">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="42b8c-149">Os detalhes do hardward para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-149">The hardward details for the device.</span></span>  <span data-ttu-id="42b8c-150">Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-150">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="42b8c-151">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-151">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-152">ownerType</span><span class="sxs-lookup"><span data-stu-id="42b8c-152">ownerType</span></span>|[<span data-ttu-id="42b8c-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="42b8c-153">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="42b8c-154">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-154">Ownership of the device.</span></span> <span data-ttu-id="42b8c-155">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-155">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-156">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-156">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="42b8c-157">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="42b8c-157">managedDeviceOwnerType</span></span>|[<span data-ttu-id="42b8c-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="42b8c-158">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="42b8c-159">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-159">Ownership of the device.</span></span> <span data-ttu-id="42b8c-160">Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-160">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-161">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-161">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="42b8c-162">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="42b8c-162">deviceActionResults</span></span>|<span data-ttu-id="42b8c-163">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-163">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="42b8c-164">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="42b8c-164">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="42b8c-165">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-165">This property is read-only.</span></span> <span data-ttu-id="42b8c-166">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-166">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-167">ManagementState</span><span class="sxs-lookup"><span data-stu-id="42b8c-167">managementState</span></span>|[<span data-ttu-id="42b8c-168">ManagementState</span><span class="sxs-lookup"><span data-stu-id="42b8c-168">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="42b8c-169">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-169">Management state of the device.</span></span> <span data-ttu-id="42b8c-170">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-170">This property is read-only.</span></span> <span data-ttu-id="42b8c-171">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-172">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-172">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="42b8c-173">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-173">enrolledDateTime</span></span>|<span data-ttu-id="42b8c-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-174">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-175">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-175">Enrollment time of the device.</span></span> <span data-ttu-id="42b8c-176">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-176">This property is read-only.</span></span> <span data-ttu-id="42b8c-177">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-177">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-178">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-178">lastSyncDateTime</span></span>|<span data-ttu-id="42b8c-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-179">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-180">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="42b8c-180">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="42b8c-181">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-181">This property is read-only.</span></span> <span data-ttu-id="42b8c-182">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-182">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-183">chassisType</span><span class="sxs-lookup"><span data-stu-id="42b8c-183">chassisType</span></span>|[<span data-ttu-id="42b8c-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="42b8c-184">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="42b8c-185">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-185">Chassis type of the device.</span></span> <span data-ttu-id="42b8c-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-186">This property is read-only.</span></span> <span data-ttu-id="42b8c-187">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-187">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-188">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-188">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="42b8c-189">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="42b8c-189">operatingSystem</span></span>|<span data-ttu-id="42b8c-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-190">String</span></span>|<span data-ttu-id="42b8c-191">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-191">Operating system of the device.</span></span> <span data-ttu-id="42b8c-192">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-192">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="42b8c-193">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-193">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-194">deviceType</span><span class="sxs-lookup"><span data-stu-id="42b8c-194">deviceType</span></span>|[<span data-ttu-id="42b8c-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="42b8c-195">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="42b8c-196">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-196">Platform of the device.</span></span> <span data-ttu-id="42b8c-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-197">This property is read-only.</span></span> <span data-ttu-id="42b8c-198">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-198">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-199">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="42b8c-199">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="42b8c-200">complianceState</span><span class="sxs-lookup"><span data-stu-id="42b8c-200">complianceState</span></span>|[<span data-ttu-id="42b8c-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="42b8c-201">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="42b8c-202">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-202">Compliance state of the device.</span></span> <span data-ttu-id="42b8c-203">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-203">This property is read-only.</span></span> <span data-ttu-id="42b8c-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-205">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-205">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="42b8c-206">jailBroken</span><span class="sxs-lookup"><span data-stu-id="42b8c-206">jailBroken</span></span>|<span data-ttu-id="42b8c-207">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-207">String</span></span>|<span data-ttu-id="42b8c-208">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="42b8c-208">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="42b8c-209">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-209">This property is read-only.</span></span> <span data-ttu-id="42b8c-210">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-210">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-211">managementAgent</span><span class="sxs-lookup"><span data-stu-id="42b8c-211">managementAgent</span></span>|[<span data-ttu-id="42b8c-212">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="42b8c-212">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="42b8c-213">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-213">Management channel of the device.</span></span> <span data-ttu-id="42b8c-214">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-214">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="42b8c-215">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-216">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-216">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="42b8c-217">osVersion</span><span class="sxs-lookup"><span data-stu-id="42b8c-217">osVersion</span></span>|<span data-ttu-id="42b8c-218">String</span><span class="sxs-lookup"><span data-stu-id="42b8c-218">String</span></span>|<span data-ttu-id="42b8c-219">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-219">Operating system version of the device.</span></span> <span data-ttu-id="42b8c-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-220">This property is read-only.</span></span> <span data-ttu-id="42b8c-221">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-221">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-222">easActivated</span><span class="sxs-lookup"><span data-stu-id="42b8c-222">easActivated</span></span>|<span data-ttu-id="42b8c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-223">Boolean</span></span>|<span data-ttu-id="42b8c-224">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="42b8c-224">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="42b8c-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-225">This property is read-only.</span></span> <span data-ttu-id="42b8c-226">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-226">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="42b8c-227">easDeviceId</span></span>|<span data-ttu-id="42b8c-228">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-228">String</span></span>|<span data-ttu-id="42b8c-229">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-229">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="42b8c-230">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-230">This property is read-only.</span></span> <span data-ttu-id="42b8c-231">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-231">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-232">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-232">easActivationDateTime</span></span>|<span data-ttu-id="42b8c-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-233">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-234">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-234">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="42b8c-235">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-235">This property is read-only.</span></span> <span data-ttu-id="42b8c-236">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-237">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="42b8c-237">aadRegistered</span></span>|<span data-ttu-id="42b8c-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-238">Boolean</span></span>|<span data-ttu-id="42b8c-239">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="42b8c-239">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="42b8c-240">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-240">This property is read-only.</span></span> <span data-ttu-id="42b8c-241">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-241">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-242">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="42b8c-242">azureADRegistered</span></span>|<span data-ttu-id="42b8c-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-243">Boolean</span></span>|<span data-ttu-id="42b8c-244">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="42b8c-244">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="42b8c-245">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-245">This property is read-only.</span></span> <span data-ttu-id="42b8c-246">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-246">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-247">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="42b8c-247">deviceEnrollmentType</span></span>|[<span data-ttu-id="42b8c-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="42b8c-248">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="42b8c-249">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-249">Enrollment type of the device.</span></span> <span data-ttu-id="42b8c-250">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-250">This property is read-only.</span></span> <span data-ttu-id="42b8c-251">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-251">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-252">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-252">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="42b8c-253">lostModeState</span><span class="sxs-lookup"><span data-stu-id="42b8c-253">lostModeState</span></span>|[<span data-ttu-id="42b8c-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="42b8c-254">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="42b8c-255">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="42b8c-255">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="42b8c-256">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-256">This property is read-only.</span></span> <span data-ttu-id="42b8c-257">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-257">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-258">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-258">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="42b8c-259">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="42b8c-259">activationLockBypassCode</span></span>|<span data-ttu-id="42b8c-260">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-260">String</span></span>|<span data-ttu-id="42b8c-261">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="42b8c-261">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="42b8c-262">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-262">This property is read-only.</span></span> <span data-ttu-id="42b8c-263">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-263">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-264">emailAddress</span><span class="sxs-lookup"><span data-stu-id="42b8c-264">emailAddress</span></span>|<span data-ttu-id="42b8c-265">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-265">String</span></span>|<span data-ttu-id="42b8c-266">Email (s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-266">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="42b8c-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-267">This property is read-only.</span></span> <span data-ttu-id="42b8c-268">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-269">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="42b8c-269">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="42b8c-270">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-270">String</span></span>|<span data-ttu-id="42b8c-271">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="42b8c-271">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="42b8c-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-272">Read only.</span></span> <span data-ttu-id="42b8c-273">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-273">This property is read-only.</span></span> <span data-ttu-id="42b8c-274">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-275">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="42b8c-275">azureADDeviceId</span></span>|<span data-ttu-id="42b8c-276">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-276">String</span></span>|<span data-ttu-id="42b8c-277">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="42b8c-277">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="42b8c-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-278">Read only.</span></span> <span data-ttu-id="42b8c-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-279">This property is read-only.</span></span> <span data-ttu-id="42b8c-280">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-280">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-281">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="42b8c-281">deviceRegistrationState</span></span>|[<span data-ttu-id="42b8c-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="42b8c-282">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="42b8c-283">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-283">Device registration state.</span></span> <span data-ttu-id="42b8c-284">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-284">This property is read-only.</span></span> <span data-ttu-id="42b8c-285">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-285">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-286">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-286">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="42b8c-287">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="42b8c-287">deviceCategoryDisplayName</span></span>|<span data-ttu-id="42b8c-288">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-288">String</span></span>|<span data-ttu-id="42b8c-289">Nome de exibição da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-289">Device category display name.</span></span> <span data-ttu-id="42b8c-290">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-290">This property is read-only.</span></span> <span data-ttu-id="42b8c-291">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-291">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-292">isSupervised</span><span class="sxs-lookup"><span data-stu-id="42b8c-292">isSupervised</span></span>|<span data-ttu-id="42b8c-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-293">Boolean</span></span>|<span data-ttu-id="42b8c-294">Status supervisionado de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-294">Device supervised status.</span></span> <span data-ttu-id="42b8c-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-295">This property is read-only.</span></span> <span data-ttu-id="42b8c-296">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-296">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-297">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-297">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="42b8c-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-298">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-299">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="42b8c-299">Last time the device contacted Exchange.</span></span> <span data-ttu-id="42b8c-300">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-300">This property is read-only.</span></span> <span data-ttu-id="42b8c-301">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-301">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="42b8c-302">exchangeAccessState</span></span>|[<span data-ttu-id="42b8c-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="42b8c-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="42b8c-304">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="42b8c-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="42b8c-305">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-305">This property is read-only.</span></span> <span data-ttu-id="42b8c-306">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-306">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-307">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-307">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="42b8c-308">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="42b8c-308">exchangeAccessStateReason</span></span>|[<span data-ttu-id="42b8c-309">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="42b8c-309">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="42b8c-310">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="42b8c-310">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="42b8c-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-311">This property is read-only.</span></span> <span data-ttu-id="42b8c-312">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-312">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-313">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-313">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="42b8c-314">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="42b8c-314">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="42b8c-315">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-315">String</span></span>|<span data-ttu-id="42b8c-316">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-316">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="42b8c-317">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-317">This property is read-only.</span></span> <span data-ttu-id="42b8c-318">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-318">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-319">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="42b8c-319">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="42b8c-320">String</span><span class="sxs-lookup"><span data-stu-id="42b8c-320">String</span></span>|<span data-ttu-id="42b8c-321">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="42b8c-321">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="42b8c-322">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-322">This property is read-only.</span></span> <span data-ttu-id="42b8c-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-324">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="42b8c-324">isEncrypted</span></span>|<span data-ttu-id="42b8c-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-325">Boolean</span></span>|<span data-ttu-id="42b8c-326">Status de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-326">Device encryption status.</span></span> <span data-ttu-id="42b8c-327">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-327">This property is read-only.</span></span> <span data-ttu-id="42b8c-328">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-328">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-329">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42b8c-329">userPrincipalName</span></span>|<span data-ttu-id="42b8c-330">String</span><span class="sxs-lookup"><span data-stu-id="42b8c-330">String</span></span>|<span data-ttu-id="42b8c-331">Nome principal de usuário de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-331">Device user principal name.</span></span> <span data-ttu-id="42b8c-332">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-332">This property is read-only.</span></span> <span data-ttu-id="42b8c-333">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-333">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-334">modelo</span><span class="sxs-lookup"><span data-stu-id="42b8c-334">model</span></span>|<span data-ttu-id="42b8c-335">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-335">String</span></span>|<span data-ttu-id="42b8c-336">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-336">Model of the device.</span></span> <span data-ttu-id="42b8c-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-337">This property is read-only.</span></span> <span data-ttu-id="42b8c-338">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-338">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-339">fabricante</span><span class="sxs-lookup"><span data-stu-id="42b8c-339">manufacturer</span></span>|<span data-ttu-id="42b8c-340">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-340">String</span></span>|<span data-ttu-id="42b8c-341">O fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-341">Manufacturer of the device.</span></span> <span data-ttu-id="42b8c-342">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-342">This property is read-only.</span></span> <span data-ttu-id="42b8c-343">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-343">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-344">imei</span><span class="sxs-lookup"><span data-stu-id="42b8c-344">imei</span></span>|<span data-ttu-id="42b8c-345">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-345">String</span></span>|<span data-ttu-id="42b8c-346">IMEI.</span><span class="sxs-lookup"><span data-stu-id="42b8c-346">IMEI.</span></span> <span data-ttu-id="42b8c-347">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-347">This property is read-only.</span></span> <span data-ttu-id="42b8c-348">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-348">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-349">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-349">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="42b8c-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-350">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-351">O DateTime quando o período de cortesia de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="42b8c-351">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="42b8c-352">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-352">This property is read-only.</span></span> <span data-ttu-id="42b8c-353">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-353">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-354">serialNumber</span><span class="sxs-lookup"><span data-stu-id="42b8c-354">serialNumber</span></span>|<span data-ttu-id="42b8c-355">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-355">String</span></span>|<span data-ttu-id="42b8c-356">Autoridade.</span><span class="sxs-lookup"><span data-stu-id="42b8c-356">SerialNumber.</span></span> <span data-ttu-id="42b8c-357">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-357">This property is read-only.</span></span> <span data-ttu-id="42b8c-358">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-359">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="42b8c-359">phoneNumber</span></span>|<span data-ttu-id="42b8c-360">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-360">String</span></span>|<span data-ttu-id="42b8c-361">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-361">Phone number of the device.</span></span> <span data-ttu-id="42b8c-362">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-362">This property is read-only.</span></span> <span data-ttu-id="42b8c-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-364">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="42b8c-364">androidSecurityPatchLevel</span></span>|<span data-ttu-id="42b8c-365">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-365">String</span></span>|<span data-ttu-id="42b8c-366">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="42b8c-366">Android security patch level.</span></span> <span data-ttu-id="42b8c-367">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-367">This property is read-only.</span></span> <span data-ttu-id="42b8c-368">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-368">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-369">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="42b8c-369">userDisplayName</span></span>|<span data-ttu-id="42b8c-370">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-370">String</span></span>|<span data-ttu-id="42b8c-371">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="42b8c-371">User display name.</span></span> <span data-ttu-id="42b8c-372">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-372">This property is read-only.</span></span> <span data-ttu-id="42b8c-373">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-374">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="42b8c-374">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="42b8c-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="42b8c-375">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="42b8c-376">Recursos habilitados para cliente do ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="42b8c-376">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="42b8c-377">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-377">This property is read-only.</span></span> <span data-ttu-id="42b8c-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-379">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="42b8c-379">wiFiMacAddress</span></span>|<span data-ttu-id="42b8c-380">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-380">String</span></span>|<span data-ttu-id="42b8c-381">MAC Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="42b8c-381">Wi-Fi MAC.</span></span> <span data-ttu-id="42b8c-382">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-382">This property is read-only.</span></span> <span data-ttu-id="42b8c-383">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-383">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-384">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="42b8c-384">deviceHealthAttestationState</span></span>|[<span data-ttu-id="42b8c-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="42b8c-385">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="42b8c-386">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-386">The device health attestation state.</span></span> <span data-ttu-id="42b8c-387">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-387">This property is read-only.</span></span> <span data-ttu-id="42b8c-388">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-388">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-389">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="42b8c-389">subscriberCarrier</span></span>|<span data-ttu-id="42b8c-390">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-390">String</span></span>|<span data-ttu-id="42b8c-391">Operadora de assinante.</span><span class="sxs-lookup"><span data-stu-id="42b8c-391">Subscriber Carrier.</span></span> <span data-ttu-id="42b8c-392">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-392">This property is read-only.</span></span> <span data-ttu-id="42b8c-393">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-393">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-394">meid</span><span class="sxs-lookup"><span data-stu-id="42b8c-394">meid</span></span>|<span data-ttu-id="42b8c-395">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-395">String</span></span>|<span data-ttu-id="42b8c-396">MEID.</span><span class="sxs-lookup"><span data-stu-id="42b8c-396">MEID.</span></span> <span data-ttu-id="42b8c-397">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-397">This property is read-only.</span></span> <span data-ttu-id="42b8c-398">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-398">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-399">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="42b8c-399">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="42b8c-400">Int64</span><span class="sxs-lookup"><span data-stu-id="42b8c-400">Int64</span></span>|<span data-ttu-id="42b8c-401">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="42b8c-401">Total Storage in Bytes.</span></span> <span data-ttu-id="42b8c-402">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-402">This property is read-only.</span></span> <span data-ttu-id="42b8c-403">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-403">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-404">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="42b8c-404">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="42b8c-405">Int64</span><span class="sxs-lookup"><span data-stu-id="42b8c-405">Int64</span></span>|<span data-ttu-id="42b8c-406">Armazenamento gratuito em bytes.</span><span class="sxs-lookup"><span data-stu-id="42b8c-406">Free Storage in Bytes.</span></span> <span data-ttu-id="42b8c-407">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-407">This property is read-only.</span></span> <span data-ttu-id="42b8c-408">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-408">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-409">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="42b8c-409">managedDeviceName</span></span>|<span data-ttu-id="42b8c-410">String</span><span class="sxs-lookup"><span data-stu-id="42b8c-410">String</span></span>|<span data-ttu-id="42b8c-411">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-411">Automatically generated name to identify a device.</span></span> <span data-ttu-id="42b8c-412">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="42b8c-412">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="42b8c-413">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-413">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-414">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="42b8c-414">partnerReportedThreatState</span></span>|[<span data-ttu-id="42b8c-415">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="42b8c-415">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="42b8c-416">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-416">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="42b8c-417">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-417">Read Only.</span></span> <span data-ttu-id="42b8c-418">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-418">This property is read-only.</span></span> <span data-ttu-id="42b8c-419">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-419">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-420">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-420">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="42b8c-421">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-421">retireAfterDateTime</span></span>|<span data-ttu-id="42b8c-422">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-422">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-423">Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="42b8c-423">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="42b8c-424">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-424">This property is read-only.</span></span> <span data-ttu-id="42b8c-425">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-425">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-426">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="42b8c-426">usersLoggedOn</span></span>|<span data-ttu-id="42b8c-427">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-427">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="42b8c-428">Indica o último usuário conectado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-428">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="42b8c-429">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-429">This property is read-only.</span></span> <span data-ttu-id="42b8c-430">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-430">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-431">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="42b8c-431">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="42b8c-432">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-432">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-433">Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="42b8c-433">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="42b8c-434">Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="42b8c-434">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="42b8c-435">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-435">Read Only.</span></span> <span data-ttu-id="42b8c-436">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-436">This property is read-only.</span></span> <span data-ttu-id="42b8c-437">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-437">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-438">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="42b8c-438">autopilotEnrolled</span></span>|<span data-ttu-id="42b8c-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-439">Boolean</span></span>|<span data-ttu-id="42b8c-440">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="42b8c-440">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="42b8c-441">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-441">This property is read-only.</span></span> <span data-ttu-id="42b8c-442">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-442">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-443">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="42b8c-443">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="42b8c-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b8c-444">Boolean</span></span>|<span data-ttu-id="42b8c-445">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="42b8c-445">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="42b8c-446">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-446">This property is read-only.</span></span> <span data-ttu-id="42b8c-447">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-447">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-448">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="42b8c-448">managementCertificateExpirationDate</span></span>|<span data-ttu-id="42b8c-449">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b8c-449">DateTimeOffset</span></span>|<span data-ttu-id="42b8c-450">Relata a data de validade do certificado de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="42b8c-450">Reports device management certificate expiration date.</span></span> <span data-ttu-id="42b8c-451">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-451">This property is read-only.</span></span> <span data-ttu-id="42b8c-452">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-452">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-453">iccid</span><span class="sxs-lookup"><span data-stu-id="42b8c-453">iccid</span></span>|<span data-ttu-id="42b8c-454">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-454">String</span></span>|<span data-ttu-id="42b8c-455">Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="42b8c-455">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="42b8c-456">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-456">This property is read-only.</span></span> <span data-ttu-id="42b8c-457">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-457">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-458">udid</span><span class="sxs-lookup"><span data-stu-id="42b8c-458">udid</span></span>|<span data-ttu-id="42b8c-459">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-459">String</span></span>|<span data-ttu-id="42b8c-460">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="42b8c-460">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="42b8c-461">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-461">This property is read-only.</span></span> <span data-ttu-id="42b8c-462">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-462">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-463">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42b8c-463">roleScopeTagIds</span></span>|<span data-ttu-id="42b8c-464">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-464">String collection</span></span>|<span data-ttu-id="42b8c-465">Lista de IDs de marca de escopo para esta instância de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b8c-465">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="42b8c-466">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-466">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-467">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="42b8c-467">windowsActiveMalwareCount</span></span>|<span data-ttu-id="42b8c-468">Int32</span><span class="sxs-lookup"><span data-stu-id="42b8c-468">Int32</span></span>|<span data-ttu-id="42b8c-469">Contagem de malware ativo para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="42b8c-469">Count of active malware for this windows device.</span></span> <span data-ttu-id="42b8c-470">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-470">This property is read-only.</span></span> <span data-ttu-id="42b8c-471">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-471">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-472">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="42b8c-472">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="42b8c-473">Int32</span><span class="sxs-lookup"><span data-stu-id="42b8c-473">Int32</span></span>|<span data-ttu-id="42b8c-474">Contagem de malware corrigido para este dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="42b8c-474">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="42b8c-475">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-475">This property is read-only.</span></span> <span data-ttu-id="42b8c-476">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-476">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-477">notes</span><span class="sxs-lookup"><span data-stu-id="42b8c-477">notes</span></span>|<span data-ttu-id="42b8c-478">String</span><span class="sxs-lookup"><span data-stu-id="42b8c-478">String</span></span>|<span data-ttu-id="42b8c-479">Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-479">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-480">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="42b8c-480">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="42b8c-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="42b8c-481">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="42b8c-482">Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-482">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-483">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="42b8c-483">configurationManagerClientInformation</span></span>|[<span data-ttu-id="42b8c-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="42b8c-484">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="42b8c-485">Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-485">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-486">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="42b8c-486">ethernetMacAddress</span></span>|<span data-ttu-id="42b8c-487">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42b8c-487">String</span></span>|<span data-ttu-id="42b8c-488">MAC Ethernet.</span><span class="sxs-lookup"><span data-stu-id="42b8c-488">Ethernet MAC.</span></span> <span data-ttu-id="42b8c-489">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-489">This property is read-only.</span></span> <span data-ttu-id="42b8c-490">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-490">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-491">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="42b8c-491">physicalMemoryInBytes</span></span>|<span data-ttu-id="42b8c-492">Int64</span><span class="sxs-lookup"><span data-stu-id="42b8c-492">Int64</span></span>|<span data-ttu-id="42b8c-493">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="42b8c-493">Total Memory in Bytes.</span></span> <span data-ttu-id="42b8c-494">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-494">This property is read-only.</span></span> <span data-ttu-id="42b8c-495">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="42b8c-495">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="42b8c-496">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="42b8c-496">processorArchitecture</span></span>|[<span data-ttu-id="42b8c-497">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="42b8c-497">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="42b8c-498">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="42b8c-498">Processor architecture.</span></span> <span data-ttu-id="42b8c-499">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42b8c-499">This property is read-only.</span></span> <span data-ttu-id="42b8c-500">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="42b8c-500">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="42b8c-501">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="42b8c-501">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|



## <a name="response"></a><span data-ttu-id="42b8c-502">Resposta</span><span class="sxs-lookup"><span data-stu-id="42b8c-502">Response</span></span>
<span data-ttu-id="42b8c-503">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42b8c-503">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b8c-504">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42b8c-504">Example</span></span>

### <a name="request"></a><span data-ttu-id="42b8c-505">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42b8c-505">Request</span></span>
<span data-ttu-id="42b8c-506">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42b8c-506">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42b8c-507">Resposta</span><span class="sxs-lookup"><span data-stu-id="42b8c-507">Response</span></span>
<span data-ttu-id="42b8c-p171">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42b8c-p171">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





