---
title: Criar windowsManagedDevice
description: Crie um novo objeto windowsManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ebecd3e4da57aa52c896e5352204d3306e47757
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865226"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="d712f-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="d712f-103">Create windowsManagedDevice</span></span>

<span data-ttu-id="d712f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d712f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d712f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d712f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d712f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d712f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d712f-107">Crie um novo [objeto windowsManagedDevice.](../resources/intune-devices-windowsmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d712f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d712f-108">Prerequisites</span></span>
<span data-ttu-id="d712f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d712f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d712f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d712f-111">Permission type</span></span>|<span data-ttu-id="d712f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d712f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d712f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d712f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d712f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d712f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d712f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d712f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d712f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d712f-116">Not supported.</span></span>|
|<span data-ttu-id="d712f-117">Application</span><span class="sxs-lookup"><span data-stu-id="d712f-117">Application</span></span>|<span data-ttu-id="d712f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d712f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d712f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d712f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
POST /deviceManagement/comanagedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="d712f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d712f-120">Request headers</span></span>
|<span data-ttu-id="d712f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d712f-121">Header</span></span>|<span data-ttu-id="d712f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d712f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d712f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d712f-123">Authorization</span></span>|<span data-ttu-id="d712f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d712f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d712f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d712f-125">Accept</span></span>|<span data-ttu-id="d712f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d712f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d712f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d712f-127">Request body</span></span>
<span data-ttu-id="d712f-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="d712f-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="d712f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="d712f-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="d712f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d712f-130">Property</span></span>|<span data-ttu-id="d712f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d712f-131">Type</span></span>|<span data-ttu-id="d712f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d712f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d712f-133">id</span><span class="sxs-lookup"><span data-stu-id="d712f-133">id</span></span>|<span data-ttu-id="d712f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-134">String</span></span>|<span data-ttu-id="d712f-135">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-135">Unique Identifier for the device.</span></span> <span data-ttu-id="d712f-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-136">This property is read-only.</span></span> <span data-ttu-id="d712f-137">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-137">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-138">userId</span><span class="sxs-lookup"><span data-stu-id="d712f-138">userId</span></span>|<span data-ttu-id="d712f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-139">String</span></span>|<span data-ttu-id="d712f-140">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-140">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="d712f-141">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-141">This property is read-only.</span></span> <span data-ttu-id="d712f-142">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-142">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="d712f-143">deviceName</span></span>|<span data-ttu-id="d712f-144">String</span><span class="sxs-lookup"><span data-stu-id="d712f-144">String</span></span>|<span data-ttu-id="d712f-145">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-145">Name of the device.</span></span> <span data-ttu-id="d712f-146">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-146">This property is read-only.</span></span> <span data-ttu-id="d712f-147">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-147">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-148">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d712f-148">hardwareInformation</span></span>|[<span data-ttu-id="d712f-149">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d712f-149">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="d712f-150">Os detalhes rígidos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-150">The hardward details for the device.</span></span>  <span data-ttu-id="d712f-151">Inclui informações como espaço de armazenamento, fabricante, número de série etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-151">Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.</span></span> <span data-ttu-id="d712f-152">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-152">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-153">ownerType</span><span class="sxs-lookup"><span data-stu-id="d712f-153">ownerType</span></span>|[<span data-ttu-id="d712f-154">ownerType</span><span class="sxs-lookup"><span data-stu-id="d712f-154">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="d712f-155">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-155">Ownership of the device.</span></span> <span data-ttu-id="d712f-156">Pode ser 'empresa' ou 'pessoal' Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-156">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-157">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d712f-157">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d712f-158">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d712f-158">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d712f-159">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d712f-159">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="d712f-160">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-160">Ownership of the device.</span></span> <span data-ttu-id="d712f-161">Pode ser 'empresa' ou 'pessoal' Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-161">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-162">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d712f-162">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d712f-163">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d712f-163">deviceActionResults</span></span>|<span data-ttu-id="d712f-164">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-164">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d712f-165">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="d712f-165">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="d712f-166">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-166">This property is read-only.</span></span> <span data-ttu-id="d712f-167">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-168">managementState</span><span class="sxs-lookup"><span data-stu-id="d712f-168">managementState</span></span>|[<span data-ttu-id="d712f-169">managementState</span><span class="sxs-lookup"><span data-stu-id="d712f-169">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="d712f-170">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-170">Management state of the device.</span></span> <span data-ttu-id="d712f-171">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-171">This property is read-only.</span></span> <span data-ttu-id="d712f-172">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-173">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="d712f-173">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="d712f-174">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-174">enrolledDateTime</span></span>|<span data-ttu-id="d712f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-175">DateTimeOffset</span></span>|<span data-ttu-id="d712f-176">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-176">Enrollment time of the device.</span></span> <span data-ttu-id="d712f-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-177">This property is read-only.</span></span> <span data-ttu-id="d712f-178">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-178">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-179">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-179">lastSyncDateTime</span></span>|<span data-ttu-id="d712f-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-180">DateTimeOffset</span></span>|<span data-ttu-id="d712f-181">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="d712f-181">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="d712f-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-182">This property is read-only.</span></span> <span data-ttu-id="d712f-183">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-183">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-184">chassisType</span><span class="sxs-lookup"><span data-stu-id="d712f-184">chassisType</span></span>|[<span data-ttu-id="d712f-185">chassisType</span><span class="sxs-lookup"><span data-stu-id="d712f-185">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="d712f-186">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-186">Chassis type of the device.</span></span> <span data-ttu-id="d712f-187">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-187">This property is read-only.</span></span> <span data-ttu-id="d712f-188">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-188">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-189">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="d712f-189">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="d712f-190">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d712f-190">operatingSystem</span></span>|<span data-ttu-id="d712f-191">String</span><span class="sxs-lookup"><span data-stu-id="d712f-191">String</span></span>|<span data-ttu-id="d712f-192">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-192">Operating system of the device.</span></span> <span data-ttu-id="d712f-193">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-193">Windows, iOS, etc. This property is read-only.</span></span> <span data-ttu-id="d712f-194">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-195">deviceType</span><span class="sxs-lookup"><span data-stu-id="d712f-195">deviceType</span></span>|[<span data-ttu-id="d712f-196">deviceType</span><span class="sxs-lookup"><span data-stu-id="d712f-196">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d712f-197">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-197">Platform of the device.</span></span> <span data-ttu-id="d712f-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-198">This property is read-only.</span></span> <span data-ttu-id="d712f-199">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-199">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-200">Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="d712f-200">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="d712f-201">complianceState</span><span class="sxs-lookup"><span data-stu-id="d712f-201">complianceState</span></span>|[<span data-ttu-id="d712f-202">complianceState</span><span class="sxs-lookup"><span data-stu-id="d712f-202">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d712f-203">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-203">Compliance state of the device.</span></span> <span data-ttu-id="d712f-204">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-204">This property is read-only.</span></span> <span data-ttu-id="d712f-205">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-205">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-206">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="d712f-206">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d712f-207">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d712f-207">jailBroken</span></span>|<span data-ttu-id="d712f-208">String</span><span class="sxs-lookup"><span data-stu-id="d712f-208">String</span></span>|<span data-ttu-id="d712f-209">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="d712f-209">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="d712f-210">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-210">This property is read-only.</span></span> <span data-ttu-id="d712f-211">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-212">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d712f-212">managementAgent</span></span>|[<span data-ttu-id="d712f-213">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d712f-213">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="d712f-214">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-214">Management channel of the device.</span></span> <span data-ttu-id="d712f-215">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-215">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="d712f-216">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-217">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `msSense`.</span><span class="sxs-lookup"><span data-stu-id="d712f-217">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `msSense`.</span></span>|
|<span data-ttu-id="d712f-218">osVersion</span><span class="sxs-lookup"><span data-stu-id="d712f-218">osVersion</span></span>|<span data-ttu-id="d712f-219">String</span><span class="sxs-lookup"><span data-stu-id="d712f-219">String</span></span>|<span data-ttu-id="d712f-220">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-220">Operating system version of the device.</span></span> <span data-ttu-id="d712f-221">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-221">This property is read-only.</span></span> <span data-ttu-id="d712f-222">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-222">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-223">easActivated</span><span class="sxs-lookup"><span data-stu-id="d712f-223">easActivated</span></span>|<span data-ttu-id="d712f-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-224">Boolean</span></span>|<span data-ttu-id="d712f-225">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d712f-225">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="d712f-226">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-226">This property is read-only.</span></span> <span data-ttu-id="d712f-227">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-228">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d712f-228">easDeviceId</span></span>|<span data-ttu-id="d712f-229">String</span><span class="sxs-lookup"><span data-stu-id="d712f-229">String</span></span>|<span data-ttu-id="d712f-230">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-230">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="d712f-231">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-231">This property is read-only.</span></span> <span data-ttu-id="d712f-232">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-232">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-233">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-233">easActivationDateTime</span></span>|<span data-ttu-id="d712f-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-234">DateTimeOffset</span></span>|<span data-ttu-id="d712f-235">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-235">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="d712f-236">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-236">This property is read-only.</span></span> <span data-ttu-id="d712f-237">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-238">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="d712f-238">aadRegistered</span></span>|<span data-ttu-id="d712f-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-239">Boolean</span></span>|<span data-ttu-id="d712f-240">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d712f-240">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d712f-241">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-241">This property is read-only.</span></span> <span data-ttu-id="d712f-242">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-242">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-243">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d712f-243">azureADRegistered</span></span>|<span data-ttu-id="d712f-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-244">Boolean</span></span>|<span data-ttu-id="d712f-245">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d712f-245">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d712f-246">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-246">This property is read-only.</span></span> <span data-ttu-id="d712f-247">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-247">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-248">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d712f-248">deviceEnrollmentType</span></span>|[<span data-ttu-id="d712f-249">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d712f-249">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d712f-250">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-250">Enrollment type of the device.</span></span> <span data-ttu-id="d712f-251">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-251">This property is read-only.</span></span> <span data-ttu-id="d712f-252">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-252">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-253">Os valores possíveis são: `unknown` , , , , , , , , `userEnrollment` , , , `deviceEnrollmentManager` , , `appleBulkWithUser` , , , `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` , `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` .</span><span class="sxs-lookup"><span data-stu-id="d712f-253">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="d712f-254">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d712f-254">lostModeState</span></span>|[<span data-ttu-id="d712f-255">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d712f-255">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="d712f-256">Indica se o modo Perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="d712f-256">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="d712f-257">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-257">This property is read-only.</span></span> <span data-ttu-id="d712f-258">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-258">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-259">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="d712f-259">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d712f-260">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d712f-260">activationLockBypassCode</span></span>|<span data-ttu-id="d712f-261">String</span><span class="sxs-lookup"><span data-stu-id="d712f-261">String</span></span>|<span data-ttu-id="d712f-262">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="d712f-262">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="d712f-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-263">This property is read-only.</span></span> <span data-ttu-id="d712f-264">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-265">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d712f-265">emailAddress</span></span>|<span data-ttu-id="d712f-266">String</span><span class="sxs-lookup"><span data-stu-id="d712f-266">String</span></span>|<span data-ttu-id="d712f-267">Email(s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-267">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="d712f-268">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-268">This property is read-only.</span></span> <span data-ttu-id="d712f-269">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-270">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="d712f-270">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d712f-271">String</span><span class="sxs-lookup"><span data-stu-id="d712f-271">String</span></span>|<span data-ttu-id="d712f-272">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d712f-272">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d712f-273">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-273">Read only.</span></span> <span data-ttu-id="d712f-274">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-274">This property is read-only.</span></span> <span data-ttu-id="d712f-275">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-275">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-276">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d712f-276">azureADDeviceId</span></span>|<span data-ttu-id="d712f-277">String</span><span class="sxs-lookup"><span data-stu-id="d712f-277">String</span></span>|<span data-ttu-id="d712f-278">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d712f-278">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d712f-279">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-279">Read only.</span></span> <span data-ttu-id="d712f-280">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-280">This property is read-only.</span></span> <span data-ttu-id="d712f-281">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-281">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-282">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d712f-282">deviceRegistrationState</span></span>|[<span data-ttu-id="d712f-283">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d712f-283">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d712f-284">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-284">Device registration state.</span></span> <span data-ttu-id="d712f-285">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-285">This property is read-only.</span></span> <span data-ttu-id="d712f-286">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-286">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-287">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d712f-287">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d712f-288">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d712f-288">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d712f-289">String</span><span class="sxs-lookup"><span data-stu-id="d712f-289">String</span></span>|<span data-ttu-id="d712f-290">Nome de exibição de categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-290">Device category display name.</span></span> <span data-ttu-id="d712f-291">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-291">This property is read-only.</span></span> <span data-ttu-id="d712f-292">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-292">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-293">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d712f-293">isSupervised</span></span>|<span data-ttu-id="d712f-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-294">Boolean</span></span>|<span data-ttu-id="d712f-295">Status supervisionado pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-295">Device supervised status.</span></span> <span data-ttu-id="d712f-296">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-296">This property is read-only.</span></span> <span data-ttu-id="d712f-297">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-297">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-298">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-298">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d712f-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-299">DateTimeOffset</span></span>|<span data-ttu-id="d712f-300">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="d712f-300">Last time the device contacted Exchange.</span></span> <span data-ttu-id="d712f-301">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-301">This property is read-only.</span></span> <span data-ttu-id="d712f-302">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-302">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d712f-303">exchangeAccessState</span></span>|[<span data-ttu-id="d712f-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d712f-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d712f-305">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d712f-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d712f-306">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-306">This property is read-only.</span></span> <span data-ttu-id="d712f-307">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-307">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-308">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="d712f-308">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d712f-309">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d712f-309">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d712f-310">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d712f-310">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d712f-311">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d712f-311">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d712f-312">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-312">This property is read-only.</span></span> <span data-ttu-id="d712f-313">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-313">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-314">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="d712f-314">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d712f-315">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d712f-315">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d712f-316">String</span><span class="sxs-lookup"><span data-stu-id="d712f-316">String</span></span>|<span data-ttu-id="d712f-317">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-317">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="d712f-318">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-318">This property is read-only.</span></span> <span data-ttu-id="d712f-319">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-319">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-320">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d712f-320">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d712f-321">String</span><span class="sxs-lookup"><span data-stu-id="d712f-321">String</span></span>|<span data-ttu-id="d712f-322">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="d712f-322">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="d712f-323">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-323">This property is read-only.</span></span> <span data-ttu-id="d712f-324">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-324">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d712f-325">isEncrypted</span></span>|<span data-ttu-id="d712f-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-326">Boolean</span></span>|<span data-ttu-id="d712f-327">Status da criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-327">Device encryption status.</span></span> <span data-ttu-id="d712f-328">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-328">This property is read-only.</span></span> <span data-ttu-id="d712f-329">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-329">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-330">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d712f-330">userPrincipalName</span></span>|<span data-ttu-id="d712f-331">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-331">String</span></span>|<span data-ttu-id="d712f-332">Nome principal do usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-332">Device user principal name.</span></span> <span data-ttu-id="d712f-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-333">This property is read-only.</span></span> <span data-ttu-id="d712f-334">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-334">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-335">modelo</span><span class="sxs-lookup"><span data-stu-id="d712f-335">model</span></span>|<span data-ttu-id="d712f-336">String</span><span class="sxs-lookup"><span data-stu-id="d712f-336">String</span></span>|<span data-ttu-id="d712f-337">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-337">Model of the device.</span></span> <span data-ttu-id="d712f-338">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-338">This property is read-only.</span></span> <span data-ttu-id="d712f-339">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-340">fabricante</span><span class="sxs-lookup"><span data-stu-id="d712f-340">manufacturer</span></span>|<span data-ttu-id="d712f-341">String</span><span class="sxs-lookup"><span data-stu-id="d712f-341">String</span></span>|<span data-ttu-id="d712f-342">Fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-342">Manufacturer of the device.</span></span> <span data-ttu-id="d712f-343">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-343">This property is read-only.</span></span> <span data-ttu-id="d712f-344">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-345">imei</span><span class="sxs-lookup"><span data-stu-id="d712f-345">imei</span></span>|<span data-ttu-id="d712f-346">String</span><span class="sxs-lookup"><span data-stu-id="d712f-346">String</span></span>|<span data-ttu-id="d712f-347">IMEI.</span><span class="sxs-lookup"><span data-stu-id="d712f-347">IMEI.</span></span> <span data-ttu-id="d712f-348">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-348">This property is read-only.</span></span> <span data-ttu-id="d712f-349">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-349">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-350">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-350">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d712f-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-351">DateTimeOffset</span></span>|<span data-ttu-id="d712f-352">DateTime quando o período de carência de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="d712f-352">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="d712f-353">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-353">This property is read-only.</span></span> <span data-ttu-id="d712f-354">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-355">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d712f-355">serialNumber</span></span>|<span data-ttu-id="d712f-356">String</span><span class="sxs-lookup"><span data-stu-id="d712f-356">String</span></span>|<span data-ttu-id="d712f-357">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="d712f-357">SerialNumber.</span></span> <span data-ttu-id="d712f-358">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-358">This property is read-only.</span></span> <span data-ttu-id="d712f-359">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-360">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d712f-360">phoneNumber</span></span>|<span data-ttu-id="d712f-361">String</span><span class="sxs-lookup"><span data-stu-id="d712f-361">String</span></span>|<span data-ttu-id="d712f-362">Número de telefone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-362">Phone number of the device.</span></span> <span data-ttu-id="d712f-363">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-363">This property is read-only.</span></span> <span data-ttu-id="d712f-364">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-364">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-365">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d712f-365">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d712f-366">String</span><span class="sxs-lookup"><span data-stu-id="d712f-366">String</span></span>|<span data-ttu-id="d712f-367">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="d712f-367">Android security patch level.</span></span> <span data-ttu-id="d712f-368">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-368">This property is read-only.</span></span> <span data-ttu-id="d712f-369">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-370">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d712f-370">userDisplayName</span></span>|<span data-ttu-id="d712f-371">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-371">String</span></span>|<span data-ttu-id="d712f-372">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="d712f-372">User display name.</span></span> <span data-ttu-id="d712f-373">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-373">This property is read-only.</span></span> <span data-ttu-id="d712f-374">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-375">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d712f-375">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d712f-376">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d712f-376">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d712f-377">Recursos habilitados para cliente ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="d712f-377">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="d712f-378">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-378">This property is read-only.</span></span> <span data-ttu-id="d712f-379">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-379">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-380">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d712f-380">wiFiMacAddress</span></span>|<span data-ttu-id="d712f-381">String</span><span class="sxs-lookup"><span data-stu-id="d712f-381">String</span></span>|<span data-ttu-id="d712f-382">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="d712f-382">Wi-Fi MAC.</span></span> <span data-ttu-id="d712f-383">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-383">This property is read-only.</span></span> <span data-ttu-id="d712f-384">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-384">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-385">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d712f-385">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d712f-386">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d712f-386">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d712f-387">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-387">The device health attestation state.</span></span> <span data-ttu-id="d712f-388">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-388">This property is read-only.</span></span> <span data-ttu-id="d712f-389">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-389">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-390">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d712f-390">subscriberCarrier</span></span>|<span data-ttu-id="d712f-391">String</span><span class="sxs-lookup"><span data-stu-id="d712f-391">String</span></span>|<span data-ttu-id="d712f-392">Operadora de Assinantes.</span><span class="sxs-lookup"><span data-stu-id="d712f-392">Subscriber Carrier.</span></span> <span data-ttu-id="d712f-393">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-393">This property is read-only.</span></span> <span data-ttu-id="d712f-394">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-394">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-395">meid</span><span class="sxs-lookup"><span data-stu-id="d712f-395">meid</span></span>|<span data-ttu-id="d712f-396">String</span><span class="sxs-lookup"><span data-stu-id="d712f-396">String</span></span>|<span data-ttu-id="d712f-397">MEID.</span><span class="sxs-lookup"><span data-stu-id="d712f-397">MEID.</span></span> <span data-ttu-id="d712f-398">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-398">This property is read-only.</span></span> <span data-ttu-id="d712f-399">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-399">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-400">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d712f-400">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d712f-401">Int64</span><span class="sxs-lookup"><span data-stu-id="d712f-401">Int64</span></span>|<span data-ttu-id="d712f-402">Armazenamento total em bytes.</span><span class="sxs-lookup"><span data-stu-id="d712f-402">Total Storage in Bytes.</span></span> <span data-ttu-id="d712f-403">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-403">This property is read-only.</span></span> <span data-ttu-id="d712f-404">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-404">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-405">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d712f-405">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d712f-406">Int64</span><span class="sxs-lookup"><span data-stu-id="d712f-406">Int64</span></span>|<span data-ttu-id="d712f-407">Armazenamento gratuito em Bytes.</span><span class="sxs-lookup"><span data-stu-id="d712f-407">Free Storage in Bytes.</span></span> <span data-ttu-id="d712f-408">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-408">This property is read-only.</span></span> <span data-ttu-id="d712f-409">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-409">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-410">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d712f-410">managedDeviceName</span></span>|<span data-ttu-id="d712f-411">String</span><span class="sxs-lookup"><span data-stu-id="d712f-411">String</span></span>|<span data-ttu-id="d712f-412">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-412">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d712f-413">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d712f-413">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="d712f-414">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-414">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-415">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d712f-415">partnerReportedThreatState</span></span>|[<span data-ttu-id="d712f-416">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="d712f-416">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d712f-417">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-417">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d712f-418">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-418">Read Only.</span></span> <span data-ttu-id="d712f-419">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-419">This property is read-only.</span></span> <span data-ttu-id="d712f-420">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-420">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-421">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="d712f-421">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="d712f-422">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-422">retireAfterDateTime</span></span>|<span data-ttu-id="d712f-423">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-423">DateTimeOffset</span></span>|<span data-ttu-id="d712f-424">Indica a hora após a resuspensão automática de um dispositivo devido à ação agendada.</span><span class="sxs-lookup"><span data-stu-id="d712f-424">Indicates the time after when a device will be auto retired because of scheduled action.</span></span> <span data-ttu-id="d712f-425">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-425">This property is read-only.</span></span> <span data-ttu-id="d712f-426">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-426">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-427">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="d712f-427">usersLoggedOn</span></span>|<span data-ttu-id="d712f-428">[coleção loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-428">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="d712f-429">Indica o último usuário conectado a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-429">Indicates the last logged on users of a device.</span></span> <span data-ttu-id="d712f-430">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-430">This property is read-only.</span></span> <span data-ttu-id="d712f-431">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-431">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-432">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="d712f-432">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="d712f-433">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-433">DateTimeOffset</span></span>|<span data-ttu-id="d712f-434">Relata que DateTime a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="d712f-434">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="d712f-435">Quando definidas, as configurações do MDM do Intune substituirão as configurações da Política de Grupo se houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="d712f-435">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="d712f-436">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-436">Read Only.</span></span> <span data-ttu-id="d712f-437">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-437">This property is read-only.</span></span> <span data-ttu-id="d712f-438">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-438">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-439">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="d712f-439">autopilotEnrolled</span></span>|<span data-ttu-id="d712f-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-440">Boolean</span></span>|<span data-ttu-id="d712f-441">Relata se o dispositivo gerenciado está inscrito por meio de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="d712f-441">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="d712f-442">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-442">This property is read-only.</span></span> <span data-ttu-id="d712f-443">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-443">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-444">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="d712f-444">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="d712f-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="d712f-445">Boolean</span></span>|<span data-ttu-id="d712f-446">Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="d712f-446">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="d712f-447">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-447">This property is read-only.</span></span> <span data-ttu-id="d712f-448">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-448">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-449">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d712f-449">managementCertificateExpirationDate</span></span>|<span data-ttu-id="d712f-450">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d712f-450">DateTimeOffset</span></span>|<span data-ttu-id="d712f-451">Relata a data de expiração do certificado de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-451">Reports device management certificate expiration date.</span></span> <span data-ttu-id="d712f-452">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-452">This property is read-only.</span></span> <span data-ttu-id="d712f-453">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-453">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-454">iccid</span><span class="sxs-lookup"><span data-stu-id="d712f-454">iccid</span></span>|<span data-ttu-id="d712f-455">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-455">String</span></span>|<span data-ttu-id="d712f-456">Identificador integrado de cartão de circuito, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="d712f-456">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="d712f-457">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-457">This property is read-only.</span></span> <span data-ttu-id="d712f-458">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-458">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-459">udid</span><span class="sxs-lookup"><span data-stu-id="d712f-459">udid</span></span>|<span data-ttu-id="d712f-460">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-460">String</span></span>|<span data-ttu-id="d712f-461">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="d712f-461">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="d712f-462">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-462">This property is read-only.</span></span> <span data-ttu-id="d712f-463">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-463">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-464">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d712f-464">roleScopeTagIds</span></span>|<span data-ttu-id="d712f-465">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d712f-465">String collection</span></span>|<span data-ttu-id="d712f-466">Lista de IDs de marca de escopo para esta instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d712f-466">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="d712f-467">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-467">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-468">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d712f-468">windowsActiveMalwareCount</span></span>|<span data-ttu-id="d712f-469">Int32</span><span class="sxs-lookup"><span data-stu-id="d712f-469">Int32</span></span>|<span data-ttu-id="d712f-470">Contagem de malware ativo para este dispositivo windows.</span><span class="sxs-lookup"><span data-stu-id="d712f-470">Count of active malware for this windows device.</span></span> <span data-ttu-id="d712f-471">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-471">This property is read-only.</span></span> <span data-ttu-id="d712f-472">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-472">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-473">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d712f-473">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="d712f-474">Int32</span><span class="sxs-lookup"><span data-stu-id="d712f-474">Int32</span></span>|<span data-ttu-id="d712f-475">Contagem de malwares remediados para este dispositivo windows.</span><span class="sxs-lookup"><span data-stu-id="d712f-475">Count of remediated malware for this windows device.</span></span> <span data-ttu-id="d712f-476">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-476">This property is read-only.</span></span> <span data-ttu-id="d712f-477">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-477">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-478">notes</span><span class="sxs-lookup"><span data-stu-id="d712f-478">notes</span></span>|<span data-ttu-id="d712f-479">String</span><span class="sxs-lookup"><span data-stu-id="d712f-479">String</span></span>|<span data-ttu-id="d712f-480">Observações sobre o dispositivo criado pelo administrador de IT Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-480">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-481">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d712f-481">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="d712f-482">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d712f-482">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="d712f-483">Estado de saúde do cliente do gerenciador de configuração, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-483">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-484">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="d712f-484">configurationManagerClientInformation</span></span>|[<span data-ttu-id="d712f-485">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="d712f-485">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="d712f-486">Informações do cliente do Gerenciador de Configurações, válidas apenas para dispositivos gerenciados, gerenciados pelo duelo ou gerenciados pelo Agente ConfigMgr Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-486">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-487">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="d712f-487">ethernetMacAddress</span></span>|<span data-ttu-id="d712f-488">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-488">String</span></span>|<span data-ttu-id="d712f-489">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="d712f-489">Ethernet MAC.</span></span> <span data-ttu-id="d712f-490">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-490">This property is read-only.</span></span> <span data-ttu-id="d712f-491">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-491">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-492">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="d712f-492">physicalMemoryInBytes</span></span>|<span data-ttu-id="d712f-493">Int64</span><span class="sxs-lookup"><span data-stu-id="d712f-493">Int64</span></span>|<span data-ttu-id="d712f-494">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="d712f-494">Total Memory in Bytes.</span></span> <span data-ttu-id="d712f-495">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-495">This property is read-only.</span></span> <span data-ttu-id="d712f-496">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-496">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-497">processorArchitecture</span><span class="sxs-lookup"><span data-stu-id="d712f-497">processorArchitecture</span></span>|[<span data-ttu-id="d712f-498">managedDeviceArchitecture</span><span class="sxs-lookup"><span data-stu-id="d712f-498">managedDeviceArchitecture</span></span>](../resources/intune-devices-manageddevicearchitecture.md)|<span data-ttu-id="d712f-499">Arquitetura do processador.</span><span class="sxs-lookup"><span data-stu-id="d712f-499">Processor architecture.</span></span> <span data-ttu-id="d712f-500">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-500">This property is read-only.</span></span> <span data-ttu-id="d712f-501">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-501">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-502">Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span><span class="sxs-lookup"><span data-stu-id="d712f-502">Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.</span></span>|
|<span data-ttu-id="d712f-503">specificationVersion</span><span class="sxs-lookup"><span data-stu-id="d712f-503">specificationVersion</span></span>|<span data-ttu-id="d712f-504">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-504">String</span></span>|<span data-ttu-id="d712f-505">Versão de especificação.</span><span class="sxs-lookup"><span data-stu-id="d712f-505">Specification version.</span></span> <span data-ttu-id="d712f-506">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-506">This property is read-only.</span></span> <span data-ttu-id="d712f-507">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-507">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-508">joinType</span><span class="sxs-lookup"><span data-stu-id="d712f-508">joinType</span></span>|[<span data-ttu-id="d712f-509">joinType</span><span class="sxs-lookup"><span data-stu-id="d712f-509">joinType</span></span>](../resources/intune-devices-jointype.md)|<span data-ttu-id="d712f-510">Tipo de junção de dispositivo Herdado [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-510">Device join type Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-511">Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span><span class="sxs-lookup"><span data-stu-id="d712f-511">Possible values are: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.</span></span>|
|<span data-ttu-id="d712f-512">skuFamily</span><span class="sxs-lookup"><span data-stu-id="d712f-512">skuFamily</span></span>|<span data-ttu-id="d712f-513">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d712f-513">String</span></span>|<span data-ttu-id="d712f-514">Família sku de dispositivo Herdada [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-514">Device sku family Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-515">skuNumber</span><span class="sxs-lookup"><span data-stu-id="d712f-515">skuNumber</span></span>|<span data-ttu-id="d712f-516">Int32</span><span class="sxs-lookup"><span data-stu-id="d712f-516">Int32</span></span>|<span data-ttu-id="d712f-517">Número sku do dispositivo, consulte também: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo .</span><span class="sxs-lookup"><span data-stu-id="d712f-517">Device sku number, see also: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo.</span></span> <span data-ttu-id="d712f-518">Valores válidos de 0 a 2147483647.</span><span class="sxs-lookup"><span data-stu-id="d712f-518">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="d712f-519">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d712f-519">This property is read-only.</span></span> <span data-ttu-id="d712f-520">Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d712f-520">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d712f-521">managementFeatures</span><span class="sxs-lookup"><span data-stu-id="d712f-521">managementFeatures</span></span>|[<span data-ttu-id="d712f-522">managedDeviceManagementFeatures</span><span class="sxs-lookup"><span data-stu-id="d712f-522">managedDeviceManagementFeatures</span></span>](../resources/intune-devices-manageddevicemanagementfeatures.md)|<span data-ttu-id="d712f-523">Recursos de gerenciamento de dispositivo Herdados [de managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d712f-523">Device management features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d712f-524">Os valores possíveis são: `none` e `microsoftManagedDesktop`.</span><span class="sxs-lookup"><span data-stu-id="d712f-524">Possible values are: `none`, `microsoftManagedDesktop`.</span></span>|



## <a name="response"></a><span data-ttu-id="d712f-525">Resposta</span><span class="sxs-lookup"><span data-stu-id="d712f-525">Response</span></span>
<span data-ttu-id="d712f-526">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d712f-526">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d712f-527">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d712f-527">Example</span></span>

### <a name="request"></a><span data-ttu-id="d712f-528">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d712f-528">Request</span></span>
<span data-ttu-id="d712f-529">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d712f-529">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
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
  "managementFeatures": "microsoftManagedDesktop"
}
```

### <a name="response"></a><span data-ttu-id="d712f-530">Resposta</span><span class="sxs-lookup"><span data-stu-id="d712f-530">Response</span></span>
<span data-ttu-id="d712f-p175">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d712f-p175">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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
  "managementFeatures": "microsoftManagedDesktop"
}
```




