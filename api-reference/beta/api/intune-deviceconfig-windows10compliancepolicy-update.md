---
title: Atualizar windows10CompliancePolicy
description: Atualiza as propriedades de um objeto windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f799d0e3bffd3174500c4b5b0da5e62d73d0150
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43340524"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="4592f-103">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4592f-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="4592f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4592f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4592f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4592f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4592f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4592f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4592f-107">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4592f-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4592f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4592f-108">Prerequisites</span></span>
<span data-ttu-id="4592f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4592f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4592f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4592f-111">Permission type</span></span>|<span data-ttu-id="4592f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4592f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4592f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4592f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4592f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4592f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4592f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4592f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4592f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4592f-116">Not supported.</span></span>|
|<span data-ttu-id="4592f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4592f-117">Application</span></span>|<span data-ttu-id="4592f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4592f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4592f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4592f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4592f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4592f-120">Request headers</span></span>
|<span data-ttu-id="4592f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4592f-121">Header</span></span>|<span data-ttu-id="4592f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4592f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4592f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4592f-123">Authorization</span></span>|<span data-ttu-id="4592f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4592f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4592f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4592f-125">Accept</span></span>|<span data-ttu-id="4592f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4592f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4592f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4592f-127">Request body</span></span>
<span data-ttu-id="4592f-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4592f-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="4592f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4592f-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="4592f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4592f-130">Property</span></span>|<span data-ttu-id="4592f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4592f-131">Type</span></span>|<span data-ttu-id="4592f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4592f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4592f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4592f-133">roleScopeTagIds</span></span>|<span data-ttu-id="4592f-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4592f-134">String collection</span></span>|<span data-ttu-id="4592f-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4592f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4592f-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-137">id</span><span class="sxs-lookup"><span data-stu-id="4592f-137">id</span></span>|<span data-ttu-id="4592f-138">String</span><span class="sxs-lookup"><span data-stu-id="4592f-138">String</span></span>|<span data-ttu-id="4592f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4592f-139">Key of the entity.</span></span> <span data-ttu-id="4592f-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4592f-141">createdDateTime</span></span>|<span data-ttu-id="4592f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4592f-142">DateTimeOffset</span></span>|<span data-ttu-id="4592f-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4592f-143">DateTime the object was created.</span></span> <span data-ttu-id="4592f-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-145">description</span><span class="sxs-lookup"><span data-stu-id="4592f-145">description</span></span>|<span data-ttu-id="4592f-146">String</span><span class="sxs-lookup"><span data-stu-id="4592f-146">String</span></span>|<span data-ttu-id="4592f-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4592f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4592f-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4592f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4592f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4592f-150">DateTimeOffset</span></span>|<span data-ttu-id="4592f-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4592f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="4592f-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4592f-153">displayName</span></span>|<span data-ttu-id="4592f-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4592f-154">String</span></span>|<span data-ttu-id="4592f-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4592f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4592f-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-157">version</span><span class="sxs-lookup"><span data-stu-id="4592f-157">version</span></span>|<span data-ttu-id="4592f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4592f-158">Int32</span></span>|<span data-ttu-id="4592f-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4592f-159">Version of the device configuration.</span></span> <span data-ttu-id="4592f-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4592f-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4592f-161">passwordRequired</span></span>|<span data-ttu-id="4592f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-162">Boolean</span></span>|<span data-ttu-id="4592f-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="4592f-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4592f-164">passwordBlockSimple</span></span>|<span data-ttu-id="4592f-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-165">Boolean</span></span>|<span data-ttu-id="4592f-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4592f-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="4592f-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="4592f-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="4592f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-168">Boolean</span></span>|<span data-ttu-id="4592f-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="4592f-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="4592f-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4592f-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4592f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4592f-171">Int32</span></span>|<span data-ttu-id="4592f-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="4592f-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4592f-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4592f-173">passwordExpirationDays</span></span>|<span data-ttu-id="4592f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4592f-174">Int32</span></span>|<span data-ttu-id="4592f-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="4592f-175">The password expiration in days.</span></span>|
|<span data-ttu-id="4592f-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4592f-176">passwordMinimumLength</span></span>|<span data-ttu-id="4592f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4592f-177">Int32</span></span>|<span data-ttu-id="4592f-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="4592f-178">The minimum password length.</span></span>|
|<span data-ttu-id="4592f-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4592f-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4592f-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4592f-180">Int32</span></span>|<span data-ttu-id="4592f-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="4592f-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4592f-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4592f-182">passwordRequiredType</span></span>|[<span data-ttu-id="4592f-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4592f-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4592f-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="4592f-184">The required password type.</span></span> <span data-ttu-id="4592f-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4592f-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4592f-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4592f-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4592f-187">Int32</span><span class="sxs-lookup"><span data-stu-id="4592f-187">Int32</span></span>|<span data-ttu-id="4592f-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="4592f-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="4592f-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="4592f-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="4592f-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-190">Boolean</span></span>|<span data-ttu-id="4592f-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4592f-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4592f-192">osMinimumVersion</span></span>|<span data-ttu-id="4592f-193">String</span><span class="sxs-lookup"><span data-stu-id="4592f-193">String</span></span>|<span data-ttu-id="4592f-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4592f-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="4592f-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4592f-195">osMaximumVersion</span></span>|<span data-ttu-id="4592f-196">String</span><span class="sxs-lookup"><span data-stu-id="4592f-196">String</span></span>|<span data-ttu-id="4592f-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4592f-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="4592f-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4592f-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="4592f-199">String</span><span class="sxs-lookup"><span data-stu-id="4592f-199">String</span></span>|<span data-ttu-id="4592f-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4592f-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="4592f-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4592f-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="4592f-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4592f-202">String</span></span>|<span data-ttu-id="4592f-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4592f-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="4592f-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="4592f-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-205">Boolean</span></span>|<span data-ttu-id="4592f-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="4592f-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="4592f-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-207">bitLockerEnabled</span></span>|<span data-ttu-id="4592f-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-208">Boolean</span></span>|<span data-ttu-id="4592f-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="4592f-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="4592f-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-210">secureBootEnabled</span></span>|<span data-ttu-id="4592f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-211">Boolean</span></span>|<span data-ttu-id="4592f-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="4592f-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="4592f-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="4592f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-214">Boolean</span></span>|<span data-ttu-id="4592f-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4592f-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4592f-216">storageRequireEncryption</span></span>|<span data-ttu-id="4592f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-217">Boolean</span></span>|<span data-ttu-id="4592f-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="4592f-219">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="4592f-219">activeFirewallRequired</span></span>|<span data-ttu-id="4592f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-220">Boolean</span></span>|<span data-ttu-id="4592f-221">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="4592f-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-222">defenderEnabled</span></span>|<span data-ttu-id="4592f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-223">Boolean</span></span>|<span data-ttu-id="4592f-224">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="4592f-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="4592f-225">defenderVersion</span></span>|<span data-ttu-id="4592f-226">String</span><span class="sxs-lookup"><span data-stu-id="4592f-226">String</span></span>|<span data-ttu-id="4592f-227">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="4592f-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="4592f-228">signatureOutOfDate</span></span>|<span data-ttu-id="4592f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-229">Boolean</span></span>|<span data-ttu-id="4592f-230">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="4592f-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-231">rtpEnabled</span></span>|<span data-ttu-id="4592f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-232">Boolean</span></span>|<span data-ttu-id="4592f-233">Requer a proteção em tempo real do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="4592f-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="4592f-234">antivirusRequired</span></span>|<span data-ttu-id="4592f-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-235">Boolean</span></span>|<span data-ttu-id="4592f-236">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="4592f-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="4592f-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="4592f-237">antiSpywareRequired</span></span>|<span data-ttu-id="4592f-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-238">Boolean</span></span>|<span data-ttu-id="4592f-239">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="4592f-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="4592f-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="4592f-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="4592f-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="4592f-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="4592f-242">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4592f-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="4592f-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="4592f-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4592f-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4592f-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4592f-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-245">Boolean</span></span>|<span data-ttu-id="4592f-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="4592f-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4592f-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4592f-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4592f-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4592f-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4592f-249">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="4592f-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4592f-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4592f-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4592f-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="4592f-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="4592f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-252">Boolean</span></span>|<span data-ttu-id="4592f-253">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="4592f-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="4592f-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="4592f-254">tpmRequired</span></span>|<span data-ttu-id="4592f-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="4592f-255">Boolean</span></span>|<span data-ttu-id="4592f-256">Requer o módulo de plataforma confiável (TPM) para estar presente.</span><span class="sxs-lookup"><span data-stu-id="4592f-256">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="4592f-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="4592f-257">Response</span></span>
<span data-ttu-id="4592f-258">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4592f-258">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4592f-259">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4592f-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="4592f-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4592f-260">Request</span></span>
<span data-ttu-id="4592f-261">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4592f-261">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1690

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```

### <a name="response"></a><span data-ttu-id="4592f-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="4592f-262">Response</span></span>
<span data-ttu-id="4592f-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4592f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1862

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```



