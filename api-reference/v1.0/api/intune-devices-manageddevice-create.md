---
title: Criar managedDevice
description: Criar um novo objeto managedDevice.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d8c1eb015e4381863bf48679e59307aeb0cc3da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513585"
---
# <a name="create-manageddevice"></a><span data-ttu-id="ec8d4-103">Criar managedDevice</span><span class="sxs-lookup"><span data-stu-id="ec8d4-103">Create managedDevice</span></span>

<span data-ttu-id="ec8d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec8d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec8d4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec8d4-106">Criar um novo objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="ec8d4-106">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec8d4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec8d4-107">Prerequisites</span></span>
<span data-ttu-id="ec8d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec8d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec8d4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec8d4-110">Permission type</span></span>|<span data-ttu-id="ec8d4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec8d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec8d4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec8d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec8d4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec8d4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ec8d4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec8d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec8d4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-115">Not supported.</span></span>|
|<span data-ttu-id="ec8d4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-116">Application</span></span>|<span data-ttu-id="ec8d4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec8d4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec8d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="ec8d4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec8d4-119">Request headers</span></span>
|<span data-ttu-id="ec8d4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec8d4-120">Header</span></span>|<span data-ttu-id="ec8d4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ec8d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec8d4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec8d4-122">Authorization</span></span>|<span data-ttu-id="ec8d4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec8d4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec8d4-124">Accept</span></span>|<span data-ttu-id="ec8d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec8d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec8d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec8d4-126">Request body</span></span>
<span data-ttu-id="ec8d4-127">No corpo da solicitação, forneça uma representação JSON do objeto managedDevice.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-127">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="ec8d4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDevice.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-128">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="ec8d4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec8d4-129">Property</span></span>|<span data-ttu-id="ec8d4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-130">Type</span></span>|<span data-ttu-id="ec8d4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec8d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec8d4-132">id</span><span class="sxs-lookup"><span data-stu-id="ec8d4-132">id</span></span>|<span data-ttu-id="ec8d4-133">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-133">String</span></span>|<span data-ttu-id="ec8d4-134">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="ec8d4-135">userId</span><span class="sxs-lookup"><span data-stu-id="ec8d4-135">userId</span></span>|<span data-ttu-id="ec8d4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec8d4-136">String</span></span>|<span data-ttu-id="ec8d4-137">O identificador exclusivo do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="ec8d4-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="ec8d4-138">deviceName</span></span>|<span data-ttu-id="ec8d4-139">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-139">String</span></span>|<span data-ttu-id="ec8d4-140">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-140">Name of the device</span></span>|
|<span data-ttu-id="ec8d4-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ec8d4-141">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ec8d4-142">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ec8d4-142">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="ec8d4-143">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-143">Ownership of the device.</span></span> <span data-ttu-id="ec8d4-144">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="ec8d4-144">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ec8d4-145">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-145">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ec8d4-146">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ec8d4-146">deviceActionResults</span></span>|<span data-ttu-id="ec8d4-147">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ec8d4-147">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ec8d4-148">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-148">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="ec8d4-149">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8d4-149">enrolledDateTime</span></span>|<span data-ttu-id="ec8d4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8d4-150">DateTimeOffset</span></span>|<span data-ttu-id="ec8d4-151">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-151">Enrollment time of the device.</span></span>|
|<span data-ttu-id="ec8d4-152">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8d4-152">lastSyncDateTime</span></span>|<span data-ttu-id="ec8d4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8d4-153">DateTimeOffset</span></span>|<span data-ttu-id="ec8d4-154">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-154">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="ec8d4-155">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ec8d4-155">operatingSystem</span></span>|<span data-ttu-id="ec8d4-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec8d4-156">String</span></span>|<span data-ttu-id="ec8d4-157">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-157">Operating system of the device.</span></span> <span data-ttu-id="ec8d4-158">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-158">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="ec8d4-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-159">complianceState</span></span>|[<span data-ttu-id="ec8d4-160">complianceState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-160">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ec8d4-161">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-161">Compliance state of the device.</span></span> <span data-ttu-id="ec8d4-162">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-162">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ec8d4-163">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ec8d4-163">jailBroken</span></span>|<span data-ttu-id="ec8d4-164">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-164">String</span></span>|<span data-ttu-id="ec8d4-165">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-165">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="ec8d4-166">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ec8d4-166">managementAgent</span></span>|[<span data-ttu-id="ec8d4-167">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ec8d4-167">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="ec8d4-168">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-168">Management channel of the device.</span></span> <span data-ttu-id="ec8d4-169">Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-169">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="ec8d4-170">osVersion</span><span class="sxs-lookup"><span data-stu-id="ec8d4-170">osVersion</span></span>|<span data-ttu-id="ec8d4-171">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-171">String</span></span>|<span data-ttu-id="ec8d4-172">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-172">Operating system version of the device.</span></span>|
|<span data-ttu-id="ec8d4-173">easActivated</span><span class="sxs-lookup"><span data-stu-id="ec8d4-173">easActivated</span></span>|<span data-ttu-id="ec8d4-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec8d4-174">Boolean</span></span>|<span data-ttu-id="ec8d4-175">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-175">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="ec8d4-176">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ec8d4-176">easDeviceId</span></span>|<span data-ttu-id="ec8d4-177">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-177">String</span></span>|<span data-ttu-id="ec8d4-178">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-178">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="ec8d4-179">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8d4-179">easActivationDateTime</span></span>|<span data-ttu-id="ec8d4-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8d4-180">DateTimeOffset</span></span>|<span data-ttu-id="ec8d4-181">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-181">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="ec8d4-182">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ec8d4-182">azureADRegistered</span></span>|<span data-ttu-id="ec8d4-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec8d4-183">Boolean</span></span>|<span data-ttu-id="ec8d4-184">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-184">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ec8d4-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ec8d4-185">deviceEnrollmentType</span></span>|[<span data-ttu-id="ec8d4-186">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ec8d4-186">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="ec8d4-187">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-187">Enrollment type of the device.</span></span> <span data-ttu-id="ec8d4-188">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-188">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="ec8d4-189">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ec8d4-189">activationLockBypassCode</span></span>|<span data-ttu-id="ec8d4-190">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-190">String</span></span>|<span data-ttu-id="ec8d4-191">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-191">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="ec8d4-192">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ec8d4-192">emailAddress</span></span>|<span data-ttu-id="ec8d4-193">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-193">String</span></span>|<span data-ttu-id="ec8d4-194">Email(s) do usuário associado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-194">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="ec8d4-195">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ec8d4-195">azureADDeviceId</span></span>|<span data-ttu-id="ec8d4-196">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-196">String</span></span>|<span data-ttu-id="ec8d4-197">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-197">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ec8d4-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-198">Read only.</span></span>|
|<span data-ttu-id="ec8d4-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-199">deviceRegistrationState</span></span>|[<span data-ttu-id="ec8d4-200">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-200">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ec8d4-201">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-201">Device registration state.</span></span> <span data-ttu-id="ec8d4-202">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-202">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ec8d4-203">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec8d4-203">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ec8d4-204">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-204">String</span></span>|<span data-ttu-id="ec8d4-205">Nome de exibição da categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-205">Device category display name</span></span>|
|<span data-ttu-id="ec8d4-206">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ec8d4-206">isSupervised</span></span>|<span data-ttu-id="ec8d4-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec8d4-207">Boolean</span></span>|<span data-ttu-id="ec8d4-208">Status supervisionado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-208">Device supervised status</span></span>|
|<span data-ttu-id="ec8d4-209">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8d4-209">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ec8d4-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8d4-210">DateTimeOffset</span></span>|<span data-ttu-id="ec8d4-211">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-211">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="ec8d4-212">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-212">exchangeAccessState</span></span>|[<span data-ttu-id="ec8d4-213">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-213">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ec8d4-214">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-214">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ec8d4-215">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-215">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ec8d4-216">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ec8d4-216">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ec8d4-217">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ec8d4-217">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ec8d4-218">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-218">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ec8d4-219">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-219">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ec8d4-220">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ec8d4-220">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ec8d4-221">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-221">String</span></span>|<span data-ttu-id="ec8d4-222">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-222">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="ec8d4-223">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ec8d4-223">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ec8d4-224">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-224">String</span></span>|<span data-ttu-id="ec8d4-225">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-225">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="ec8d4-226">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ec8d4-226">isEncrypted</span></span>|<span data-ttu-id="ec8d4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec8d4-227">Boolean</span></span>|<span data-ttu-id="ec8d4-228">Status da criptografia de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-228">Device encryption status</span></span>|
|<span data-ttu-id="ec8d4-229">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec8d4-229">userPrincipalName</span></span>|<span data-ttu-id="ec8d4-230">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-230">String</span></span>|<span data-ttu-id="ec8d4-231">Nome principal do usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-231">Device user principal name</span></span>|
|<span data-ttu-id="ec8d4-232">modelo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-232">model</span></span>|<span data-ttu-id="ec8d4-233">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-233">String</span></span>|<span data-ttu-id="ec8d4-234">Modelo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-234">Model of the device</span></span>|
|<span data-ttu-id="ec8d4-235">fabricante</span><span class="sxs-lookup"><span data-stu-id="ec8d4-235">manufacturer</span></span>|<span data-ttu-id="ec8d4-236">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-236">String</span></span>|<span data-ttu-id="ec8d4-237">Fabricante do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-237">Manufacturer of the device</span></span>|
|<span data-ttu-id="ec8d4-238">imei</span><span class="sxs-lookup"><span data-stu-id="ec8d4-238">imei</span></span>|<span data-ttu-id="ec8d4-239">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-239">String</span></span>|<span data-ttu-id="ec8d4-240">IMEI</span><span class="sxs-lookup"><span data-stu-id="ec8d4-240">IMEI</span></span>|
|<span data-ttu-id="ec8d4-241">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ec8d4-241">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ec8d4-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec8d4-242">DateTimeOffset</span></span>|<span data-ttu-id="ec8d4-243">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="ec8d4-243">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ec8d4-244">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ec8d4-244">serialNumber</span></span>|<span data-ttu-id="ec8d4-245">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec8d4-245">String</span></span>|<span data-ttu-id="ec8d4-246">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="ec8d4-246">SerialNumber</span></span>|
|<span data-ttu-id="ec8d4-247">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ec8d4-247">phoneNumber</span></span>|<span data-ttu-id="ec8d4-248">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-248">String</span></span>|<span data-ttu-id="ec8d4-249">Número de telefone do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-249">Phone number of the device</span></span>|
|<span data-ttu-id="ec8d4-250">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ec8d4-250">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ec8d4-251">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-251">String</span></span>|<span data-ttu-id="ec8d4-252">Nível do patch de segurança Android</span><span class="sxs-lookup"><span data-stu-id="ec8d4-252">Android security patch level</span></span>|
|<span data-ttu-id="ec8d4-253">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec8d4-253">userDisplayName</span></span>|<span data-ttu-id="ec8d4-254">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-254">String</span></span>|<span data-ttu-id="ec8d4-255">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="ec8d4-255">User display name</span></span>|
|<span data-ttu-id="ec8d4-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ec8d4-256">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ec8d4-257">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ec8d4-257">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ec8d4-258">Recursos habilitados pelo cliente do ConfigrMgr</span><span class="sxs-lookup"><span data-stu-id="ec8d4-258">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="ec8d4-259">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ec8d4-259">wiFiMacAddress</span></span>|<span data-ttu-id="ec8d4-260">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-260">String</span></span>|<span data-ttu-id="ec8d4-261">MAC Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="ec8d4-261">Wi-Fi MAC</span></span>|
|<span data-ttu-id="ec8d4-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-262">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ec8d4-263">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-263">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ec8d4-264">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-264">The device health attestation state.</span></span>|
|<span data-ttu-id="ec8d4-265">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ec8d4-265">subscriberCarrier</span></span>|<span data-ttu-id="ec8d4-266">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-266">String</span></span>|<span data-ttu-id="ec8d4-267">Operadora do assinante</span><span class="sxs-lookup"><span data-stu-id="ec8d4-267">Subscriber Carrier</span></span>|
|<span data-ttu-id="ec8d4-268">meid</span><span class="sxs-lookup"><span data-stu-id="ec8d4-268">meid</span></span>|<span data-ttu-id="ec8d4-269">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-269">String</span></span>|<span data-ttu-id="ec8d4-270">MEID</span><span class="sxs-lookup"><span data-stu-id="ec8d4-270">MEID</span></span>|
|<span data-ttu-id="ec8d4-271">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ec8d4-271">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ec8d4-272">Int64</span><span class="sxs-lookup"><span data-stu-id="ec8d4-272">Int64</span></span>|<span data-ttu-id="ec8d4-273">Total de armazenamento em bytes</span><span class="sxs-lookup"><span data-stu-id="ec8d4-273">Total Storage in Bytes</span></span>|
|<span data-ttu-id="ec8d4-274">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ec8d4-274">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ec8d4-275">Int64</span><span class="sxs-lookup"><span data-stu-id="ec8d4-275">Int64</span></span>|<span data-ttu-id="ec8d4-276">Armazenamento gratuito em bytes</span><span class="sxs-lookup"><span data-stu-id="ec8d4-276">Free Storage in Bytes</span></span>|
|<span data-ttu-id="ec8d4-277">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ec8d4-277">managedDeviceName</span></span>|<span data-ttu-id="ec8d4-278">String</span><span class="sxs-lookup"><span data-stu-id="ec8d4-278">String</span></span>|<span data-ttu-id="ec8d4-279">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-279">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ec8d4-280">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-280">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="ec8d4-281">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-281">partnerReportedThreatState</span></span>|[<span data-ttu-id="ec8d4-282">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="ec8d4-282">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ec8d4-283">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-283">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ec8d4-284">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-284">Read Only.</span></span> <span data-ttu-id="ec8d4-285">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-285">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="ec8d4-286">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec8d4-286">Response</span></span>
<span data-ttu-id="ec8d4-287">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedDevice](../resources/intune-devices-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-287">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec8d4-288">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec8d4-288">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec8d4-289">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec8d4-289">Request</span></span>
<span data-ttu-id="ec8d4-290">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-290">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec8d4-291">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec8d4-291">Response</span></span>
<span data-ttu-id="ec8d4-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec8d4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




