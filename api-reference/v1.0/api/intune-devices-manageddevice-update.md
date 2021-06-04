---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dcf132bafb6ca0023b7789c2c390a4a7869a3c9c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745811"
---
# <a name="update-manageddevice"></a><span data-ttu-id="5b8cb-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="5b8cb-103">Update managedDevice</span></span>

<span data-ttu-id="5b8cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b8cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b8cb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b8cb-106">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="5b8cb-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b8cb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b8cb-107">Prerequisites</span></span>
<span data-ttu-id="5b8cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b8cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b8cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b8cb-110">Permission type</span></span>|<span data-ttu-id="5b8cb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b8cb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b8cb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b8cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b8cb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b8cb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5b8cb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b8cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b8cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-115">Not supported.</span></span>|
|<span data-ttu-id="5b8cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b8cb-116">Application</span></span>|<span data-ttu-id="5b8cb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b8cb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b8cb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b8cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="5b8cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b8cb-119">Request headers</span></span>
|<span data-ttu-id="5b8cb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b8cb-120">Header</span></span>|<span data-ttu-id="5b8cb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b8cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b8cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b8cb-122">Authorization</span></span>|<span data-ttu-id="5b8cb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b8cb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b8cb-124">Accept</span></span>|<span data-ttu-id="5b8cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b8cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b8cb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b8cb-126">Request body</span></span>
<span data-ttu-id="5b8cb-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="5b8cb-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="5b8cb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="5b8cb-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="5b8cb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b8cb-129">Property</span></span>|<span data-ttu-id="5b8cb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b8cb-130">Type</span></span>|<span data-ttu-id="5b8cb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b8cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b8cb-132">id</span><span class="sxs-lookup"><span data-stu-id="5b8cb-132">id</span></span>|<span data-ttu-id="5b8cb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-133">String</span></span>|<span data-ttu-id="5b8cb-134">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-134">Unique Identifier for the device.</span></span> <span data-ttu-id="5b8cb-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-135">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-136">userId</span><span class="sxs-lookup"><span data-stu-id="5b8cb-136">userId</span></span>|<span data-ttu-id="5b8cb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-137">String</span></span>|<span data-ttu-id="5b8cb-138">Identificador exclusivo do usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-138">Unique Identifier for the user associated with the device.</span></span> <span data-ttu-id="5b8cb-139">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-139">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-140">deviceName</span><span class="sxs-lookup"><span data-stu-id="5b8cb-140">deviceName</span></span>|<span data-ttu-id="5b8cb-141">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-141">String</span></span>|<span data-ttu-id="5b8cb-142">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-142">Name of the device.</span></span> <span data-ttu-id="5b8cb-143">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-143">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-144">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5b8cb-144">managedDeviceOwnerType</span></span>|[<span data-ttu-id="5b8cb-145">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="5b8cb-145">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="5b8cb-146">Propriedade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-146">Ownership of the device.</span></span> <span data-ttu-id="5b8cb-147">Pode ser "empresa" ou "pessoal".</span><span class="sxs-lookup"><span data-stu-id="5b8cb-147">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="5b8cb-148">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-148">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="5b8cb-149">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="5b8cb-149">deviceActionResults</span></span>|<span data-ttu-id="5b8cb-150">Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5b8cb-150">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="5b8cb-151">Lista de objetos ComplexType deviceActionResult.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-151">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="5b8cb-152">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-152">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-153">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="5b8cb-153">enrolledDateTime</span></span>|<span data-ttu-id="5b8cb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b8cb-154">DateTimeOffset</span></span>|<span data-ttu-id="5b8cb-155">Hora de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-155">Enrollment time of the device.</span></span> <span data-ttu-id="5b8cb-156">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-156">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-157">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5b8cb-157">lastSyncDateTime</span></span>|<span data-ttu-id="5b8cb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b8cb-158">DateTimeOffset</span></span>|<span data-ttu-id="5b8cb-159">A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-159">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="5b8cb-160">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-160">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-161">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5b8cb-161">operatingSystem</span></span>|<span data-ttu-id="5b8cb-162">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-162">String</span></span>|<span data-ttu-id="5b8cb-163">Sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-163">Operating system of the device.</span></span> <span data-ttu-id="5b8cb-164">Windows, iOS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-164">Windows, iOS, etc. This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-165">complianceState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-165">complianceState</span></span>|[<span data-ttu-id="5b8cb-166">complianceState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-166">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="5b8cb-167">Estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-167">Compliance state of the device.</span></span> <span data-ttu-id="5b8cb-168">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-168">This property is read-only.</span></span> <span data-ttu-id="5b8cb-169">Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-169">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="5b8cb-170">jailBroken</span><span class="sxs-lookup"><span data-stu-id="5b8cb-170">jailBroken</span></span>|<span data-ttu-id="5b8cb-171">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-171">String</span></span>|<span data-ttu-id="5b8cb-172">se o dispositivo está desbloqueado ou modificado.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-172">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="5b8cb-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-173">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-174">managementAgent</span><span class="sxs-lookup"><span data-stu-id="5b8cb-174">managementAgent</span></span>|[<span data-ttu-id="5b8cb-175">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="5b8cb-175">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="5b8cb-176">Canal de gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-176">Management channel of the device.</span></span> <span data-ttu-id="5b8cb-177">Intune, EAS, etc. Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-177">Intune, EAS, etc. This property is read-only.</span></span> <span data-ttu-id="5b8cb-178">Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-178">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="5b8cb-179">osVersion</span><span class="sxs-lookup"><span data-stu-id="5b8cb-179">osVersion</span></span>|<span data-ttu-id="5b8cb-180">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-180">String</span></span>|<span data-ttu-id="5b8cb-181">A versão do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-181">Operating system version of the device.</span></span> <span data-ttu-id="5b8cb-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-182">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-183">easActivated</span><span class="sxs-lookup"><span data-stu-id="5b8cb-183">easActivated</span></span>|<span data-ttu-id="5b8cb-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b8cb-184">Boolean</span></span>|<span data-ttu-id="5b8cb-185">Se o dispositivo está ativado para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-185">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="5b8cb-186">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-186">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-187">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="5b8cb-187">easDeviceId</span></span>|<span data-ttu-id="5b8cb-188">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-188">String</span></span>|<span data-ttu-id="5b8cb-189">ID do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-189">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="5b8cb-190">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-190">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-191">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="5b8cb-191">easActivationDateTime</span></span>|<span data-ttu-id="5b8cb-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b8cb-192">DateTimeOffset</span></span>|<span data-ttu-id="5b8cb-193">Hora de ativação do Exchange ActiveSync do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-193">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="5b8cb-194">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-194">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-195">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="5b8cb-195">azureADRegistered</span></span>|<span data-ttu-id="5b8cb-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b8cb-196">Boolean</span></span>|<span data-ttu-id="5b8cb-197">Se o dispositivo é registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-197">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="5b8cb-198">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-198">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-199">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5b8cb-199">deviceEnrollmentType</span></span>|[<span data-ttu-id="5b8cb-200">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5b8cb-200">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="5b8cb-201">Tipo de registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-201">Enrollment type of the device.</span></span> <span data-ttu-id="5b8cb-202">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-202">This property is read-only.</span></span> <span data-ttu-id="5b8cb-203">Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment` e `appleUserEnrollmentWithServiceAccount`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-203">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.</span></span>|
|<span data-ttu-id="5b8cb-204">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="5b8cb-204">activationLockBypassCode</span></span>|<span data-ttu-id="5b8cb-205">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-205">String</span></span>|<span data-ttu-id="5b8cb-206">Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-206">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="5b8cb-207">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-207">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-208">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5b8cb-208">emailAddress</span></span>|<span data-ttu-id="5b8cb-209">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-209">String</span></span>|<span data-ttu-id="5b8cb-210">Email(s) para o usuário associado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-210">Email(s) for the user associated with the device.</span></span> <span data-ttu-id="5b8cb-211">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-211">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-212">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="5b8cb-212">azureADDeviceId</span></span>|<span data-ttu-id="5b8cb-213">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-213">String</span></span>|<span data-ttu-id="5b8cb-214">O identificador exclusivo do dispositivo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-214">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="5b8cb-215">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-215">Read only.</span></span> <span data-ttu-id="5b8cb-216">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-216">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-217">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-217">deviceRegistrationState</span></span>|[<span data-ttu-id="5b8cb-218">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-218">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="5b8cb-219">Estado do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-219">Device registration state.</span></span> <span data-ttu-id="5b8cb-220">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-220">This property is read-only.</span></span> <span data-ttu-id="5b8cb-221">Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-221">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="5b8cb-222">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="5b8cb-222">deviceCategoryDisplayName</span></span>|<span data-ttu-id="5b8cb-223">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-223">String</span></span>|<span data-ttu-id="5b8cb-224">Nome de exibição de categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-224">Device category display name.</span></span> <span data-ttu-id="5b8cb-225">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-225">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-226">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5b8cb-226">isSupervised</span></span>|<span data-ttu-id="5b8cb-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b8cb-227">Boolean</span></span>|<span data-ttu-id="5b8cb-228">Status supervisionado pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-228">Device supervised status.</span></span> <span data-ttu-id="5b8cb-229">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-229">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-230">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5b8cb-230">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="5b8cb-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b8cb-231">DateTimeOffset</span></span>|<span data-ttu-id="5b8cb-232">Última vez em que o dispositivo entrou em contato com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-232">Last time the device contacted Exchange.</span></span> <span data-ttu-id="5b8cb-233">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-233">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-234">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-234">exchangeAccessState</span></span>|[<span data-ttu-id="5b8cb-235">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-235">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="5b8cb-236">O estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-236">The Access State of the device in Exchange.</span></span> <span data-ttu-id="5b8cb-237">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-237">This property is read-only.</span></span> <span data-ttu-id="5b8cb-238">Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-238">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="5b8cb-239">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5b8cb-239">exchangeAccessStateReason</span></span>|[<span data-ttu-id="5b8cb-240">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="5b8cb-240">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="5b8cb-241">A razão para o estado de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-241">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="5b8cb-242">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-242">This property is read-only.</span></span> <span data-ttu-id="5b8cb-243">Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-243">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="5b8cb-244">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="5b8cb-244">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="5b8cb-245">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-245">String</span></span>|<span data-ttu-id="5b8cb-246">A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-246">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="5b8cb-247">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-247">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-248">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5b8cb-248">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="5b8cb-249">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-249">String</span></span>|<span data-ttu-id="5b8cb-250">Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-250">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="5b8cb-251">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-251">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-252">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5b8cb-252">isEncrypted</span></span>|<span data-ttu-id="5b8cb-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b8cb-253">Boolean</span></span>|<span data-ttu-id="5b8cb-254">Status da criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-254">Device encryption status.</span></span> <span data-ttu-id="5b8cb-255">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-255">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-256">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5b8cb-256">userPrincipalName</span></span>|<span data-ttu-id="5b8cb-257">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-257">String</span></span>|<span data-ttu-id="5b8cb-258">Nome principal do usuário do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-258">Device user principal name.</span></span> <span data-ttu-id="5b8cb-259">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-259">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-260">modelo</span><span class="sxs-lookup"><span data-stu-id="5b8cb-260">model</span></span>|<span data-ttu-id="5b8cb-261">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-261">String</span></span>|<span data-ttu-id="5b8cb-262">Modelo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-262">Model of the device.</span></span> <span data-ttu-id="5b8cb-263">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-263">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-264">fabricante</span><span class="sxs-lookup"><span data-stu-id="5b8cb-264">manufacturer</span></span>|<span data-ttu-id="5b8cb-265">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-265">String</span></span>|<span data-ttu-id="5b8cb-266">Fabricante do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-266">Manufacturer of the device.</span></span> <span data-ttu-id="5b8cb-267">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-267">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-268">imei</span><span class="sxs-lookup"><span data-stu-id="5b8cb-268">imei</span></span>|<span data-ttu-id="5b8cb-269">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-269">String</span></span>|<span data-ttu-id="5b8cb-270">IMEI.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-270">IMEI.</span></span> <span data-ttu-id="5b8cb-271">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-271">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-272">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5b8cb-272">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5b8cb-273">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b8cb-273">DateTimeOffset</span></span>|<span data-ttu-id="5b8cb-274">DateTime quando o período de carência de conformidade do dispositivo expira.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-274">The DateTime when device compliance grace period expires.</span></span> <span data-ttu-id="5b8cb-275">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-275">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5b8cb-276">serialNumber</span></span>|<span data-ttu-id="5b8cb-277">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-277">String</span></span>|<span data-ttu-id="5b8cb-278">SerialNumber.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-278">SerialNumber.</span></span> <span data-ttu-id="5b8cb-279">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-279">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="5b8cb-280">phoneNumber</span></span>|<span data-ttu-id="5b8cb-281">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-281">String</span></span>|<span data-ttu-id="5b8cb-282">Telefone número do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-282">Phone number of the device.</span></span> <span data-ttu-id="5b8cb-283">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-283">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-284">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5b8cb-284">androidSecurityPatchLevel</span></span>|<span data-ttu-id="5b8cb-285">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-285">String</span></span>|<span data-ttu-id="5b8cb-286">Nível de patch de segurança do Android.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-286">Android security patch level.</span></span> <span data-ttu-id="5b8cb-287">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-287">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-288">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5b8cb-288">userDisplayName</span></span>|<span data-ttu-id="5b8cb-289">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-289">String</span></span>|<span data-ttu-id="5b8cb-290">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-290">User display name.</span></span> <span data-ttu-id="5b8cb-291">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-291">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-292">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5b8cb-292">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="5b8cb-293">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5b8cb-293">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="5b8cb-294">Recursos habilitados para cliente ConfigrMgr.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-294">ConfigrMgr client enabled features.</span></span> <span data-ttu-id="5b8cb-295">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-295">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-296">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="5b8cb-296">wiFiMacAddress</span></span>|<span data-ttu-id="5b8cb-297">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-297">String</span></span>|<span data-ttu-id="5b8cb-298">Wi-Fi MAC.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-298">Wi-Fi MAC.</span></span> <span data-ttu-id="5b8cb-299">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-299">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-300">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-300">deviceHealthAttestationState</span></span>|[<span data-ttu-id="5b8cb-301">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-301">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="5b8cb-302">O estado do atestado de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-302">The device health attestation state.</span></span> <span data-ttu-id="5b8cb-303">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-303">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-304">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="5b8cb-304">subscriberCarrier</span></span>|<span data-ttu-id="5b8cb-305">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-305">String</span></span>|<span data-ttu-id="5b8cb-306">Operadora de Assinantes.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-306">Subscriber Carrier.</span></span> <span data-ttu-id="5b8cb-307">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-307">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-308">meid</span><span class="sxs-lookup"><span data-stu-id="5b8cb-308">meid</span></span>|<span data-ttu-id="5b8cb-309">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-309">String</span></span>|<span data-ttu-id="5b8cb-310">MEID.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-310">MEID.</span></span> <span data-ttu-id="5b8cb-311">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-311">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-312">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5b8cb-312">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="5b8cb-313">Int64</span><span class="sxs-lookup"><span data-stu-id="5b8cb-313">Int64</span></span>|<span data-ttu-id="5b8cb-314">Total Armazenamento em Bytes.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-314">Total Storage in Bytes.</span></span> <span data-ttu-id="5b8cb-315">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-315">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-316">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="5b8cb-316">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="5b8cb-317">Int64</span><span class="sxs-lookup"><span data-stu-id="5b8cb-317">Int64</span></span>|<span data-ttu-id="5b8cb-318">Free Armazenamento em Bytes.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-318">Free Storage in Bytes.</span></span> <span data-ttu-id="5b8cb-319">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-319">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-320">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="5b8cb-320">managedDeviceName</span></span>|<span data-ttu-id="5b8cb-321">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-321">String</span></span>|<span data-ttu-id="5b8cb-322">Nome gerado automaticamente para identificar um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-322">Automatically generated name to identify a device.</span></span> <span data-ttu-id="5b8cb-323">Pode ser substituído por um nome amigável ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-323">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="5b8cb-324">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-324">partnerReportedThreatState</span></span>|[<span data-ttu-id="5b8cb-325">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="5b8cb-325">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="5b8cb-326">Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-326">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="5b8cb-327">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-327">Read Only.</span></span> <span data-ttu-id="5b8cb-328">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-328">This property is read-only.</span></span> <span data-ttu-id="5b8cb-329">Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-329">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="5b8cb-330">iccid</span><span class="sxs-lookup"><span data-stu-id="5b8cb-330">iccid</span></span>|<span data-ttu-id="5b8cb-331">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-331">String</span></span>|<span data-ttu-id="5b8cb-332">Identificador integrado de cartão de circuito, é o número de identificação exclusivo de um cartão SIM.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-332">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="5b8cb-333">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-333">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-334">udid</span><span class="sxs-lookup"><span data-stu-id="5b8cb-334">udid</span></span>|<span data-ttu-id="5b8cb-335">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-335">String</span></span>|<span data-ttu-id="5b8cb-336">Identificador de dispositivo exclusivo para dispositivos iOS e macOS.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-336">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="5b8cb-337">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-337">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-338">notes</span><span class="sxs-lookup"><span data-stu-id="5b8cb-338">notes</span></span>|<span data-ttu-id="5b8cb-339">String</span><span class="sxs-lookup"><span data-stu-id="5b8cb-339">String</span></span>|<span data-ttu-id="5b8cb-340">Observações sobre o dispositivo criado pelo administrador de IT</span><span class="sxs-lookup"><span data-stu-id="5b8cb-340">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="5b8cb-341">ethernetMacAddress</span><span class="sxs-lookup"><span data-stu-id="5b8cb-341">ethernetMacAddress</span></span>|<span data-ttu-id="5b8cb-342">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b8cb-342">String</span></span>|<span data-ttu-id="5b8cb-343">Ethernet MAC.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-343">Ethernet MAC.</span></span> <span data-ttu-id="5b8cb-344">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-344">This property is read-only.</span></span>|
|<span data-ttu-id="5b8cb-345">physicalMemoryInBytes</span><span class="sxs-lookup"><span data-stu-id="5b8cb-345">physicalMemoryInBytes</span></span>|<span data-ttu-id="5b8cb-346">Int64</span><span class="sxs-lookup"><span data-stu-id="5b8cb-346">Int64</span></span>|<span data-ttu-id="5b8cb-347">Memória total em bytes.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-347">Total Memory in Bytes.</span></span> <span data-ttu-id="5b8cb-348">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-348">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="5b8cb-349">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b8cb-349">Response</span></span>
<span data-ttu-id="5b8cb-350">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-devices-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-350">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b8cb-351">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b8cb-351">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b8cb-352">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b8cb-352">Request</span></span>
<span data-ttu-id="5b8cb-353">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-353">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
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

### <a name="response"></a><span data-ttu-id="5b8cb-354">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b8cb-354">Response</span></span>
<span data-ttu-id="5b8cb-p153">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b8cb-p153">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




