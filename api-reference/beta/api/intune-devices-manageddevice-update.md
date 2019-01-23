---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 525623c99d8f3238ee548e634bc7ffe2c3162111
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404383"
---
# <a name="update-manageddevice"></a><span data-ttu-id="27cad-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="27cad-103">Update managedDevice</span></span>

> <span data-ttu-id="27cad-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="27cad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27cad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27cad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27cad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="27cad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27cad-107">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="27cad-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27cad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27cad-108">Prerequisites</span></span>
<span data-ttu-id="27cad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="27cad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="27cad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27cad-111">Permission type</span></span>|<span data-ttu-id="27cad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27cad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27cad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27cad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27cad-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27cad-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27cad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27cad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27cad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27cad-116">Not supported.</span></span>|
|<span data-ttu-id="27cad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27cad-117">Application</span></span>|<span data-ttu-id="27cad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27cad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27cad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27cad-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="27cad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27cad-120">Request headers</span></span>
|<span data-ttu-id="27cad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27cad-121">Header</span></span>|<span data-ttu-id="27cad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27cad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27cad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27cad-123">Authorization</span></span>|<span data-ttu-id="27cad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27cad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27cad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27cad-125">Accept</span></span>|<span data-ttu-id="27cad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27cad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27cad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27cad-127">Request body</span></span>
<span data-ttu-id="27cad-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="27cad-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="27cad-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="27cad-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="27cad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27cad-130">Property</span></span>|<span data-ttu-id="27cad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27cad-131">Type</span></span>|<span data-ttu-id="27cad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27cad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27cad-133">id</span><span class="sxs-lookup"><span data-stu-id="27cad-133">id</span></span>|<span data-ttu-id="27cad-134">String</span><span class="sxs-lookup"><span data-stu-id="27cad-134">String</span></span>|<span data-ttu-id="27cad-135">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-135">Unique Identifier for the device</span></span>|
|<span data-ttu-id="27cad-136">userId</span><span class="sxs-lookup"><span data-stu-id="27cad-136">userId</span></span>|<span data-ttu-id="27cad-137">String</span><span class="sxs-lookup"><span data-stu-id="27cad-137">String</span></span>|<span data-ttu-id="27cad-138">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-138">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="27cad-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="27cad-139">deviceName</span></span>|<span data-ttu-id="27cad-140">String</span><span class="sxs-lookup"><span data-stu-id="27cad-140">String</span></span>|<span data-ttu-id="27cad-141">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-141">Name of the device</span></span>|
|<span data-ttu-id="27cad-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="27cad-142">hardwareInformation</span></span>|[<span data-ttu-id="27cad-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="27cad-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="27cad-144">Os detalhes de hardware do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-144">The hardward details for the device.</span></span>  <span data-ttu-id="27cad-145">Inclui informações como o espaço de armazenamento, fabricante, número de série, etc.</span><span class="sxs-lookup"><span data-stu-id="27cad-145">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="27cad-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="27cad-146">ownerType</span></span>|[<span data-ttu-id="27cad-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="27cad-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="27cad-148">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-148">Ownership of the device.</span></span> <span data-ttu-id="27cad-149">Pode ser 'empresa' ou 'pessoal'.</span><span class="sxs-lookup"><span data-stu-id="27cad-149">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="27cad-150">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="27cad-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="27cad-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="27cad-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="27cad-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="27cad-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="27cad-153">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-153">Ownership of the device.</span></span> <span data-ttu-id="27cad-154">Pode ser 'empresa' ou 'pessoal'.</span><span class="sxs-lookup"><span data-stu-id="27cad-154">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="27cad-155">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="27cad-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="27cad-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="27cad-156">deviceActionResults</span></span>|<span data-ttu-id="27cad-157">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="27cad-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="27cad-158">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="27cad-158">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="27cad-159">managementState</span><span class="sxs-lookup"><span data-stu-id="27cad-159">managementState</span></span>|[<span data-ttu-id="27cad-160">managementState</span><span class="sxs-lookup"><span data-stu-id="27cad-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="27cad-161">Estado de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-161">Management state of the device.</span></span> <span data-ttu-id="27cad-162">Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span><span class="sxs-lookup"><span data-stu-id="27cad-162">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="27cad-163">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="27cad-163">enrolledDateTime</span></span>|<span data-ttu-id="27cad-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-164">DateTimeOffset</span></span>|<span data-ttu-id="27cad-165">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-165">Enrollment time of the device.</span></span>|
|<span data-ttu-id="27cad-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="27cad-166">lastSyncDateTime</span></span>|<span data-ttu-id="27cad-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-167">DateTimeOffset</span></span>|<span data-ttu-id="27cad-168">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="27cad-168">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="27cad-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="27cad-169">chassisType</span></span>|[<span data-ttu-id="27cad-170">chassisType</span><span class="sxs-lookup"><span data-stu-id="27cad-170">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="27cad-171">Tipo de chassi do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-171">Chassis type of the device.</span></span> <span data-ttu-id="27cad-172">Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="27cad-172">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="27cad-173">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="27cad-173">operatingSystem</span></span>|<span data-ttu-id="27cad-174">String</span><span class="sxs-lookup"><span data-stu-id="27cad-174">String</span></span>|<span data-ttu-id="27cad-175">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-175">Operating system of the device.</span></span> <span data-ttu-id="27cad-176">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="27cad-176">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="27cad-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="27cad-177">deviceType</span></span>|[<span data-ttu-id="27cad-178">deviceType</span><span class="sxs-lookup"><span data-stu-id="27cad-178">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="27cad-179">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-179">Platform of the device.</span></span> <span data-ttu-id="27cad-180">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="27cad-180">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="27cad-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="27cad-181">complianceState</span></span>|[<span data-ttu-id="27cad-182">complianceState</span><span class="sxs-lookup"><span data-stu-id="27cad-182">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="27cad-183">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-183">Compliance state of the device.</span></span> <span data-ttu-id="27cad-184">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="27cad-184">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="27cad-185">jailBroken</span><span class="sxs-lookup"><span data-stu-id="27cad-185">jailBroken</span></span>|<span data-ttu-id="27cad-186">String</span><span class="sxs-lookup"><span data-stu-id="27cad-186">String</span></span>|<span data-ttu-id="27cad-187">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="27cad-187">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="27cad-188">managementAgent</span><span class="sxs-lookup"><span data-stu-id="27cad-188">managementAgent</span></span>|[<span data-ttu-id="27cad-189">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="27cad-189">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="27cad-190">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-190">Management channel of the device.</span></span> <span data-ttu-id="27cad-191">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="27cad-191">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="27cad-192">osVersion</span><span class="sxs-lookup"><span data-stu-id="27cad-192">osVersion</span></span>|<span data-ttu-id="27cad-193">String</span><span class="sxs-lookup"><span data-stu-id="27cad-193">String</span></span>|<span data-ttu-id="27cad-194">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-194">Operating system version of the device.</span></span>|
|<span data-ttu-id="27cad-195">easActivated</span><span class="sxs-lookup"><span data-stu-id="27cad-195">easActivated</span></span>|<span data-ttu-id="27cad-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-196">Boolean</span></span>|<span data-ttu-id="27cad-197">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="27cad-197">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="27cad-198">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="27cad-198">easDeviceId</span></span>|<span data-ttu-id="27cad-199">String</span><span class="sxs-lookup"><span data-stu-id="27cad-199">String</span></span>|<span data-ttu-id="27cad-200">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-200">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="27cad-201">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="27cad-201">easActivationDateTime</span></span>|<span data-ttu-id="27cad-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-202">DateTimeOffset</span></span>|<span data-ttu-id="27cad-203">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-203">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="27cad-204">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="27cad-204">aadRegistered</span></span>|<span data-ttu-id="27cad-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-205">Boolean</span></span>|<span data-ttu-id="27cad-206">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="27cad-206">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="27cad-207">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="27cad-207">azureADRegistered</span></span>|<span data-ttu-id="27cad-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-208">Boolean</span></span>|<span data-ttu-id="27cad-209">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="27cad-209">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="27cad-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="27cad-210">deviceEnrollmentType</span></span>|[<span data-ttu-id="27cad-211">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="27cad-211">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="27cad-212">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-212">Enrollment type of the device.</span></span> <span data-ttu-id="27cad-213">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="27cad-213">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="27cad-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="27cad-214">lostModeState</span></span>|[<span data-ttu-id="27cad-215">lostModeState</span><span class="sxs-lookup"><span data-stu-id="27cad-215">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="27cad-216">Indica se o modo perdido está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="27cad-216">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="27cad-217">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="27cad-217">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="27cad-218">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="27cad-218">activationLockBypassCode</span></span>|<span data-ttu-id="27cad-219">String</span><span class="sxs-lookup"><span data-stu-id="27cad-219">String</span></span>|<span data-ttu-id="27cad-220">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="27cad-220">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="27cad-221">emailAddress</span><span class="sxs-lookup"><span data-stu-id="27cad-221">emailAddress</span></span>|<span data-ttu-id="27cad-222">String</span><span class="sxs-lookup"><span data-stu-id="27cad-222">String</span></span>|<span data-ttu-id="27cad-223">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-223">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="27cad-224">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="27cad-224">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="27cad-225">String</span><span class="sxs-lookup"><span data-stu-id="27cad-225">String</span></span>|<span data-ttu-id="27cad-226">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="27cad-226">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="27cad-227">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27cad-227">Read only.</span></span>|
|<span data-ttu-id="27cad-228">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="27cad-228">azureADDeviceId</span></span>|<span data-ttu-id="27cad-229">String</span><span class="sxs-lookup"><span data-stu-id="27cad-229">String</span></span>|<span data-ttu-id="27cad-230">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="27cad-230">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="27cad-231">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27cad-231">Read only.</span></span>|
|<span data-ttu-id="27cad-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="27cad-232">deviceRegistrationState</span></span>|[<span data-ttu-id="27cad-233">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="27cad-233">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="27cad-234">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-234">Device registration state.</span></span> <span data-ttu-id="27cad-235">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="27cad-235">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="27cad-236">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="27cad-236">deviceCategoryDisplayName</span></span>|<span data-ttu-id="27cad-237">String</span><span class="sxs-lookup"><span data-stu-id="27cad-237">String</span></span>|<span data-ttu-id="27cad-238">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-238">Device category display name</span></span>|
|<span data-ttu-id="27cad-239">isSupervised</span><span class="sxs-lookup"><span data-stu-id="27cad-239">isSupervised</span></span>|<span data-ttu-id="27cad-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-240">Boolean</span></span>|<span data-ttu-id="27cad-241">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-241">Device supervised status</span></span>|
|<span data-ttu-id="27cad-242">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="27cad-242">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="27cad-243">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-243">DateTimeOffset</span></span>|<span data-ttu-id="27cad-244">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="27cad-244">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="27cad-245">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="27cad-245">exchangeAccessState</span></span>|[<span data-ttu-id="27cad-246">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="27cad-246">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="27cad-247">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="27cad-247">The Access State of the device in Exchange.</span></span> <span data-ttu-id="27cad-248">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="27cad-248">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="27cad-249">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="27cad-249">exchangeAccessStateReason</span></span>|[<span data-ttu-id="27cad-250">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="27cad-250">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="27cad-251">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="27cad-251">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="27cad-252">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="27cad-252">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="27cad-253">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="27cad-253">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="27cad-254">String</span><span class="sxs-lookup"><span data-stu-id="27cad-254">String</span></span>|<span data-ttu-id="27cad-255">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-255">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="27cad-256">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="27cad-256">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="27cad-257">String</span><span class="sxs-lookup"><span data-stu-id="27cad-257">String</span></span>|<span data-ttu-id="27cad-258">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="27cad-258">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="27cad-259">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="27cad-259">isEncrypted</span></span>|<span data-ttu-id="27cad-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-260">Boolean</span></span>|<span data-ttu-id="27cad-261">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-261">Device encryption status</span></span>|
|<span data-ttu-id="27cad-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27cad-262">userPrincipalName</span></span>|<span data-ttu-id="27cad-263">String</span><span class="sxs-lookup"><span data-stu-id="27cad-263">String</span></span>|<span data-ttu-id="27cad-264">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-264">Device user principal name</span></span>|
|<span data-ttu-id="27cad-265">modelo</span><span class="sxs-lookup"><span data-stu-id="27cad-265">model</span></span>|<span data-ttu-id="27cad-266">String</span><span class="sxs-lookup"><span data-stu-id="27cad-266">String</span></span>|<span data-ttu-id="27cad-267">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-267">Model of the device</span></span>|
|<span data-ttu-id="27cad-268">fabricante</span><span class="sxs-lookup"><span data-stu-id="27cad-268">manufacturer</span></span>|<span data-ttu-id="27cad-269">String</span><span class="sxs-lookup"><span data-stu-id="27cad-269">String</span></span>|<span data-ttu-id="27cad-270">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-270">Manufacturer of the device</span></span>|
|<span data-ttu-id="27cad-271">imei</span><span class="sxs-lookup"><span data-stu-id="27cad-271">imei</span></span>|<span data-ttu-id="27cad-272">String</span><span class="sxs-lookup"><span data-stu-id="27cad-272">String</span></span>|<span data-ttu-id="27cad-273">IMEI</span><span class="sxs-lookup"><span data-stu-id="27cad-273">IMEI</span></span>|
|<span data-ttu-id="27cad-274">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="27cad-274">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="27cad-275">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-275">DateTimeOffset</span></span>|<span data-ttu-id="27cad-276">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="27cad-276">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="27cad-277">serialNumber</span><span class="sxs-lookup"><span data-stu-id="27cad-277">serialNumber</span></span>|<span data-ttu-id="27cad-278">String</span><span class="sxs-lookup"><span data-stu-id="27cad-278">String</span></span>|<span data-ttu-id="27cad-279">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="27cad-279">SerialNumber</span></span>|
|<span data-ttu-id="27cad-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="27cad-280">phoneNumber</span></span>|<span data-ttu-id="27cad-281">String</span><span class="sxs-lookup"><span data-stu-id="27cad-281">String</span></span>|<span data-ttu-id="27cad-282">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-282">Phone number of the device</span></span>|
|<span data-ttu-id="27cad-283">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="27cad-283">androidSecurityPatchLevel</span></span>|<span data-ttu-id="27cad-284">String</span><span class="sxs-lookup"><span data-stu-id="27cad-284">String</span></span>|<span data-ttu-id="27cad-285">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="27cad-285">Android security patch level</span></span>|
|<span data-ttu-id="27cad-286">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="27cad-286">userDisplayName</span></span>|<span data-ttu-id="27cad-287">String</span><span class="sxs-lookup"><span data-stu-id="27cad-287">String</span></span>|<span data-ttu-id="27cad-288">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="27cad-288">User display name</span></span>|
|<span data-ttu-id="27cad-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="27cad-289">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="27cad-290">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="27cad-290">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="27cad-291">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="27cad-291">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="27cad-292">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="27cad-292">wiFiMacAddress</span></span>|<span data-ttu-id="27cad-293">String</span><span class="sxs-lookup"><span data-stu-id="27cad-293">String</span></span>|<span data-ttu-id="27cad-294">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="27cad-294">Wi-Fi MAC</span></span>|
|<span data-ttu-id="27cad-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="27cad-295">deviceHealthAttestationState</span></span>|[<span data-ttu-id="27cad-296">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="27cad-296">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="27cad-297">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-297">The device health attestation state.</span></span>|
|<span data-ttu-id="27cad-298">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="27cad-298">subscriberCarrier</span></span>|<span data-ttu-id="27cad-299">String</span><span class="sxs-lookup"><span data-stu-id="27cad-299">String</span></span>|<span data-ttu-id="27cad-300">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="27cad-300">Subscriber Carrier</span></span>|
|<span data-ttu-id="27cad-301">meid</span><span class="sxs-lookup"><span data-stu-id="27cad-301">meid</span></span>|<span data-ttu-id="27cad-302">String</span><span class="sxs-lookup"><span data-stu-id="27cad-302">String</span></span>|<span data-ttu-id="27cad-303">MEID</span><span class="sxs-lookup"><span data-stu-id="27cad-303">MEID</span></span>|
|<span data-ttu-id="27cad-304">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="27cad-304">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="27cad-305">Int64</span><span class="sxs-lookup"><span data-stu-id="27cad-305">Int64</span></span>|<span data-ttu-id="27cad-306">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="27cad-306">Total Storage in Bytes</span></span>|
|<span data-ttu-id="27cad-307">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="27cad-307">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="27cad-308">Int64</span><span class="sxs-lookup"><span data-stu-id="27cad-308">Int64</span></span>|<span data-ttu-id="27cad-309">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="27cad-309">Free Storage in Bytes</span></span>|
|<span data-ttu-id="27cad-310">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="27cad-310">managedDeviceName</span></span>|<span data-ttu-id="27cad-311">String</span><span class="sxs-lookup"><span data-stu-id="27cad-311">String</span></span>|<span data-ttu-id="27cad-312">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-312">Automatically generated name to identify a device.</span></span> <span data-ttu-id="27cad-313">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="27cad-313">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="27cad-314">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="27cad-314">partnerReportedThreatState</span></span>|[<span data-ttu-id="27cad-315">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="27cad-315">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="27cad-316">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-316">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="27cad-317">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27cad-317">Read Only.</span></span> <span data-ttu-id="27cad-318">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="27cad-318">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="27cad-319">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="27cad-319">usersLoggedOn</span></span>|<span data-ttu-id="27cad-320">coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)</span><span class="sxs-lookup"><span data-stu-id="27cad-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="27cad-321">Indica o último logon usuários de um dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-321">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="27cad-322">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="27cad-322">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="27cad-323">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-323">DateTimeOffset</span></span>|<span data-ttu-id="27cad-324">Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.</span><span class="sxs-lookup"><span data-stu-id="27cad-324">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="27cad-325">Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito.</span><span class="sxs-lookup"><span data-stu-id="27cad-325">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="27cad-326">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27cad-326">Read Only.</span></span>|
|<span data-ttu-id="27cad-327">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="27cad-327">autopilotEnrolled</span></span>|<span data-ttu-id="27cad-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-328">Boolean</span></span>|<span data-ttu-id="27cad-329">Relata se o dispositivo gerenciado está inscrito via piloto automático.</span><span class="sxs-lookup"><span data-stu-id="27cad-329">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="27cad-330">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="27cad-330">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="27cad-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cad-331">Boolean</span></span>|<span data-ttu-id="27cad-332">Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário.</span><span class="sxs-lookup"><span data-stu-id="27cad-332">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="27cad-333">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="27cad-333">managementCertificateExpirationDate</span></span>|<span data-ttu-id="27cad-334">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cad-334">DateTimeOffset</span></span>|<span data-ttu-id="27cad-335">Relata a data de validade do certificado de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="27cad-335">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="27cad-336">iccid</span><span class="sxs-lookup"><span data-stu-id="27cad-336">iccid</span></span>|<span data-ttu-id="27cad-337">String</span><span class="sxs-lookup"><span data-stu-id="27cad-337">String</span></span>|<span data-ttu-id="27cad-338">Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM.</span><span class="sxs-lookup"><span data-stu-id="27cad-338">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="27cad-339">UDID</span><span class="sxs-lookup"><span data-stu-id="27cad-339">udid</span></span>|<span data-ttu-id="27cad-340">String</span><span class="sxs-lookup"><span data-stu-id="27cad-340">String</span></span>|<span data-ttu-id="27cad-341">Identificador exclusivo do dispositivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="27cad-341">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="27cad-342">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27cad-342">roleScopeTagIds</span></span>|<span data-ttu-id="27cad-343">String collection</span><span class="sxs-lookup"><span data-stu-id="27cad-343">String collection</span></span>|<span data-ttu-id="27cad-344">Lista de IDs de marca de escopo para essa instância do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27cad-344">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="27cad-345">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="27cad-345">windowsActiveMalwareCount</span></span>|<span data-ttu-id="27cad-346">Int32</span><span class="sxs-lookup"><span data-stu-id="27cad-346">Int32</span></span>|<span data-ttu-id="27cad-347">Contagem de malware ativos para este dispositivo do windows</span><span class="sxs-lookup"><span data-stu-id="27cad-347">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="27cad-348">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="27cad-348">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="27cad-349">Int32</span><span class="sxs-lookup"><span data-stu-id="27cad-349">Int32</span></span>|<span data-ttu-id="27cad-350">Contagem de malware remediados por teste para este dispositivo do windows</span><span class="sxs-lookup"><span data-stu-id="27cad-350">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="27cad-351">Observações</span><span class="sxs-lookup"><span data-stu-id="27cad-351">notes</span></span>|<span data-ttu-id="27cad-352">String</span><span class="sxs-lookup"><span data-stu-id="27cad-352">String</span></span>|<span data-ttu-id="27cad-353">Anotações no dispositivo criado pelo administrador de TI</span><span class="sxs-lookup"><span data-stu-id="27cad-353">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="27cad-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="27cad-354">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="27cad-355">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="27cad-355">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="27cad-356">Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados por agente MDM/ConfigMgr</span><span class="sxs-lookup"><span data-stu-id="27cad-356">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="27cad-357">Resposta</span><span class="sxs-lookup"><span data-stu-id="27cad-357">Response</span></span>
<span data-ttu-id="27cad-358">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27cad-358">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27cad-359">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27cad-359">Example</span></span>

### <a name="request"></a><span data-ttu-id="27cad-360">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27cad-360">Request</span></span>
<span data-ttu-id="27cad-361">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27cad-361">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7166

{
  "@odata.type": "#microsoft.graph.managedDevice",
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

### <a name="response"></a><span data-ttu-id="27cad-362">Resposta</span><span class="sxs-lookup"><span data-stu-id="27cad-362">Response</span></span>
<span data-ttu-id="27cad-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27cad-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7215

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
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




