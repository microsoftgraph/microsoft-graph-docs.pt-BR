---
title: Criar managedDevice
description: Criar um novo objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bdd3bc460148298b91386e6ce0988f743cc78e5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756152"
---
# <a name="create-manageddevice"></a><span data-ttu-id="b2fe4-103">Criar managedDevice</span><span class="sxs-lookup"><span data-stu-id="b2fe4-103">Create managedDevice</span></span>

<span data-ttu-id="b2fe4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2fe4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2fe4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2fe4-106">Criar um novo objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b2fe4-106">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2fe4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2fe4-107">Prerequisites</span></span>
<span data-ttu-id="b2fe4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2fe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2fe4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2fe4-110">Permission type</span></span>|<span data-ttu-id="b2fe4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2fe4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2fe4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2fe4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2fe4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fe4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b2fe4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2fe4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2fe4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-115">Not supported.</span></span>|
|<span data-ttu-id="b2fe4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2fe4-116">Application</span></span>|<span data-ttu-id="b2fe4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fe4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2fe4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2fe4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="b2fe4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2fe4-119">Request headers</span></span>
|<span data-ttu-id="b2fe4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2fe4-120">Header</span></span>|<span data-ttu-id="b2fe4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2fe4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2fe4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2fe4-122">Authorization</span></span>|<span data-ttu-id="b2fe4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2fe4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2fe4-124">Accept</span></span>|<span data-ttu-id="b2fe4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2fe4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2fe4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2fe4-126">Request body</span></span>
<span data-ttu-id="b2fe4-127">No corpo da solicitação, forneça uma representação JSON do objeto managedDevice.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-127">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="b2fe4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDevice.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-128">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="b2fe4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2fe4-129">Property</span></span>|<span data-ttu-id="b2fe4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2fe4-130">Type</span></span>|<span data-ttu-id="b2fe4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2fe4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2fe4-132">id</span><span class="sxs-lookup"><span data-stu-id="b2fe4-132">id</span></span>|<span data-ttu-id="b2fe4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-133">String</span></span>|<span data-ttu-id="b2fe4-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-134">Unique Identifier for the device.</span></span> <span data-ttu-id="b2fe4-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-135">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-136">userId</span><span class="sxs-lookup"><span data-stu-id="b2fe4-136">userId</span></span>|<span data-ttu-id="b2fe4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-137">String</span></span>|<span data-ttu-id="b2fe4-138">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="b2fe4-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-139">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="b2fe4-140">deviceName</span></span>|<span data-ttu-id="b2fe4-141">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-141">String</span></span>|<span data-ttu-id="b2fe4-142">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-142">Name of the device.</span></span> <span data-ttu-id="b2fe4-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-143">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-144">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b2fe4-144">managedDeviceOwnerType</span></span>|[<span data-ttu-id="b2fe4-145">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b2fe4-145">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="b2fe4-146">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-146">Ownership of the device.</span></span> <span data-ttu-id="b2fe4-147">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="b2fe4-147">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="b2fe4-148">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-148">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="b2fe4-149">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="b2fe4-149">deviceActionResults</span></span>|<span data-ttu-id="b2fe4-150">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b2fe4-150">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="b2fe4-151">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-151">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="b2fe4-152">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-152">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-153">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="b2fe4-153">enrolledDateTime</span></span>|<span data-ttu-id="b2fe4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2fe4-154">DateTimeOffset</span></span>|<span data-ttu-id="b2fe4-155">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-155">Enrollment time of the device.</span></span> <span data-ttu-id="b2fe4-156">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-156">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-157">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b2fe4-157">lastSyncDateTime</span></span>|<span data-ttu-id="b2fe4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2fe4-158">DateTimeOffset</span></span>|<span data-ttu-id="b2fe4-159">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-159">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="b2fe4-160">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-160">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-161">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2fe4-161">operatingSystem</span></span>|<span data-ttu-id="b2fe4-162">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-162">String</span></span>|<span data-ttu-id="b2fe4-163">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-163">Operating system of the device.</span></span> <span data-ttu-id="b2fe4-164">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-164">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-165">complianceState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-165">complianceState</span></span>|[<span data-ttu-id="b2fe4-166">complianceState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-166">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="b2fe4-167">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-167">Compliance state of the device.</span></span> <span data-ttu-id="b2fe4-168">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-168">This property is read-only.</span></span> <span data-ttu-id="b2fe4-169">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-169">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="b2fe4-170">jailBroken</span><span class="sxs-lookup"><span data-stu-id="b2fe4-170">jailBroken</span></span>|<span data-ttu-id="b2fe4-171">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-171">String</span></span>|<span data-ttu-id="b2fe4-172">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-172">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="b2fe4-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-173">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-174">managementAgent</span><span class="sxs-lookup"><span data-stu-id="b2fe4-174">managementAgent</span></span>|[<span data-ttu-id="b2fe4-175">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="b2fe4-175">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="b2fe4-176">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-176">Management channel of the device.</span></span> <span data-ttu-id="b2fe4-177">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-177">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="b2fe4-178">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-178">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="b2fe4-179">osVersion</span><span class="sxs-lookup"><span data-stu-id="b2fe4-179">osVersion</span></span>|<span data-ttu-id="b2fe4-180">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-180">String</span></span>|<span data-ttu-id="b2fe4-181">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-181">Operating system version of the device.</span></span> <span data-ttu-id="b2fe4-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-182">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-183">easActivated</span><span class="sxs-lookup"><span data-stu-id="b2fe4-183">easActivated</span></span>|<span data-ttu-id="b2fe4-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fe4-184">Boolean</span></span>|<span data-ttu-id="b2fe4-185">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-185">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="b2fe4-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-186">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-187">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="b2fe4-187">easDeviceId</span></span>|<span data-ttu-id="b2fe4-188">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-188">String</span></span>|<span data-ttu-id="b2fe4-189">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-189">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="b2fe4-190">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-190">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-191">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="b2fe4-191">easActivationDateTime</span></span>|<span data-ttu-id="b2fe4-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2fe4-192">DateTimeOffset</span></span>|<span data-ttu-id="b2fe4-193">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-193">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="b2fe4-194">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-194">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-195">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="b2fe4-195">azureADRegistered</span></span>|<span data-ttu-id="b2fe4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fe4-196">Boolean</span></span>|<span data-ttu-id="b2fe4-197">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-197">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="b2fe4-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-198">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-199">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b2fe4-199">deviceEnrollmentType</span></span>|[<span data-ttu-id="b2fe4-200">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b2fe4-200">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="b2fe4-201">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-201">Enrollment type of the device.</span></span> <span data-ttu-id="b2fe4-202">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-202">This property is read-only.</span></span> <span data-ttu-id="b2fe4-203">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment` e `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-203">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="b2fe4-204">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="b2fe4-204">activationLockBypassCode</span></span>|<span data-ttu-id="b2fe4-205">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-205">String</span></span>|<span data-ttu-id="b2fe4-206">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-206">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="b2fe4-207">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-207">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-208">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b2fe4-208">emailAddress</span></span>|<span data-ttu-id="b2fe4-209">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-209">String</span></span>|<span data-ttu-id="b2fe4-210">Email(s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-210">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="b2fe4-211">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-211">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-212">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="b2fe4-212">azureADDeviceId</span></span>|<span data-ttu-id="b2fe4-213">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-213">String</span></span>|<span data-ttu-id="b2fe4-214">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-214">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="b2fe4-215">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-215">Read only.</span></span> <span data-ttu-id="b2fe4-216">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-216">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-217">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-217">deviceRegistrationState</span></span>|[<span data-ttu-id="b2fe4-218">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-218">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="b2fe4-219">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-219">Device registration state.</span></span> <span data-ttu-id="b2fe4-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-220">This property is read-only.</span></span> <span data-ttu-id="b2fe4-221">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-221">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="b2fe4-222">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="b2fe4-222">deviceCategoryDisplayName</span></span>|<span data-ttu-id="b2fe4-223">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-223">String</span></span>|<span data-ttu-id="b2fe4-224">Nome de exibição de categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-224">Device category display name.</span></span> <span data-ttu-id="b2fe4-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-225">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-226">isSupervised</span><span class="sxs-lookup"><span data-stu-id="b2fe4-226">isSupervised</span></span>|<span data-ttu-id="b2fe4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fe4-227">Boolean</span></span>|<span data-ttu-id="b2fe4-228">Status supervisionado pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-228">Device supervised status.</span></span> <span data-ttu-id="b2fe4-229">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-229">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-230">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b2fe4-230">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b2fe4-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2fe4-231">DateTimeOffset</span></span>|<span data-ttu-id="b2fe4-232">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-232">Last time the device contacted Exchange.</span></span> <span data-ttu-id="b2fe4-233">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-233">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-234">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-234">exchangeAccessState</span></span>|[<span data-ttu-id="b2fe4-235">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-235">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="b2fe4-236">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-236">The Access State of the device in Exchange.</span></span> <span data-ttu-id="b2fe4-237">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-237">This property is read-only.</span></span> <span data-ttu-id="b2fe4-238">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-238">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="b2fe4-239">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="b2fe4-239">exchangeAccessStateReason</span></span>|[<span data-ttu-id="b2fe4-240">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="b2fe4-240">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="b2fe4-241">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-241">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="b2fe4-242">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-242">This property is read-only.</span></span> <span data-ttu-id="b2fe4-243">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-243">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="b2fe4-244">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="b2fe4-244">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="b2fe4-245">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-245">String</span></span>|<span data-ttu-id="b2fe4-246">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-246">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="b2fe4-247">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-247">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-248">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b2fe4-248">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="b2fe4-249">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-249">String</span></span>|<span data-ttu-id="b2fe4-250">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-250">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="b2fe4-251">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-251">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-252">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b2fe4-252">isEncrypted</span></span>|<span data-ttu-id="b2fe4-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2fe4-253">Boolean</span></span>|<span data-ttu-id="b2fe4-254">Status da criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-254">Device encryption status.</span></span> <span data-ttu-id="b2fe4-255">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-255">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-256">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b2fe4-256">userPrincipalName</span></span>|<span data-ttu-id="b2fe4-257">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-257">String</span></span>|<span data-ttu-id="b2fe4-258">Nome principal do usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-258">Device user principal name.</span></span> <span data-ttu-id="b2fe4-259">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-259">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-260">modelo</span><span class="sxs-lookup"><span data-stu-id="b2fe4-260">model</span></span>|<span data-ttu-id="b2fe4-261">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-261">String</span></span>|<span data-ttu-id="b2fe4-262">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-262">Model of the device.</span></span> <span data-ttu-id="b2fe4-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-263">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-264">fabricante</span><span class="sxs-lookup"><span data-stu-id="b2fe4-264">manufacturer</span></span>|<span data-ttu-id="b2fe4-265">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-265">String</span></span>|<span data-ttu-id="b2fe4-266">Fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-266">Manufacturer of the device.</span></span> <span data-ttu-id="b2fe4-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-267">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-268">imei</span><span class="sxs-lookup"><span data-stu-id="b2fe4-268">imei</span></span>|<span data-ttu-id="b2fe4-269">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-269">String</span></span>|<span data-ttu-id="b2fe4-270">IMEI.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-270">IMEI.</span></span> <span data-ttu-id="b2fe4-271">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-271">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-272">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b2fe4-272">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b2fe4-273">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2fe4-273">DateTimeOffset</span></span>|<span data-ttu-id="b2fe4-274">DateTime quando o período de carência de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-274">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="b2fe4-275">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-275">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b2fe4-276">serialNumber</span></span>|<span data-ttu-id="b2fe4-277">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-277">String</span></span>|<span data-ttu-id="b2fe4-278">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-278">SerialNumber.</span></span> <span data-ttu-id="b2fe4-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-279">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b2fe4-280">phoneNumber</span></span>|<span data-ttu-id="b2fe4-281">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-281">String</span></span>|<span data-ttu-id="b2fe4-282">Telefone número do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-282">Phone number of the device.</span></span> <span data-ttu-id="b2fe4-283">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-283">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-284">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b2fe4-284">androidSecurityPatchLevel</span></span>|<span data-ttu-id="b2fe4-285">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-285">String</span></span>|<span data-ttu-id="b2fe4-286">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-286">Android security patch level.</span></span> <span data-ttu-id="b2fe4-287">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-287">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-288">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b2fe4-288">userDisplayName</span></span>|<span data-ttu-id="b2fe4-289">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-289">String</span></span>|<span data-ttu-id="b2fe4-290">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-290">User display name.</span></span> <span data-ttu-id="b2fe4-291">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-291">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-292">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b2fe4-292">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="b2fe4-293">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b2fe4-293">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="b2fe4-294">Recursos habilitados para cliente ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-294">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="b2fe4-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-295">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-296">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="b2fe4-296">wiFiMacAddress</span></span>|<span data-ttu-id="b2fe4-297">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-297">String</span></span>|<span data-ttu-id="b2fe4-298">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-298">Wi-Fi MAC.</span></span> <span data-ttu-id="b2fe4-299">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-299">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-300">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-300">deviceHealthAttestationState</span></span>|[<span data-ttu-id="b2fe4-301">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-301">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="b2fe4-302">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-302">The device health attestation state.</span></span> <span data-ttu-id="b2fe4-303">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-303">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-304">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="b2fe4-304">subscriberCarrier</span></span>|<span data-ttu-id="b2fe4-305">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-305">String</span></span>|<span data-ttu-id="b2fe4-306">Operadora de Assinantes.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-306">Subscriber Carrier.</span></span> <span data-ttu-id="b2fe4-307">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-307">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-308">meid</span><span class="sxs-lookup"><span data-stu-id="b2fe4-308">meid</span></span>|<span data-ttu-id="b2fe4-309">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-309">String</span></span>|<span data-ttu-id="b2fe4-310">MEID.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-310">MEID.</span></span> <span data-ttu-id="b2fe4-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-311">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-312">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="b2fe4-312">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="b2fe4-313">Int64</span><span class="sxs-lookup"><span data-stu-id="b2fe4-313">Int64</span></span>|<span data-ttu-id="b2fe4-314">Total Armazenamento em Bytes.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-314">Total Storage in Bytes.</span></span> <span data-ttu-id="b2fe4-315">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-315">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-316">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="b2fe4-316">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="b2fe4-317">Int64</span><span class="sxs-lookup"><span data-stu-id="b2fe4-317">Int64</span></span>|<span data-ttu-id="b2fe4-318">Free Armazenamento em Bytes.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-318">Free Storage in Bytes.</span></span> <span data-ttu-id="b2fe4-319">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-319">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-320">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b2fe4-320">managedDeviceName</span></span>|<span data-ttu-id="b2fe4-321">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-321">String</span></span>|<span data-ttu-id="b2fe4-322">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-322">Automatically generated name to identify a device.</span></span> <span data-ttu-id="b2fe4-323">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-323">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="b2fe4-324">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-324">partnerReportedThreatState</span></span>|[<span data-ttu-id="b2fe4-325">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="b2fe4-325">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="b2fe4-326">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-326">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="b2fe4-327">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-327">Read Only.</span></span> <span data-ttu-id="b2fe4-328">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-328">This property is read-only.</span></span> <span data-ttu-id="b2fe4-329">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-329">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="b2fe4-330">iccid</span><span class="sxs-lookup"><span data-stu-id="b2fe4-330">iccid</span></span>|<span data-ttu-id="b2fe4-331">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-331">String</span></span>|<span data-ttu-id="b2fe4-332">Identificador integrado de cartão de circuito, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-332">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="b2fe4-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-333">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-334">udid</span><span class="sxs-lookup"><span data-stu-id="b2fe4-334">udid</span></span>|<span data-ttu-id="b2fe4-335">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-335">String</span></span>|<span data-ttu-id="b2fe4-336">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-336">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="b2fe4-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-337">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-338">notes</span><span class="sxs-lookup"><span data-stu-id="b2fe4-338">notes</span></span>|<span data-ttu-id="b2fe4-339">String</span><span class="sxs-lookup"><span data-stu-id="b2fe4-339">String</span></span>|<span data-ttu-id="b2fe4-340">Observações sobre o dispositivo criado pelo administrador de IT</span><span class="sxs-lookup"><span data-stu-id="b2fe4-340">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="b2fe4-341">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="b2fe4-341">ethernetMacAddress</span></span>|<span data-ttu-id="b2fe4-342">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2fe4-342">String</span></span>|<span data-ttu-id="b2fe4-343">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-343">Ethernet MAC.</span></span> <span data-ttu-id="b2fe4-344">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-344">This property is read-only.</span></span>|
|<span data-ttu-id="b2fe4-345">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="b2fe4-345">physicalMemoryInBytes</span></span>|<span data-ttu-id="b2fe4-346">Int64</span><span class="sxs-lookup"><span data-stu-id="b2fe4-346">Int64</span></span>|<span data-ttu-id="b2fe4-347">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-347">Total Memory in Bytes.</span></span> <span data-ttu-id="b2fe4-348">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-348">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="b2fe4-349">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2fe4-349">Response</span></span>
<span data-ttu-id="b2fe4-350">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedDevice](../resources/intune-devices-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-350">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2fe4-351">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2fe4-351">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2fe4-352">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2fe4-352">Request</span></span>
<span data-ttu-id="b2fe4-353">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-353">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4821

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
  "partnerReportedThreatState": "activated",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "notes": "Notes value",
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5
}
```

### <a name="response"></a><span data-ttu-id="b2fe4-354">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2fe4-354">Response</span></span>
<span data-ttu-id="b2fe4-p153">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2fe4-p153">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4870

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
  "partnerReportedThreatState": "activated",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "notes": "Notes value",
  "ethernetMacAddress": "Ethernet Mac Address value",
  "physicalMemoryInBytes": 5
}
```




