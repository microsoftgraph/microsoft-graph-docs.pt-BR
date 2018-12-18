---
title: Criar windowsManagedDevice
description: Crie um novo objeto de windowsManagedDevice.
author: tfitzmac
ms.openlocfilehash: 21626854a52ed305dbf237562e151e168330f170
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324441"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="17ab8-103">Criar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="17ab8-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="17ab8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17ab8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17ab8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17ab8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17ab8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="17ab8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17ab8-107">Crie um novo objeto de [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="17ab8-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17ab8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17ab8-108">Prerequisites</span></span>
<span data-ttu-id="17ab8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17ab8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17ab8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17ab8-111">Permission type</span></span>|<span data-ttu-id="17ab8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17ab8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17ab8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17ab8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17ab8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ab8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="17ab8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17ab8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ab8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17ab8-116">Not supported.</span></span>|
|<span data-ttu-id="17ab8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17ab8-117">Application</span></span>|<span data-ttu-id="17ab8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17ab8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17ab8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17ab8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="17ab8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17ab8-120">Request headers</span></span>
|<span data-ttu-id="17ab8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17ab8-121">Header</span></span>|<span data-ttu-id="17ab8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17ab8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17ab8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17ab8-123">Authorization</span></span>|<span data-ttu-id="17ab8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17ab8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17ab8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17ab8-125">Accept</span></span>|<span data-ttu-id="17ab8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17ab8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ab8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17ab8-127">Request body</span></span>
<span data-ttu-id="17ab8-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="17ab8-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="17ab8-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="17ab8-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="17ab8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17ab8-130">Property</span></span>|<span data-ttu-id="17ab8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17ab8-131">Type</span></span>|<span data-ttu-id="17ab8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17ab8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ab8-133">id</span><span class="sxs-lookup"><span data-stu-id="17ab8-133">id</span></span>|<span data-ttu-id="17ab8-134">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-134">String</span></span>|<span data-ttu-id="17ab8-135">Identificador exclusivo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-136">userId</span><span class="sxs-lookup"><span data-stu-id="17ab8-136">userId</span></span>|<span data-ttu-id="17ab8-137">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-137">String</span></span>|<span data-ttu-id="17ab8-138">Identificador exclusivo para o usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="17ab8-139">deviceName</span></span>|<span data-ttu-id="17ab8-140">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-140">String</span></span>|<span data-ttu-id="17ab8-141">Nome do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="17ab8-142">hardwareInformation</span></span>|[<span data-ttu-id="17ab8-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="17ab8-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="17ab8-144">Os detalhes de hardware do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-144">The hardward details for the device.</span></span>  <span data-ttu-id="17ab8-145">Inclui informações como o espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="17ab8-146">ownerType</span></span>|[<span data-ttu-id="17ab8-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="17ab8-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="17ab8-148">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-148">Ownership of the device.</span></span> <span data-ttu-id="17ab8-149">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="17ab8-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="17ab8-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="17ab8-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="17ab8-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="17ab8-153">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-153">Ownership of the device.</span></span> <span data-ttu-id="17ab8-154">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-155">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="17ab8-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="17ab8-156">deviceActionResults</span></span>|<span data-ttu-id="17ab8-157">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="17ab8-158">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="17ab8-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="17ab8-159">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-160">managementState</span><span class="sxs-lookup"><span data-stu-id="17ab8-160">managementState</span></span>|[<span data-ttu-id="17ab8-161">managementState</span><span class="sxs-lookup"><span data-stu-id="17ab8-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="17ab8-162">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-162">Management state of the device.</span></span> <span data-ttu-id="17ab8-163">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-164">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="17ab8-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="17ab8-165">enrolledDateTime</span></span>|<span data-ttu-id="17ab8-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-166">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-167">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-167">Enrollment time of the device.</span></span> <span data-ttu-id="17ab8-168">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="17ab8-169">lastSyncDateTime</span></span>|<span data-ttu-id="17ab8-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-170">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-171">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="17ab8-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="17ab8-172">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="17ab8-173">chassisType</span></span>|[<span data-ttu-id="17ab8-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="17ab8-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="17ab8-175">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-175">Chassis type of the device.</span></span> <span data-ttu-id="17ab8-176">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-177">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="17ab8-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="17ab8-178">operatingSystem</span></span>|<span data-ttu-id="17ab8-179">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-179">String</span></span>|<span data-ttu-id="17ab8-180">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-180">Operating system of the device.</span></span> <span data-ttu-id="17ab8-181">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="17ab8-182">deviceType</span></span>|[<span data-ttu-id="17ab8-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="17ab8-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="17ab8-184">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-184">Platform of the device.</span></span> <span data-ttu-id="17ab8-185">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-186">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="17ab8-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="17ab8-187">complianceState</span></span>|[<span data-ttu-id="17ab8-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="17ab8-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="17ab8-189">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-189">Compliance state of the device.</span></span> <span data-ttu-id="17ab8-190">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-191">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="17ab8-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="17ab8-192">jailBroken</span></span>|<span data-ttu-id="17ab8-193">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-193">String</span></span>|<span data-ttu-id="17ab8-194">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="17ab8-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="17ab8-195">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="17ab8-196">managementAgent</span></span>|[<span data-ttu-id="17ab8-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="17ab8-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="17ab8-198">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-198">Management channel of the device.</span></span> <span data-ttu-id="17ab8-199">Intune, EAS, etc. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-200">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="17ab8-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="17ab8-201">osVersion</span></span>|<span data-ttu-id="17ab8-202">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-202">String</span></span>|<span data-ttu-id="17ab8-203">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-203">Operating system version of the device.</span></span> <span data-ttu-id="17ab8-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="17ab8-205">easActivated</span></span>|<span data-ttu-id="17ab8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-206">Boolean</span></span>|<span data-ttu-id="17ab8-207">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="17ab8-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="17ab8-208">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="17ab8-209">easDeviceId</span></span>|<span data-ttu-id="17ab8-210">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-210">String</span></span>|<span data-ttu-id="17ab8-211">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="17ab8-212">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="17ab8-213">easActivationDateTime</span></span>|<span data-ttu-id="17ab8-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-214">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-215">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="17ab8-216">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="17ab8-217">aadRegistered</span></span>|<span data-ttu-id="17ab8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-218">Boolean</span></span>|<span data-ttu-id="17ab8-219">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="17ab8-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="17ab8-220">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="17ab8-221">azureADRegistered</span></span>|<span data-ttu-id="17ab8-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-222">Boolean</span></span>|<span data-ttu-id="17ab8-223">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="17ab8-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="17ab8-224">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="17ab8-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="17ab8-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="17ab8-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="17ab8-227">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-227">Enrollment type of the device.</span></span> <span data-ttu-id="17ab8-228">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-229">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="17ab8-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="17ab8-230">lostModeState</span></span>|[<span data-ttu-id="17ab8-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="17ab8-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="17ab8-232">Indica se o modo perdido está habilitado ou desabilitada Inherited em [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-233">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="17ab8-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="17ab8-234">activationLockBypassCode</span></span>|<span data-ttu-id="17ab8-235">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-235">String</span></span>|<span data-ttu-id="17ab8-236">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="17ab8-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="17ab8-237">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="17ab8-238">emailAddress</span></span>|<span data-ttu-id="17ab8-239">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-239">String</span></span>|<span data-ttu-id="17ab8-240">O usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md) email(s)</span><span class="sxs-lookup"><span data-stu-id="17ab8-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="17ab8-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="17ab8-242">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-242">String</span></span>|<span data-ttu-id="17ab8-243">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="17ab8-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="17ab8-244">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17ab8-244">Read only.</span></span> <span data-ttu-id="17ab8-245">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="17ab8-246">azureADDeviceId</span></span>|<span data-ttu-id="17ab8-247">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-247">String</span></span>|<span data-ttu-id="17ab8-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="17ab8-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="17ab8-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17ab8-249">Read only.</span></span> <span data-ttu-id="17ab8-250">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="17ab8-251">deviceRegistrationState</span></span>|[<span data-ttu-id="17ab8-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="17ab8-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="17ab8-253">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-253">Device registration state.</span></span> <span data-ttu-id="17ab8-254">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-255">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="17ab8-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="17ab8-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="17ab8-257">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-257">String</span></span>|<span data-ttu-id="17ab8-258">Nome de exibição de categoria dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="17ab8-259">isSupervised</span></span>|<span data-ttu-id="17ab8-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-260">Boolean</span></span>|<span data-ttu-id="17ab8-261">Status do dispositivo supervisionado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="17ab8-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="17ab8-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-263">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-264">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ab8-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="17ab8-265">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="17ab8-266">exchangeAccessState</span></span>|[<span data-ttu-id="17ab8-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="17ab8-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="17ab8-268">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ab8-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="17ab8-269">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-270">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="17ab8-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="17ab8-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="17ab8-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="17ab8-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="17ab8-273">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="17ab8-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="17ab8-274">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-275">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="17ab8-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="17ab8-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="17ab8-277">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-277">String</span></span>|<span data-ttu-id="17ab8-278">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="17ab8-279">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="17ab8-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="17ab8-281">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-281">String</span></span>|<span data-ttu-id="17ab8-282">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="17ab8-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="17ab8-283">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="17ab8-284">isEncrypted</span></span>|<span data-ttu-id="17ab8-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-285">Boolean</span></span>|<span data-ttu-id="17ab8-286">Status de criptografia do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="17ab8-287">userPrincipalName</span></span>|<span data-ttu-id="17ab8-288">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-288">String</span></span>|<span data-ttu-id="17ab8-289">Dispositivo nome principal de usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-290">modelo</span><span class="sxs-lookup"><span data-stu-id="17ab8-290">model</span></span>|<span data-ttu-id="17ab8-291">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-291">String</span></span>|<span data-ttu-id="17ab8-292">Modelo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-293">fabricante</span><span class="sxs-lookup"><span data-stu-id="17ab8-293">manufacturer</span></span>|<span data-ttu-id="17ab8-294">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-294">String</span></span>|<span data-ttu-id="17ab8-295">Fabricante do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-296">imei</span><span class="sxs-lookup"><span data-stu-id="17ab8-296">imei</span></span>|<span data-ttu-id="17ab8-297">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-297">String</span></span>|<span data-ttu-id="17ab8-298">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="17ab8-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="17ab8-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-300">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-301">A data e hora quando o período de carência de conformidade do dispositivo expiram Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="17ab8-302">serialNumber</span></span>|<span data-ttu-id="17ab8-303">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-303">String</span></span>|<span data-ttu-id="17ab8-304">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="17ab8-305">phoneNumber</span></span>|<span data-ttu-id="17ab8-306">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-306">String</span></span>|<span data-ttu-id="17ab8-307">Número de telefone do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="17ab8-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="17ab8-309">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-309">String</span></span>|<span data-ttu-id="17ab8-310">Nível de patch de segurança Android Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="17ab8-311">userDisplayName</span></span>|<span data-ttu-id="17ab8-312">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-312">String</span></span>|<span data-ttu-id="17ab8-313">Nome de exibição do usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="17ab8-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="17ab8-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="17ab8-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="17ab8-316">Cliente de ConfigrMgr habilitado recursos Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="17ab8-317">wiFiMacAddress</span></span>|<span data-ttu-id="17ab8-318">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-318">String</span></span>|<span data-ttu-id="17ab8-319">Wi-Fi MAC herdada do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="17ab8-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="17ab8-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="17ab8-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="17ab8-322">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-322">The device health attestation state.</span></span> <span data-ttu-id="17ab8-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="17ab8-324">subscriberCarrier</span></span>|<span data-ttu-id="17ab8-325">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-325">String</span></span>|<span data-ttu-id="17ab8-326">Herdado de operadora de assinante de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-327">meid</span><span class="sxs-lookup"><span data-stu-id="17ab8-327">meid</span></span>|<span data-ttu-id="17ab8-328">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-328">String</span></span>|<span data-ttu-id="17ab8-329">MEID herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="17ab8-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="17ab8-331">Int64</span><span class="sxs-lookup"><span data-stu-id="17ab8-331">Int64</span></span>|<span data-ttu-id="17ab8-332">Armazenamento total em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="17ab8-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="17ab8-334">Int64</span><span class="sxs-lookup"><span data-stu-id="17ab8-334">Int64</span></span>|<span data-ttu-id="17ab8-335">Armazenamento gratuito em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="17ab8-336">managedDeviceName</span></span>|<span data-ttu-id="17ab8-337">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-337">String</span></span>|<span data-ttu-id="17ab8-338">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="17ab8-339">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="17ab8-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="17ab8-340">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="17ab8-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="17ab8-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="17ab8-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="17ab8-343">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="17ab8-344">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17ab8-344">Read Only.</span></span> <span data-ttu-id="17ab8-345">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="17ab8-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="17ab8-346">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="17ab8-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="17ab8-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="17ab8-347">usersLoggedOn</span></span>|<span data-ttu-id="17ab8-348">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="17ab8-349">Indica o último logon usuários de um dispositivo Inherited da [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="17ab8-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="17ab8-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-351">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-352">Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="17ab8-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="17ab8-353">Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="17ab8-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="17ab8-354">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17ab8-354">Read Only.</span></span> <span data-ttu-id="17ab8-355">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="17ab8-356">autopilotEnrolled</span></span>|<span data-ttu-id="17ab8-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-357">Boolean</span></span>|<span data-ttu-id="17ab8-358">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="17ab8-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="17ab8-359">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="17ab8-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="17ab8-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ab8-361">Boolean</span></span>|<span data-ttu-id="17ab8-362">Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="17ab8-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="17ab8-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="17ab8-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="17ab8-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ab8-365">DateTimeOffset</span></span>|<span data-ttu-id="17ab8-366">Relatórios de dispositivo gerenciamento data de validade certificado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-367">iccid</span><span class="sxs-lookup"><span data-stu-id="17ab8-367">iccid</span></span>|<span data-ttu-id="17ab8-368">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-368">String</span></span>|<span data-ttu-id="17ab8-369">Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM.</span><span class="sxs-lookup"><span data-stu-id="17ab8-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="17ab8-370">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-371">UDID</span><span class="sxs-lookup"><span data-stu-id="17ab8-371">udid</span></span>|<span data-ttu-id="17ab8-372">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-372">String</span></span>|<span data-ttu-id="17ab8-373">Identificador exclusivo do dispositivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="17ab8-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="17ab8-374">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17ab8-375">roleScopeTagIds</span></span>|<span data-ttu-id="17ab8-376">String collection</span><span class="sxs-lookup"><span data-stu-id="17ab8-376">String collection</span></span>|<span data-ttu-id="17ab8-377">Lista de IDs de marca de escopo para essa instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17ab8-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="17ab8-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="17ab8-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="17ab8-380">Int32</span><span class="sxs-lookup"><span data-stu-id="17ab8-380">Int32</span></span>|<span data-ttu-id="17ab8-381">Contagem de malware ativos para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="17ab8-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="17ab8-383">Int32</span><span class="sxs-lookup"><span data-stu-id="17ab8-383">Int32</span></span>|<span data-ttu-id="17ab8-384">Contagem de malware remediados por teste para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-385">Observações</span><span class="sxs-lookup"><span data-stu-id="17ab8-385">notes</span></span>|<span data-ttu-id="17ab8-386">String</span><span class="sxs-lookup"><span data-stu-id="17ab8-386">String</span></span>|<span data-ttu-id="17ab8-387">Anotações no dispositivo criados pelo administrador de TI herdadas a partir do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="17ab8-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="17ab8-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="17ab8-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="17ab8-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="17ab8-390">Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados pelo MDM/ConfigMgr herdadas de agente do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="17ab8-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="17ab8-391">Resposta</span><span class="sxs-lookup"><span data-stu-id="17ab8-391">Response</span></span>
<span data-ttu-id="17ab8-392">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17ab8-392">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ab8-393">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17ab8-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="17ab8-394">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17ab8-394">Request</span></span>
<span data-ttu-id="17ab8-395">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17ab8-395">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7173

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
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
    "windowsUpdateForBusiness": true
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
  }
}
```

### <a name="response"></a><span data-ttu-id="17ab8-396">Resposta</span><span class="sxs-lookup"><span data-stu-id="17ab8-396">Response</span></span>
<span data-ttu-id="17ab8-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17ab8-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7222

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
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
    "windowsUpdateForBusiness": true
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
  }
}
```





