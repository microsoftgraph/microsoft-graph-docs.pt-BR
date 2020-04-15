---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55e63802783035e7a418ea6dd3041240685c228c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474482"
---
# <a name="update-manageddevice"></a><span data-ttu-id="d0f36-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="d0f36-103">Update managedDevice</span></span>

<span data-ttu-id="d0f36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0f36-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0f36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f36-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0f36-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0f36-107">Prerequisites</span></span>
<span data-ttu-id="d0f36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0f36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0f36-110">Permission type</span></span>|<span data-ttu-id="d0f36-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0f36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0f36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0f36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0f36-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f36-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0f36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0f36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0f36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f36-115">Not supported.</span></span>|
|<span data-ttu-id="d0f36-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0f36-116">Application</span></span>|<span data-ttu-id="d0f36-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0f36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0f36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="d0f36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f36-119">Request headers</span></span>
|<span data-ttu-id="d0f36-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0f36-120">Header</span></span>|<span data-ttu-id="d0f36-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d0f36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0f36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0f36-122">Authorization</span></span>|<span data-ttu-id="d0f36-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0f36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0f36-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0f36-124">Accept</span></span>|<span data-ttu-id="d0f36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0f36-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f36-126">Request body</span></span>
<span data-ttu-id="d0f36-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="d0f36-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="d0f36-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0f36-129">Property</span></span>|<span data-ttu-id="d0f36-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0f36-130">Type</span></span>|<span data-ttu-id="d0f36-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0f36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f36-132">id</span><span class="sxs-lookup"><span data-stu-id="d0f36-132">id</span></span>|<span data-ttu-id="d0f36-133">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-133">String</span></span>|<span data-ttu-id="d0f36-134">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="d0f36-135">userId</span><span class="sxs-lookup"><span data-stu-id="d0f36-135">userId</span></span>|<span data-ttu-id="d0f36-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0f36-136">String</span></span>|<span data-ttu-id="d0f36-137">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="d0f36-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="d0f36-138">deviceName</span></span>|<span data-ttu-id="d0f36-139">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-139">String</span></span>|<span data-ttu-id="d0f36-140">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-140">Name of the device</span></span>|
|<span data-ttu-id="d0f36-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d0f36-141">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d0f36-142">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d0f36-142">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="d0f36-143">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-143">Ownership of the device.</span></span> <span data-ttu-id="d0f36-144">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="d0f36-144">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="d0f36-145">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-145">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d0f36-146">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d0f36-146">deviceActionResults</span></span>|<span data-ttu-id="d0f36-147">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0f36-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d0f36-148">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="d0f36-148">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="d0f36-149">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-149">enrolledDateTime</span></span>|<span data-ttu-id="d0f36-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-150">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-151">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-151">Enrollment time of the device.</span></span>|
|<span data-ttu-id="d0f36-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-152">lastSyncDateTime</span></span>|<span data-ttu-id="d0f36-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-153">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-154">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="d0f36-154">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="d0f36-155">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d0f36-155">operatingSystem</span></span>|<span data-ttu-id="d0f36-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0f36-156">String</span></span>|<span data-ttu-id="d0f36-157">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-157">Operating system of the device.</span></span> <span data-ttu-id="d0f36-158">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="d0f36-158">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="d0f36-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="d0f36-159">complianceState</span></span>|[<span data-ttu-id="d0f36-160">complianceState</span><span class="sxs-lookup"><span data-stu-id="d0f36-160">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d0f36-161">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-161">Compliance state of the device.</span></span> <span data-ttu-id="d0f36-162">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-162">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d0f36-163">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d0f36-163">jailBroken</span></span>|<span data-ttu-id="d0f36-164">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-164">String</span></span>|<span data-ttu-id="d0f36-165">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="d0f36-165">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="d0f36-166">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d0f36-166">managementAgent</span></span>|[<span data-ttu-id="d0f36-167">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d0f36-167">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="d0f36-168">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-168">Management channel of the device.</span></span> <span data-ttu-id="d0f36-169">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-169">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="d0f36-170">osVersion</span><span class="sxs-lookup"><span data-stu-id="d0f36-170">osVersion</span></span>|<span data-ttu-id="d0f36-171">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-171">String</span></span>|<span data-ttu-id="d0f36-172">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-172">Operating system version of the device.</span></span>|
|<span data-ttu-id="d0f36-173">easActivated</span><span class="sxs-lookup"><span data-stu-id="d0f36-173">easActivated</span></span>|<span data-ttu-id="d0f36-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0f36-174">Boolean</span></span>|<span data-ttu-id="d0f36-175">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d0f36-175">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="d0f36-176">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0f36-176">easDeviceId</span></span>|<span data-ttu-id="d0f36-177">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-177">String</span></span>|<span data-ttu-id="d0f36-178">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-178">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="d0f36-179">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-179">easActivationDateTime</span></span>|<span data-ttu-id="d0f36-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-180">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-181">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-181">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="d0f36-182">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d0f36-182">azureADRegistered</span></span>|<span data-ttu-id="d0f36-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0f36-183">Boolean</span></span>|<span data-ttu-id="d0f36-184">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0f36-184">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="d0f36-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d0f36-185">deviceEnrollmentType</span></span>|[<span data-ttu-id="d0f36-186">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d0f36-186">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d0f36-187">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-187">Enrollment type of the device.</span></span> <span data-ttu-id="d0f36-188">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-188">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d0f36-189">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d0f36-189">activationLockBypassCode</span></span>|<span data-ttu-id="d0f36-190">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-190">String</span></span>|<span data-ttu-id="d0f36-191">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="d0f36-191">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="d0f36-192">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d0f36-192">emailAddress</span></span>|<span data-ttu-id="d0f36-193">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-193">String</span></span>|<span data-ttu-id="d0f36-194">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-194">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="d0f36-195">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0f36-195">azureADDeviceId</span></span>|<span data-ttu-id="d0f36-196">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-196">String</span></span>|<span data-ttu-id="d0f36-197">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0f36-197">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d0f36-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0f36-198">Read only.</span></span>|
|<span data-ttu-id="d0f36-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d0f36-199">deviceRegistrationState</span></span>|[<span data-ttu-id="d0f36-200">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d0f36-200">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d0f36-201">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-201">Device registration state.</span></span> <span data-ttu-id="d0f36-202">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-202">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d0f36-203">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0f36-203">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d0f36-204">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-204">String</span></span>|<span data-ttu-id="d0f36-205">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-205">Device category display name</span></span>|
|<span data-ttu-id="d0f36-206">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d0f36-206">isSupervised</span></span>|<span data-ttu-id="d0f36-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0f36-207">Boolean</span></span>|<span data-ttu-id="d0f36-208">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-208">Device supervised status</span></span>|
|<span data-ttu-id="d0f36-209">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-209">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d0f36-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-210">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-211">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0f36-211">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="d0f36-212">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d0f36-212">exchangeAccessState</span></span>|[<span data-ttu-id="d0f36-213">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d0f36-213">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d0f36-214">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0f36-214">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d0f36-215">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-215">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d0f36-216">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d0f36-216">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d0f36-217">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d0f36-217">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d0f36-218">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0f36-218">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d0f36-219">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-219">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d0f36-220">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d0f36-220">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d0f36-221">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-221">String</span></span>|<span data-ttu-id="d0f36-222">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-222">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="d0f36-223">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d0f36-223">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d0f36-224">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-224">String</span></span>|<span data-ttu-id="d0f36-225">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="d0f36-225">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="d0f36-226">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d0f36-226">isEncrypted</span></span>|<span data-ttu-id="d0f36-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0f36-227">Boolean</span></span>|<span data-ttu-id="d0f36-228">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-228">Device encryption status</span></span>|
|<span data-ttu-id="d0f36-229">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0f36-229">userPrincipalName</span></span>|<span data-ttu-id="d0f36-230">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-230">String</span></span>|<span data-ttu-id="d0f36-231">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-231">Device user principal name</span></span>|
|<span data-ttu-id="d0f36-232">modelo</span><span class="sxs-lookup"><span data-stu-id="d0f36-232">model</span></span>|<span data-ttu-id="d0f36-233">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-233">String</span></span>|<span data-ttu-id="d0f36-234">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-234">Model of the device</span></span>|
|<span data-ttu-id="d0f36-235">fabricante</span><span class="sxs-lookup"><span data-stu-id="d0f36-235">manufacturer</span></span>|<span data-ttu-id="d0f36-236">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-236">String</span></span>|<span data-ttu-id="d0f36-237">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-237">Manufacturer of the device</span></span>|
|<span data-ttu-id="d0f36-238">imei</span><span class="sxs-lookup"><span data-stu-id="d0f36-238">imei</span></span>|<span data-ttu-id="d0f36-239">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-239">String</span></span>|<span data-ttu-id="d0f36-240">IMEI</span><span class="sxs-lookup"><span data-stu-id="d0f36-240">IMEI</span></span>|
|<span data-ttu-id="d0f36-241">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-241">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d0f36-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-242">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-243">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="d0f36-243">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d0f36-244">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d0f36-244">serialNumber</span></span>|<span data-ttu-id="d0f36-245">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0f36-245">String</span></span>|<span data-ttu-id="d0f36-246">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="d0f36-246">SerialNumber</span></span>|
|<span data-ttu-id="d0f36-247">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d0f36-247">phoneNumber</span></span>|<span data-ttu-id="d0f36-248">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-248">String</span></span>|<span data-ttu-id="d0f36-249">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0f36-249">Phone number of the device</span></span>|
|<span data-ttu-id="d0f36-250">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d0f36-250">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d0f36-251">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-251">String</span></span>|<span data-ttu-id="d0f36-252">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="d0f36-252">Android security patch level</span></span>|
|<span data-ttu-id="d0f36-253">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0f36-253">userDisplayName</span></span>|<span data-ttu-id="d0f36-254">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-254">String</span></span>|<span data-ttu-id="d0f36-255">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="d0f36-255">User display name</span></span>|
|<span data-ttu-id="d0f36-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d0f36-256">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d0f36-257">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d0f36-257">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d0f36-258">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="d0f36-258">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="d0f36-259">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d0f36-259">wiFiMacAddress</span></span>|<span data-ttu-id="d0f36-260">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-260">String</span></span>|<span data-ttu-id="d0f36-261">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="d0f36-261">Wi-Fi MAC</span></span>|
|<span data-ttu-id="d0f36-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d0f36-262">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d0f36-263">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d0f36-263">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d0f36-264">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-264">The device health attestation state.</span></span>|
|<span data-ttu-id="d0f36-265">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d0f36-265">subscriberCarrier</span></span>|<span data-ttu-id="d0f36-266">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-266">String</span></span>|<span data-ttu-id="d0f36-267">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="d0f36-267">Subscriber Carrier</span></span>|
|<span data-ttu-id="d0f36-268">meid</span><span class="sxs-lookup"><span data-stu-id="d0f36-268">meid</span></span>|<span data-ttu-id="d0f36-269">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-269">String</span></span>|<span data-ttu-id="d0f36-270">MEID</span><span class="sxs-lookup"><span data-stu-id="d0f36-270">MEID</span></span>|
|<span data-ttu-id="d0f36-271">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d0f36-271">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d0f36-272">Int64</span><span class="sxs-lookup"><span data-stu-id="d0f36-272">Int64</span></span>|<span data-ttu-id="d0f36-273">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="d0f36-273">Total Storage in Bytes</span></span>|
|<span data-ttu-id="d0f36-274">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d0f36-274">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d0f36-275">Int64</span><span class="sxs-lookup"><span data-stu-id="d0f36-275">Int64</span></span>|<span data-ttu-id="d0f36-276">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="d0f36-276">Free Storage in Bytes</span></span>|
|<span data-ttu-id="d0f36-277">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d0f36-277">managedDeviceName</span></span>|<span data-ttu-id="d0f36-278">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-278">String</span></span>|<span data-ttu-id="d0f36-279">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-279">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d0f36-280">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d0f36-280">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="d0f36-281">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d0f36-281">partnerReportedThreatState</span></span>|[<span data-ttu-id="d0f36-282">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="d0f36-282">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d0f36-283">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0f36-283">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d0f36-284">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0f36-284">Read Only.</span></span> <span data-ttu-id="d0f36-285">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="d0f36-285">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0f36-286">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f36-286">Response</span></span>
<span data-ttu-id="d0f36-287">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0f36-287">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f36-288">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0f36-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0f36-289">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f36-289">Request</span></span>
<span data-ttu-id="d0f36-290">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0f36-290">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4656

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
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
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="d0f36-291">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f36-291">Response</span></span>
<span data-ttu-id="d0f36-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0f36-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
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
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
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
  "partnerReportedThreatState": "activated"
}
```






