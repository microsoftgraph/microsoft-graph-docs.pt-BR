---
title: Atualizar windowsManagedDevice
description: Atualize as propriedades de um objeto windowsManagedDevice.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7cef925cc73e28aabe15c29f28676f7c3adfc338
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822726"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="d6017-103">Atualizar windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="d6017-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="d6017-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6017-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6017-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6017-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6017-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6017-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6017-107">Atualize as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="d6017-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6017-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6017-108">Prerequisites</span></span>
<span data-ttu-id="d6017-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6017-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6017-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6017-111">Permission type</span></span>|<span data-ttu-id="d6017-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6017-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6017-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6017-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6017-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6017-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6017-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6017-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6017-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6017-116">Not supported.</span></span>|
|<span data-ttu-id="d6017-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6017-117">Application</span></span>|<span data-ttu-id="d6017-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6017-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6017-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6017-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="d6017-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6017-120">Request headers</span></span>
|<span data-ttu-id="d6017-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6017-121">Header</span></span>|<span data-ttu-id="d6017-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d6017-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6017-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6017-123">Authorization</span></span>|<span data-ttu-id="d6017-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6017-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6017-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6017-125">Accept</span></span>|<span data-ttu-id="d6017-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6017-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6017-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6017-127">Request body</span></span>
<span data-ttu-id="d6017-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="d6017-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="d6017-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="d6017-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6017-130">Property</span></span>|<span data-ttu-id="d6017-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6017-131">Type</span></span>|<span data-ttu-id="d6017-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6017-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6017-133">id</span><span class="sxs-lookup"><span data-stu-id="d6017-133">id</span></span>|<span data-ttu-id="d6017-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-134">String</span></span>|<span data-ttu-id="d6017-135">Identificador exclusivo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-136">userId</span><span class="sxs-lookup"><span data-stu-id="d6017-136">userId</span></span>|<span data-ttu-id="d6017-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-137">String</span></span>|<span data-ttu-id="d6017-138">Identificador exclusivo para o usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="d6017-139">deviceName</span></span>|<span data-ttu-id="d6017-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-140">String</span></span>|<span data-ttu-id="d6017-141">Nome do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d6017-142">hardwareInformation</span></span>|[<span data-ttu-id="d6017-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d6017-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="d6017-144">Os detalhes de hardware do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-144">The hardward details for the device.</span></span>  <span data-ttu-id="d6017-145">Inclui informações como o espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="d6017-146">ownerType</span></span>|[<span data-ttu-id="d6017-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="d6017-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="d6017-148">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-148">Ownership of the device.</span></span> <span data-ttu-id="d6017-149">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d6017-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d6017-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d6017-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d6017-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d6017-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="d6017-153">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-153">Ownership of the device.</span></span> <span data-ttu-id="d6017-154">Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-155">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d6017-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d6017-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d6017-156">deviceActionResults</span></span>|<span data-ttu-id="d6017-157">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d6017-158">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="d6017-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="d6017-159">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-160">managementState</span><span class="sxs-lookup"><span data-stu-id="d6017-160">managementState</span></span>|[<span data-ttu-id="d6017-161">managementState</span><span class="sxs-lookup"><span data-stu-id="d6017-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="d6017-162">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-162">Management state of the device.</span></span> <span data-ttu-id="d6017-163">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-164">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="d6017-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="d6017-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d6017-165">enrolledDateTime</span></span>|<span data-ttu-id="d6017-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-166">DateTimeOffset</span></span>|<span data-ttu-id="d6017-167">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-167">Enrollment time of the device.</span></span> <span data-ttu-id="d6017-168">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d6017-169">lastSyncDateTime</span></span>|<span data-ttu-id="d6017-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-170">DateTimeOffset</span></span>|<span data-ttu-id="d6017-171">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="d6017-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="d6017-172">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="d6017-173">chassisType</span></span>|[<span data-ttu-id="d6017-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="d6017-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="d6017-175">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-175">Chassis type of the device.</span></span> <span data-ttu-id="d6017-176">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-177">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="d6017-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="d6017-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d6017-178">operatingSystem</span></span>|<span data-ttu-id="d6017-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-179">String</span></span>|<span data-ttu-id="d6017-180">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-180">Operating system of the device.</span></span> <span data-ttu-id="d6017-181">Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="d6017-182">deviceType</span></span>|[<span data-ttu-id="d6017-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="d6017-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d6017-184">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-184">Platform of the device.</span></span> <span data-ttu-id="d6017-185">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-186">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d6017-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d6017-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="d6017-187">complianceState</span></span>|[<span data-ttu-id="d6017-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="d6017-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d6017-189">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-189">Compliance state of the device.</span></span> <span data-ttu-id="d6017-190">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-191">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="d6017-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d6017-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d6017-192">jailBroken</span></span>|<span data-ttu-id="d6017-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-193">String</span></span>|<span data-ttu-id="d6017-194">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="d6017-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="d6017-195">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d6017-196">managementAgent</span></span>|[<span data-ttu-id="d6017-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d6017-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="d6017-198">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-198">Management channel of the device.</span></span> <span data-ttu-id="d6017-199">Intune, EAS, etc. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-200">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="d6017-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="d6017-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="d6017-201">osVersion</span></span>|<span data-ttu-id="d6017-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-202">String</span></span>|<span data-ttu-id="d6017-203">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-203">Operating system version of the device.</span></span> <span data-ttu-id="d6017-204">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="d6017-205">easActivated</span></span>|<span data-ttu-id="d6017-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-206">Boolean</span></span>|<span data-ttu-id="d6017-207">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d6017-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="d6017-208">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d6017-209">easDeviceId</span></span>|<span data-ttu-id="d6017-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-210">String</span></span>|<span data-ttu-id="d6017-211">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="d6017-212">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d6017-213">easActivationDateTime</span></span>|<span data-ttu-id="d6017-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-214">DateTimeOffset</span></span>|<span data-ttu-id="d6017-215">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="d6017-216">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="d6017-217">aadRegistered</span></span>|<span data-ttu-id="d6017-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-218">Boolean</span></span>|<span data-ttu-id="d6017-219">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6017-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d6017-220">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d6017-221">azureADRegistered</span></span>|<span data-ttu-id="d6017-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-222">Boolean</span></span>|<span data-ttu-id="d6017-223">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6017-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d6017-224">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d6017-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="d6017-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d6017-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d6017-227">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-227">Enrollment type of the device.</span></span> <span data-ttu-id="d6017-228">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-229">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="d6017-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d6017-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d6017-230">lostModeState</span></span>|[<span data-ttu-id="d6017-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d6017-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="d6017-232">Indica se o modo perdido está habilitado ou desabilitada Inherited em [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-233">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="d6017-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d6017-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d6017-234">activationLockBypassCode</span></span>|<span data-ttu-id="d6017-235">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-235">String</span></span>|<span data-ttu-id="d6017-236">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="d6017-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="d6017-237">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d6017-238">emailAddress</span></span>|<span data-ttu-id="d6017-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-239">String</span></span>|<span data-ttu-id="d6017-240">O usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md) email(s)</span><span class="sxs-lookup"><span data-stu-id="d6017-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="d6017-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d6017-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-242">String</span></span>|<span data-ttu-id="d6017-243">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6017-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d6017-244">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6017-244">Read only.</span></span> <span data-ttu-id="d6017-245">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d6017-246">azureADDeviceId</span></span>|<span data-ttu-id="d6017-247">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-247">String</span></span>|<span data-ttu-id="d6017-248">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6017-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d6017-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6017-249">Read only.</span></span> <span data-ttu-id="d6017-250">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d6017-251">deviceRegistrationState</span></span>|[<span data-ttu-id="d6017-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d6017-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d6017-253">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-253">Device registration state.</span></span> <span data-ttu-id="d6017-254">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-255">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d6017-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d6017-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6017-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d6017-257">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-257">String</span></span>|<span data-ttu-id="d6017-258">Nome de exibição de categoria dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d6017-259">isSupervised</span></span>|<span data-ttu-id="d6017-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-260">Boolean</span></span>|<span data-ttu-id="d6017-261">Status do dispositivo supervisionado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d6017-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d6017-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-263">DateTimeOffset</span></span>|<span data-ttu-id="d6017-264">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6017-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="d6017-265">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d6017-266">exchangeAccessState</span></span>|[<span data-ttu-id="d6017-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d6017-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d6017-268">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6017-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d6017-269">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-270">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="d6017-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d6017-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d6017-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d6017-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d6017-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d6017-273">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6017-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d6017-274">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-275">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="d6017-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d6017-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d6017-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d6017-277">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-277">String</span></span>|<span data-ttu-id="d6017-278">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="d6017-279">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d6017-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d6017-281">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-281">String</span></span>|<span data-ttu-id="d6017-282">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="d6017-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="d6017-283">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d6017-284">isEncrypted</span></span>|<span data-ttu-id="d6017-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-285">Boolean</span></span>|<span data-ttu-id="d6017-286">Status de criptografia do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6017-287">userPrincipalName</span></span>|<span data-ttu-id="d6017-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-288">String</span></span>|<span data-ttu-id="d6017-289">Dispositivo nome principal de usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-290">modelo</span><span class="sxs-lookup"><span data-stu-id="d6017-290">model</span></span>|<span data-ttu-id="d6017-291">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-291">String</span></span>|<span data-ttu-id="d6017-292">Modelo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-293">fabricante</span><span class="sxs-lookup"><span data-stu-id="d6017-293">manufacturer</span></span>|<span data-ttu-id="d6017-294">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-294">String</span></span>|<span data-ttu-id="d6017-295">Fabricante do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-296">imei</span><span class="sxs-lookup"><span data-stu-id="d6017-296">imei</span></span>|<span data-ttu-id="d6017-297">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-297">String</span></span>|<span data-ttu-id="d6017-298">IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d6017-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d6017-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-300">DateTimeOffset</span></span>|<span data-ttu-id="d6017-301">A data e hora quando o período de carência de conformidade do dispositivo expiram Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d6017-302">serialNumber</span></span>|<span data-ttu-id="d6017-303">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-303">String</span></span>|<span data-ttu-id="d6017-304">SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d6017-305">phoneNumber</span></span>|<span data-ttu-id="d6017-306">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-306">String</span></span>|<span data-ttu-id="d6017-307">Número de telefone do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d6017-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d6017-309">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-309">String</span></span>|<span data-ttu-id="d6017-310">Nível de patch de segurança Android Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6017-311">userDisplayName</span></span>|<span data-ttu-id="d6017-312">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-312">String</span></span>|<span data-ttu-id="d6017-313">Nome de exibição do usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d6017-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d6017-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d6017-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d6017-316">Cliente de ConfigrMgr habilitado recursos Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d6017-317">wiFiMacAddress</span></span>|<span data-ttu-id="d6017-318">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-318">String</span></span>|<span data-ttu-id="d6017-319">Wi-Fi MAC herdada do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d6017-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d6017-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d6017-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d6017-322">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-322">The device health attestation state.</span></span> <span data-ttu-id="d6017-323">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d6017-324">subscriberCarrier</span></span>|<span data-ttu-id="d6017-325">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-325">String</span></span>|<span data-ttu-id="d6017-326">Herdado de operadora de assinante de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-327">meid</span><span class="sxs-lookup"><span data-stu-id="d6017-327">meid</span></span>|<span data-ttu-id="d6017-328">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-328">String</span></span>|<span data-ttu-id="d6017-329">MEID herdados de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d6017-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d6017-331">Int64</span><span class="sxs-lookup"><span data-stu-id="d6017-331">Int64</span></span>|<span data-ttu-id="d6017-332">Armazenamento total em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d6017-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d6017-334">Int64</span><span class="sxs-lookup"><span data-stu-id="d6017-334">Int64</span></span>|<span data-ttu-id="d6017-335">Armazenamento gratuito em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d6017-336">managedDeviceName</span></span>|<span data-ttu-id="d6017-337">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-337">String</span></span>|<span data-ttu-id="d6017-338">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d6017-339">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d6017-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="d6017-340">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d6017-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="d6017-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="d6017-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d6017-343">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d6017-344">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6017-344">Read Only.</span></span> <span data-ttu-id="d6017-345">Herdada do [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d6017-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d6017-346">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="d6017-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="d6017-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="d6017-347">usersLoggedOn</span></span>|<span data-ttu-id="d6017-348">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="d6017-349">Indica o último logon usuários de um dispositivo Inherited da [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6017-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="d6017-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-351">DateTimeOffset</span></span>|<span data-ttu-id="d6017-352">Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="d6017-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="d6017-353">Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="d6017-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="d6017-354">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6017-354">Read Only.</span></span> <span data-ttu-id="d6017-355">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="d6017-356">autopilotEnrolled</span></span>|<span data-ttu-id="d6017-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-357">Boolean</span></span>|<span data-ttu-id="d6017-358">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="d6017-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="d6017-359">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="d6017-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="d6017-361">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6017-361">Boolean</span></span>|<span data-ttu-id="d6017-362">Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6017-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="d6017-363">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d6017-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="d6017-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6017-365">DateTimeOffset</span></span>|<span data-ttu-id="d6017-366">Relatórios de dispositivo gerenciamento data de validade certificado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-367">iccid</span><span class="sxs-lookup"><span data-stu-id="d6017-367">iccid</span></span>|<span data-ttu-id="d6017-368">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-368">String</span></span>|<span data-ttu-id="d6017-369">Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM.</span><span class="sxs-lookup"><span data-stu-id="d6017-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="d6017-370">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-371">UDID</span><span class="sxs-lookup"><span data-stu-id="d6017-371">udid</span></span>|<span data-ttu-id="d6017-372">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-372">String</span></span>|<span data-ttu-id="d6017-373">Identificador exclusivo do dispositivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="d6017-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="d6017-374">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6017-375">roleScopeTagIds</span></span>|<span data-ttu-id="d6017-376">String collection</span><span class="sxs-lookup"><span data-stu-id="d6017-376">String collection</span></span>|<span data-ttu-id="d6017-377">Lista de IDs de marca de escopo para essa instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6017-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="d6017-378">Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d6017-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="d6017-380">Int32</span><span class="sxs-lookup"><span data-stu-id="d6017-380">Int32</span></span>|<span data-ttu-id="d6017-381">Contagem de malware ativos para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d6017-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="d6017-383">Int32</span><span class="sxs-lookup"><span data-stu-id="d6017-383">Int32</span></span>|<span data-ttu-id="d6017-384">Contagem de malware remediados por teste para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-385">Observações</span><span class="sxs-lookup"><span data-stu-id="d6017-385">notes</span></span>|<span data-ttu-id="d6017-386">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6017-386">String</span></span>|<span data-ttu-id="d6017-387">Anotações no dispositivo criados pelo administrador de TI herdadas a partir do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d6017-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d6017-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="d6017-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d6017-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="d6017-390">Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados pelo MDM/ConfigMgr herdadas de agente do [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d6017-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d6017-391">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6017-391">Response</span></span>
<span data-ttu-id="d6017-392">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6017-392">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6017-393">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6017-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6017-394">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6017-394">Request</span></span>
<span data-ttu-id="d6017-395">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6017-395">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7114

{
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

### <a name="response"></a><span data-ttu-id="d6017-396">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6017-396">Response</span></span>
<span data-ttu-id="d6017-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6017-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





