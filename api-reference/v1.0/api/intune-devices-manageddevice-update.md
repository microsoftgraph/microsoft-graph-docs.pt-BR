---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07e25aa9390bfdd11801b499f516ba9e7e6dbd27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513473"
---
# <a name="update-manageddevice"></a><span data-ttu-id="ee71d-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="ee71d-103">Update managedDevice</span></span>

<span data-ttu-id="ee71d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee71d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee71d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee71d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee71d-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ee71d-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee71d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee71d-107">Prerequisites</span></span>
<span data-ttu-id="ee71d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee71d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee71d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee71d-110">Permission type</span></span>|<span data-ttu-id="ee71d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee71d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee71d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee71d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee71d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee71d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee71d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee71d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee71d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee71d-115">Not supported.</span></span>|
|<span data-ttu-id="ee71d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee71d-116">Application</span></span>|<span data-ttu-id="ee71d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee71d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee71d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee71d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="ee71d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee71d-119">Request headers</span></span>
|<span data-ttu-id="ee71d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee71d-120">Header</span></span>|<span data-ttu-id="ee71d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ee71d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee71d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee71d-122">Authorization</span></span>|<span data-ttu-id="ee71d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee71d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee71d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee71d-124">Accept</span></span>|<span data-ttu-id="ee71d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee71d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee71d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee71d-126">Request body</span></span>
<span data-ttu-id="ee71d-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ee71d-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="ee71d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ee71d-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="ee71d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee71d-129">Property</span></span>|<span data-ttu-id="ee71d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee71d-130">Type</span></span>|<span data-ttu-id="ee71d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee71d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee71d-132">id</span><span class="sxs-lookup"><span data-stu-id="ee71d-132">id</span></span>|<span data-ttu-id="ee71d-133">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-133">String</span></span>|<span data-ttu-id="ee71d-134">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="ee71d-135">userId</span><span class="sxs-lookup"><span data-stu-id="ee71d-135">userId</span></span>|<span data-ttu-id="ee71d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee71d-136">String</span></span>|<span data-ttu-id="ee71d-137">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="ee71d-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="ee71d-138">deviceName</span></span>|<span data-ttu-id="ee71d-139">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-139">String</span></span>|<span data-ttu-id="ee71d-140">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-140">Name of the device</span></span>|
|<span data-ttu-id="ee71d-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ee71d-141">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ee71d-142">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ee71d-142">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="ee71d-143">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-143">Ownership of the device.</span></span> <span data-ttu-id="ee71d-144">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="ee71d-144">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ee71d-145">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-145">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ee71d-146">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ee71d-146">deviceActionResults</span></span>|<span data-ttu-id="ee71d-147">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee71d-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ee71d-148">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="ee71d-148">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="ee71d-149">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ee71d-149">enrolledDateTime</span></span>|<span data-ttu-id="ee71d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee71d-150">DateTimeOffset</span></span>|<span data-ttu-id="ee71d-151">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-151">Enrollment time of the device.</span></span>|
|<span data-ttu-id="ee71d-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ee71d-152">lastSyncDateTime</span></span>|<span data-ttu-id="ee71d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee71d-153">DateTimeOffset</span></span>|<span data-ttu-id="ee71d-154">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="ee71d-154">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="ee71d-155">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ee71d-155">operatingSystem</span></span>|<span data-ttu-id="ee71d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee71d-156">String</span></span>|<span data-ttu-id="ee71d-157">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-157">Operating system of the device.</span></span> <span data-ttu-id="ee71d-158">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="ee71d-158">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="ee71d-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="ee71d-159">complianceState</span></span>|[<span data-ttu-id="ee71d-160">complianceState</span><span class="sxs-lookup"><span data-stu-id="ee71d-160">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ee71d-161">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-161">Compliance state of the device.</span></span> <span data-ttu-id="ee71d-162">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-162">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ee71d-163">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ee71d-163">jailBroken</span></span>|<span data-ttu-id="ee71d-164">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-164">String</span></span>|<span data-ttu-id="ee71d-165">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="ee71d-165">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="ee71d-166">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ee71d-166">managementAgent</span></span>|[<span data-ttu-id="ee71d-167">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ee71d-167">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="ee71d-168">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-168">Management channel of the device.</span></span> <span data-ttu-id="ee71d-169">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-169">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="ee71d-170">osVersion</span><span class="sxs-lookup"><span data-stu-id="ee71d-170">osVersion</span></span>|<span data-ttu-id="ee71d-171">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-171">String</span></span>|<span data-ttu-id="ee71d-172">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-172">Operating system version of the device.</span></span>|
|<span data-ttu-id="ee71d-173">easActivated</span><span class="sxs-lookup"><span data-stu-id="ee71d-173">easActivated</span></span>|<span data-ttu-id="ee71d-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee71d-174">Boolean</span></span>|<span data-ttu-id="ee71d-175">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ee71d-175">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="ee71d-176">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ee71d-176">easDeviceId</span></span>|<span data-ttu-id="ee71d-177">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-177">String</span></span>|<span data-ttu-id="ee71d-178">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-178">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="ee71d-179">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee71d-179">easActivationDateTime</span></span>|<span data-ttu-id="ee71d-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee71d-180">DateTimeOffset</span></span>|<span data-ttu-id="ee71d-181">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-181">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="ee71d-182">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ee71d-182">azureADRegistered</span></span>|<span data-ttu-id="ee71d-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee71d-183">Boolean</span></span>|<span data-ttu-id="ee71d-184">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ee71d-184">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ee71d-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ee71d-185">deviceEnrollmentType</span></span>|[<span data-ttu-id="ee71d-186">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ee71d-186">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="ee71d-187">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-187">Enrollment type of the device.</span></span> <span data-ttu-id="ee71d-188">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-188">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="ee71d-189">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ee71d-189">activationLockBypassCode</span></span>|<span data-ttu-id="ee71d-190">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-190">String</span></span>|<span data-ttu-id="ee71d-191">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="ee71d-191">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="ee71d-192">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ee71d-192">emailAddress</span></span>|<span data-ttu-id="ee71d-193">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-193">String</span></span>|<span data-ttu-id="ee71d-194">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-194">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="ee71d-195">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ee71d-195">azureADDeviceId</span></span>|<span data-ttu-id="ee71d-196">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-196">String</span></span>|<span data-ttu-id="ee71d-197">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ee71d-197">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ee71d-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee71d-198">Read only.</span></span>|
|<span data-ttu-id="ee71d-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ee71d-199">deviceRegistrationState</span></span>|[<span data-ttu-id="ee71d-200">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ee71d-200">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ee71d-201">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-201">Device registration state.</span></span> <span data-ttu-id="ee71d-202">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-202">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ee71d-203">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee71d-203">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ee71d-204">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-204">String</span></span>|<span data-ttu-id="ee71d-205">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-205">Device category display name</span></span>|
|<span data-ttu-id="ee71d-206">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ee71d-206">isSupervised</span></span>|<span data-ttu-id="ee71d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee71d-207">Boolean</span></span>|<span data-ttu-id="ee71d-208">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-208">Device supervised status</span></span>|
|<span data-ttu-id="ee71d-209">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ee71d-209">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ee71d-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee71d-210">DateTimeOffset</span></span>|<span data-ttu-id="ee71d-211">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee71d-211">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="ee71d-212">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ee71d-212">exchangeAccessState</span></span>|[<span data-ttu-id="ee71d-213">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ee71d-213">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ee71d-214">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee71d-214">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ee71d-215">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-215">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ee71d-216">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ee71d-216">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ee71d-217">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ee71d-217">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ee71d-218">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee71d-218">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ee71d-219">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-219">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ee71d-220">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ee71d-220">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ee71d-221">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-221">String</span></span>|<span data-ttu-id="ee71d-222">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-222">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="ee71d-223">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ee71d-223">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ee71d-224">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-224">String</span></span>|<span data-ttu-id="ee71d-225">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="ee71d-225">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="ee71d-226">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ee71d-226">isEncrypted</span></span>|<span data-ttu-id="ee71d-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee71d-227">Boolean</span></span>|<span data-ttu-id="ee71d-228">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-228">Device encryption status</span></span>|
|<span data-ttu-id="ee71d-229">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee71d-229">userPrincipalName</span></span>|<span data-ttu-id="ee71d-230">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-230">String</span></span>|<span data-ttu-id="ee71d-231">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-231">Device user principal name</span></span>|
|<span data-ttu-id="ee71d-232">modelo</span><span class="sxs-lookup"><span data-stu-id="ee71d-232">model</span></span>|<span data-ttu-id="ee71d-233">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-233">String</span></span>|<span data-ttu-id="ee71d-234">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-234">Model of the device</span></span>|
|<span data-ttu-id="ee71d-235">fabricante</span><span class="sxs-lookup"><span data-stu-id="ee71d-235">manufacturer</span></span>|<span data-ttu-id="ee71d-236">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-236">String</span></span>|<span data-ttu-id="ee71d-237">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-237">Manufacturer of the device</span></span>|
|<span data-ttu-id="ee71d-238">imei</span><span class="sxs-lookup"><span data-stu-id="ee71d-238">imei</span></span>|<span data-ttu-id="ee71d-239">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-239">String</span></span>|<span data-ttu-id="ee71d-240">IMEI</span><span class="sxs-lookup"><span data-stu-id="ee71d-240">IMEI</span></span>|
|<span data-ttu-id="ee71d-241">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee71d-241">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ee71d-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee71d-242">DateTimeOffset</span></span>|<span data-ttu-id="ee71d-243">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="ee71d-243">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ee71d-244">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ee71d-244">serialNumber</span></span>|<span data-ttu-id="ee71d-245">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee71d-245">String</span></span>|<span data-ttu-id="ee71d-246">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="ee71d-246">SerialNumber</span></span>|
|<span data-ttu-id="ee71d-247">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ee71d-247">phoneNumber</span></span>|<span data-ttu-id="ee71d-248">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-248">String</span></span>|<span data-ttu-id="ee71d-249">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ee71d-249">Phone number of the device</span></span>|
|<span data-ttu-id="ee71d-250">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ee71d-250">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ee71d-251">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-251">String</span></span>|<span data-ttu-id="ee71d-252">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="ee71d-252">Android security patch level</span></span>|
|<span data-ttu-id="ee71d-253">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee71d-253">userDisplayName</span></span>|<span data-ttu-id="ee71d-254">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-254">String</span></span>|<span data-ttu-id="ee71d-255">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="ee71d-255">User display name</span></span>|
|<span data-ttu-id="ee71d-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ee71d-256">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ee71d-257">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ee71d-257">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ee71d-258">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="ee71d-258">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="ee71d-259">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ee71d-259">wiFiMacAddress</span></span>|<span data-ttu-id="ee71d-260">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-260">String</span></span>|<span data-ttu-id="ee71d-261">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="ee71d-261">Wi-Fi MAC</span></span>|
|<span data-ttu-id="ee71d-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ee71d-262">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ee71d-263">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ee71d-263">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ee71d-264">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-264">The device health attestation state.</span></span>|
|<span data-ttu-id="ee71d-265">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ee71d-265">subscriberCarrier</span></span>|<span data-ttu-id="ee71d-266">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-266">String</span></span>|<span data-ttu-id="ee71d-267">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="ee71d-267">Subscriber Carrier</span></span>|
|<span data-ttu-id="ee71d-268">meid</span><span class="sxs-lookup"><span data-stu-id="ee71d-268">meid</span></span>|<span data-ttu-id="ee71d-269">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-269">String</span></span>|<span data-ttu-id="ee71d-270">MEID</span><span class="sxs-lookup"><span data-stu-id="ee71d-270">MEID</span></span>|
|<span data-ttu-id="ee71d-271">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ee71d-271">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ee71d-272">Int64</span><span class="sxs-lookup"><span data-stu-id="ee71d-272">Int64</span></span>|<span data-ttu-id="ee71d-273">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="ee71d-273">Total Storage in Bytes</span></span>|
|<span data-ttu-id="ee71d-274">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ee71d-274">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ee71d-275">Int64</span><span class="sxs-lookup"><span data-stu-id="ee71d-275">Int64</span></span>|<span data-ttu-id="ee71d-276">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="ee71d-276">Free Storage in Bytes</span></span>|
|<span data-ttu-id="ee71d-277">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ee71d-277">managedDeviceName</span></span>|<span data-ttu-id="ee71d-278">String</span><span class="sxs-lookup"><span data-stu-id="ee71d-278">String</span></span>|<span data-ttu-id="ee71d-279">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-279">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ee71d-280">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ee71d-280">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="ee71d-281">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ee71d-281">partnerReportedThreatState</span></span>|[<span data-ttu-id="ee71d-282">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="ee71d-282">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ee71d-283">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ee71d-283">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ee71d-284">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee71d-284">Read Only.</span></span> <span data-ttu-id="ee71d-285">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="ee71d-285">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="ee71d-286">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee71d-286">Response</span></span>
<span data-ttu-id="ee71d-287">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee71d-287">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee71d-288">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee71d-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee71d-289">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee71d-289">Request</span></span>
<span data-ttu-id="ee71d-290">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee71d-290">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee71d-291">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee71d-291">Response</span></span>
<span data-ttu-id="ee71d-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee71d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




