---
title: Criar managedDevice
description: Criar um novo objeto managedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 320b2fd8878d5ecd0af34152761bda1af6a5985c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584689"
---
# <a name="create-manageddevice"></a><span data-ttu-id="12fc5-103">Criar managedDevice</span><span class="sxs-lookup"><span data-stu-id="12fc5-103">Create managedDevice</span></span>

> <span data-ttu-id="12fc5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12fc5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12fc5-105">Criar um novo objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="12fc5-105">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12fc5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12fc5-106">Prerequisites</span></span>
<span data-ttu-id="12fc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fc5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12fc5-109">Permission type</span></span>|<span data-ttu-id="12fc5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12fc5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fc5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12fc5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12fc5-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fc5-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12fc5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12fc5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fc5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fc5-114">Not supported.</span></span>|
|<span data-ttu-id="12fc5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12fc5-115">Application</span></span>|<span data-ttu-id="12fc5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fc5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fc5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12fc5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="12fc5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12fc5-118">Request headers</span></span>
|<span data-ttu-id="12fc5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12fc5-119">Header</span></span>|<span data-ttu-id="12fc5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="12fc5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12fc5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="12fc5-121">Authorization</span></span>|<span data-ttu-id="12fc5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12fc5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12fc5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12fc5-123">Accept</span></span>|<span data-ttu-id="12fc5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12fc5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fc5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12fc5-125">Request body</span></span>
<span data-ttu-id="12fc5-126">No corpo da solicitação, forneça uma representação JSON do objeto managedDevice.</span><span class="sxs-lookup"><span data-stu-id="12fc5-126">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="12fc5-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDevice.</span><span class="sxs-lookup"><span data-stu-id="12fc5-127">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="12fc5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12fc5-128">Property</span></span>|<span data-ttu-id="12fc5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="12fc5-129">Type</span></span>|<span data-ttu-id="12fc5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="12fc5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12fc5-131">id</span><span class="sxs-lookup"><span data-stu-id="12fc5-131">id</span></span>|<span data-ttu-id="12fc5-132">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-132">String</span></span>|<span data-ttu-id="12fc5-133">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="12fc5-134">userId</span><span class="sxs-lookup"><span data-stu-id="12fc5-134">userId</span></span>|<span data-ttu-id="12fc5-135">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-135">String</span></span>|<span data-ttu-id="12fc5-136">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="12fc5-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="12fc5-137">deviceName</span></span>|<span data-ttu-id="12fc5-138">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-138">String</span></span>|<span data-ttu-id="12fc5-139">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-139">Name of the device</span></span>|
|<span data-ttu-id="12fc5-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="12fc5-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="12fc5-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="12fc5-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="12fc5-142">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-142">Ownership of the device.</span></span> <span data-ttu-id="12fc5-143">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="12fc5-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="12fc5-144">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="12fc5-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="12fc5-145">deviceActionResults</span></span>|<span data-ttu-id="12fc5-146">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="12fc5-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="12fc5-147">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="12fc5-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="12fc5-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="12fc5-148">enrolledDateTime</span></span>|<span data-ttu-id="12fc5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fc5-149">DateTimeOffset</span></span>|<span data-ttu-id="12fc5-150">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="12fc5-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="12fc5-151">lastSyncDateTime</span></span>|<span data-ttu-id="12fc5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fc5-152">DateTimeOffset</span></span>|<span data-ttu-id="12fc5-153">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="12fc5-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="12fc5-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="12fc5-154">operatingSystem</span></span>|<span data-ttu-id="12fc5-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12fc5-155">String</span></span>|<span data-ttu-id="12fc5-156">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-156">Operating system of the device.</span></span> <span data-ttu-id="12fc5-157">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="12fc5-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="12fc5-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="12fc5-158">complianceState</span></span>|[<span data-ttu-id="12fc5-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="12fc5-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="12fc5-160">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-160">Compliance state of the device.</span></span> <span data-ttu-id="12fc5-161">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="12fc5-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="12fc5-162">jailBroken</span></span>|<span data-ttu-id="12fc5-163">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-163">String</span></span>|<span data-ttu-id="12fc5-164">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="12fc5-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="12fc5-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="12fc5-165">managementAgent</span></span>|[<span data-ttu-id="12fc5-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="12fc5-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="12fc5-167">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-167">Management channel of the device.</span></span> <span data-ttu-id="12fc5-168">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="12fc5-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="12fc5-169">osVersion</span></span>|<span data-ttu-id="12fc5-170">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-170">String</span></span>|<span data-ttu-id="12fc5-171">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="12fc5-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="12fc5-172">easActivated</span></span>|<span data-ttu-id="12fc5-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="12fc5-173">Boolean</span></span>|<span data-ttu-id="12fc5-174">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="12fc5-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="12fc5-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="12fc5-175">easDeviceId</span></span>|<span data-ttu-id="12fc5-176">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-176">String</span></span>|<span data-ttu-id="12fc5-177">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="12fc5-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="12fc5-178">easActivationDateTime</span></span>|<span data-ttu-id="12fc5-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fc5-179">DateTimeOffset</span></span>|<span data-ttu-id="12fc5-180">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="12fc5-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="12fc5-181">azureADRegistered</span></span>|<span data-ttu-id="12fc5-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="12fc5-182">Boolean</span></span>|<span data-ttu-id="12fc5-183">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12fc5-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="12fc5-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="12fc5-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="12fc5-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="12fc5-185">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="12fc5-186">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-186">Enrollment type of the device.</span></span> <span data-ttu-id="12fc5-187">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="12fc5-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="12fc5-188">activationLockBypassCode</span></span>|<span data-ttu-id="12fc5-189">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-189">String</span></span>|<span data-ttu-id="12fc5-190">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="12fc5-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="12fc5-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="12fc5-191">emailAddress</span></span>|<span data-ttu-id="12fc5-192">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-192">String</span></span>|<span data-ttu-id="12fc5-193">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="12fc5-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="12fc5-194">azureADDeviceId</span></span>|<span data-ttu-id="12fc5-195">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-195">String</span></span>|<span data-ttu-id="12fc5-196">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12fc5-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="12fc5-197">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12fc5-197">Read only.</span></span>|
|<span data-ttu-id="12fc5-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="12fc5-198">deviceRegistrationState</span></span>|[<span data-ttu-id="12fc5-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="12fc5-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="12fc5-200">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-200">Device registration state.</span></span> <span data-ttu-id="12fc5-201">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="12fc5-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="12fc5-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="12fc5-203">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-203">String</span></span>|<span data-ttu-id="12fc5-204">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-204">Device category display name</span></span>|
|<span data-ttu-id="12fc5-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="12fc5-205">isSupervised</span></span>|<span data-ttu-id="12fc5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="12fc5-206">Boolean</span></span>|<span data-ttu-id="12fc5-207">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-207">Device supervised status</span></span>|
|<span data-ttu-id="12fc5-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="12fc5-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="12fc5-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fc5-209">DateTimeOffset</span></span>|<span data-ttu-id="12fc5-210">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="12fc5-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="12fc5-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="12fc5-211">exchangeAccessState</span></span>|[<span data-ttu-id="12fc5-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="12fc5-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="12fc5-213">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="12fc5-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="12fc5-214">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="12fc5-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="12fc5-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="12fc5-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="12fc5-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="12fc5-217">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="12fc5-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="12fc5-218">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="12fc5-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="12fc5-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="12fc5-220">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-220">String</span></span>|<span data-ttu-id="12fc5-221">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="12fc5-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="12fc5-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="12fc5-223">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-223">String</span></span>|<span data-ttu-id="12fc5-224">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="12fc5-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="12fc5-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="12fc5-225">isEncrypted</span></span>|<span data-ttu-id="12fc5-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="12fc5-226">Boolean</span></span>|<span data-ttu-id="12fc5-227">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-227">Device encryption status</span></span>|
|<span data-ttu-id="12fc5-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12fc5-228">userPrincipalName</span></span>|<span data-ttu-id="12fc5-229">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-229">String</span></span>|<span data-ttu-id="12fc5-230">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-230">Device user principal name</span></span>|
|<span data-ttu-id="12fc5-231">modelo</span><span class="sxs-lookup"><span data-stu-id="12fc5-231">model</span></span>|<span data-ttu-id="12fc5-232">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-232">String</span></span>|<span data-ttu-id="12fc5-233">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-233">Model of the device</span></span>|
|<span data-ttu-id="12fc5-234">fabricante</span><span class="sxs-lookup"><span data-stu-id="12fc5-234">manufacturer</span></span>|<span data-ttu-id="12fc5-235">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-235">String</span></span>|<span data-ttu-id="12fc5-236">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="12fc5-237">imei</span><span class="sxs-lookup"><span data-stu-id="12fc5-237">imei</span></span>|<span data-ttu-id="12fc5-238">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-238">String</span></span>|<span data-ttu-id="12fc5-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="12fc5-239">IMEI</span></span>|
|<span data-ttu-id="12fc5-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="12fc5-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="12fc5-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12fc5-241">DateTimeOffset</span></span>|<span data-ttu-id="12fc5-242">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="12fc5-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="12fc5-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="12fc5-243">serialNumber</span></span>|<span data-ttu-id="12fc5-244">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12fc5-244">String</span></span>|<span data-ttu-id="12fc5-245">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="12fc5-245">SerialNumber</span></span>|
|<span data-ttu-id="12fc5-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="12fc5-246">phoneNumber</span></span>|<span data-ttu-id="12fc5-247">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-247">String</span></span>|<span data-ttu-id="12fc5-248">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12fc5-248">Phone number of the device</span></span>|
|<span data-ttu-id="12fc5-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="12fc5-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="12fc5-250">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-250">String</span></span>|<span data-ttu-id="12fc5-251">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="12fc5-251">Android security patch level</span></span>|
|<span data-ttu-id="12fc5-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="12fc5-252">userDisplayName</span></span>|<span data-ttu-id="12fc5-253">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-253">String</span></span>|<span data-ttu-id="12fc5-254">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="12fc5-254">User display name</span></span>|
|<span data-ttu-id="12fc5-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="12fc5-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="12fc5-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="12fc5-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="12fc5-257">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="12fc5-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="12fc5-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="12fc5-258">wiFiMacAddress</span></span>|<span data-ttu-id="12fc5-259">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-259">String</span></span>|<span data-ttu-id="12fc5-260">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="12fc5-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="12fc5-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="12fc5-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="12fc5-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="12fc5-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="12fc5-263">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-263">The device health attestation state.</span></span>|
|<span data-ttu-id="12fc5-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="12fc5-264">subscriberCarrier</span></span>|<span data-ttu-id="12fc5-265">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-265">String</span></span>|<span data-ttu-id="12fc5-266">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="12fc5-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="12fc5-267">meid</span><span class="sxs-lookup"><span data-stu-id="12fc5-267">meid</span></span>|<span data-ttu-id="12fc5-268">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-268">String</span></span>|<span data-ttu-id="12fc5-269">MEID</span><span class="sxs-lookup"><span data-stu-id="12fc5-269">MEID</span></span>|
|<span data-ttu-id="12fc5-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="12fc5-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="12fc5-271">Int64</span><span class="sxs-lookup"><span data-stu-id="12fc5-271">Int64</span></span>|<span data-ttu-id="12fc5-272">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="12fc5-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="12fc5-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="12fc5-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="12fc5-274">Int64</span><span class="sxs-lookup"><span data-stu-id="12fc5-274">Int64</span></span>|<span data-ttu-id="12fc5-275">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="12fc5-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="12fc5-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="12fc5-276">managedDeviceName</span></span>|<span data-ttu-id="12fc5-277">String</span><span class="sxs-lookup"><span data-stu-id="12fc5-277">String</span></span>|<span data-ttu-id="12fc5-278">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="12fc5-279">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="12fc5-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="12fc5-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="12fc5-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="12fc5-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="12fc5-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="12fc5-282">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="12fc5-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="12fc5-283">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12fc5-283">Read Only.</span></span> <span data-ttu-id="12fc5-284">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="12fc5-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="12fc5-285">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fc5-285">Response</span></span>
<span data-ttu-id="12fc5-286">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedDevice](../resources/intune-devices-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12fc5-286">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fc5-287">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12fc5-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="12fc5-288">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12fc5-288">Request</span></span>
<span data-ttu-id="12fc5-289">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12fc5-289">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
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

### <a name="response"></a><span data-ttu-id="12fc5-290">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fc5-290">Response</span></span>
<span data-ttu-id="12fc5-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12fc5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



