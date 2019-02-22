---
title: Atualizar windows10CompliancePolicy
description: Atualiza as propriedades de um objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4d24c0d964fd43e12c4fcd9a3ff91a0bcd1238b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172265"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="bc865-103">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bc865-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="bc865-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc865-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc865-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc865-106">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc865-106">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc865-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc865-107">Prerequisites</span></span>
<span data-ttu-id="bc865-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc865-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc865-110">Permission type</span></span>|<span data-ttu-id="bc865-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc865-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc865-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc865-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc865-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc865-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc865-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc865-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc865-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc865-115">Not supported.</span></span>|
|<span data-ttu-id="bc865-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc865-116">Application</span></span>|<span data-ttu-id="bc865-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc865-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc865-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc865-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bc865-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc865-119">Request headers</span></span>
|<span data-ttu-id="bc865-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc865-120">Header</span></span>|<span data-ttu-id="bc865-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bc865-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc865-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc865-122">Authorization</span></span>|<span data-ttu-id="bc865-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc865-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc865-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc865-124">Accept</span></span>|<span data-ttu-id="bc865-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc865-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc865-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc865-126">Request body</span></span>
<span data-ttu-id="bc865-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc865-127">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="bc865-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc865-128">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="bc865-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc865-129">Property</span></span>|<span data-ttu-id="bc865-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc865-130">Type</span></span>|<span data-ttu-id="bc865-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc865-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc865-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc865-132">roleScopeTagIds</span></span>|<span data-ttu-id="bc865-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc865-133">String collection</span></span>|<span data-ttu-id="bc865-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bc865-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bc865-135">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-136">id</span><span class="sxs-lookup"><span data-stu-id="bc865-136">id</span></span>|<span data-ttu-id="bc865-137">String</span><span class="sxs-lookup"><span data-stu-id="bc865-137">String</span></span>|<span data-ttu-id="bc865-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc865-138">Key of the entity.</span></span> <span data-ttu-id="bc865-139">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc865-140">createdDateTime</span></span>|<span data-ttu-id="bc865-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc865-141">DateTimeOffset</span></span>|<span data-ttu-id="bc865-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bc865-142">DateTime the object was created.</span></span> <span data-ttu-id="bc865-143">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-144">description</span><span class="sxs-lookup"><span data-stu-id="bc865-144">description</span></span>|<span data-ttu-id="bc865-145">String</span><span class="sxs-lookup"><span data-stu-id="bc865-145">String</span></span>|<span data-ttu-id="bc865-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc865-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc865-147">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc865-148">lastModifiedDateTime</span></span>|<span data-ttu-id="bc865-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc865-149">DateTimeOffset</span></span>|<span data-ttu-id="bc865-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bc865-150">DateTime the object was last modified.</span></span> <span data-ttu-id="bc865-151">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bc865-152">displayName</span></span>|<span data-ttu-id="bc865-153">String</span><span class="sxs-lookup"><span data-stu-id="bc865-153">String</span></span>|<span data-ttu-id="bc865-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc865-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc865-155">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-156">version</span><span class="sxs-lookup"><span data-stu-id="bc865-156">version</span></span>|<span data-ttu-id="bc865-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bc865-157">Int32</span></span>|<span data-ttu-id="bc865-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc865-158">Version of the device configuration.</span></span> <span data-ttu-id="bc865-159">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc865-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bc865-160">passwordRequired</span></span>|<span data-ttu-id="bc865-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-161">Boolean</span></span>|<span data-ttu-id="bc865-162">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="bc865-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bc865-163">passwordBlockSimple</span></span>|<span data-ttu-id="bc865-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc865-164">Boolean</span></span>|<span data-ttu-id="bc865-165">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc865-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="bc865-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="bc865-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="bc865-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-167">Boolean</span></span>|<span data-ttu-id="bc865-168">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="bc865-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="bc865-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bc865-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bc865-170">Int32</span><span class="sxs-lookup"><span data-stu-id="bc865-170">Int32</span></span>|<span data-ttu-id="bc865-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="bc865-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bc865-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bc865-172">passwordExpirationDays</span></span>|<span data-ttu-id="bc865-173">Int32</span><span class="sxs-lookup"><span data-stu-id="bc865-173">Int32</span></span>|<span data-ttu-id="bc865-174">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="bc865-174">The password expiration in days.</span></span>|
|<span data-ttu-id="bc865-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bc865-175">passwordMinimumLength</span></span>|<span data-ttu-id="bc865-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bc865-176">Int32</span></span>|<span data-ttu-id="bc865-177">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="bc865-177">The minimum password length.</span></span>|
|<span data-ttu-id="bc865-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bc865-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bc865-179">Int32</span><span class="sxs-lookup"><span data-stu-id="bc865-179">Int32</span></span>|<span data-ttu-id="bc865-180">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="bc865-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bc865-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bc865-181">passwordRequiredType</span></span>|[<span data-ttu-id="bc865-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bc865-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bc865-183">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="bc865-183">The required password type.</span></span> <span data-ttu-id="bc865-184">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bc865-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bc865-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bc865-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bc865-186">Int32</span><span class="sxs-lookup"><span data-stu-id="bc865-186">Int32</span></span>|<span data-ttu-id="bc865-187">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="bc865-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="bc865-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="bc865-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="bc865-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-189">Boolean</span></span>|<span data-ttu-id="bc865-190">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="bc865-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bc865-191">osMinimumVersion</span></span>|<span data-ttu-id="bc865-192">String</span><span class="sxs-lookup"><span data-stu-id="bc865-192">String</span></span>|<span data-ttu-id="bc865-193">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bc865-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="bc865-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bc865-194">osMaximumVersion</span></span>|<span data-ttu-id="bc865-195">String</span><span class="sxs-lookup"><span data-stu-id="bc865-195">String</span></span>|<span data-ttu-id="bc865-196">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bc865-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="bc865-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bc865-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="bc865-198">String</span><span class="sxs-lookup"><span data-stu-id="bc865-198">String</span></span>|<span data-ttu-id="bc865-199">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="bc865-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="bc865-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bc865-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="bc865-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc865-201">String</span></span>|<span data-ttu-id="bc865-202">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="bc865-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="bc865-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="bc865-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-204">Boolean</span></span>|<span data-ttu-id="bc865-205">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="bc865-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="bc865-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-206">bitLockerEnabled</span></span>|<span data-ttu-id="bc865-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-207">Boolean</span></span>|<span data-ttu-id="bc865-208">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="bc865-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="bc865-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-209">secureBootEnabled</span></span>|<span data-ttu-id="bc865-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-210">Boolean</span></span>|<span data-ttu-id="bc865-211">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="bc865-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="bc865-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="bc865-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-213">Boolean</span></span>|<span data-ttu-id="bc865-214">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="bc865-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bc865-215">storageRequireEncryption</span></span>|<span data-ttu-id="bc865-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc865-216">Boolean</span></span>|<span data-ttu-id="bc865-217">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="bc865-218">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="bc865-218">activeFirewallRequired</span></span>|<span data-ttu-id="bc865-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-219">Boolean</span></span>|<span data-ttu-id="bc865-220">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="bc865-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-221">defenderEnabled</span></span>|<span data-ttu-id="bc865-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-222">Boolean</span></span>|<span data-ttu-id="bc865-223">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="bc865-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="bc865-224">defenderVersion</span></span>|<span data-ttu-id="bc865-225">String</span><span class="sxs-lookup"><span data-stu-id="bc865-225">String</span></span>|<span data-ttu-id="bc865-226">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="bc865-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="bc865-227">signatureOutOfDate</span></span>|<span data-ttu-id="bc865-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-228">Boolean</span></span>|<span data-ttu-id="bc865-229">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="bc865-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-230">rtpEnabled</span></span>|<span data-ttu-id="bc865-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-231">Boolean</span></span>|<span data-ttu-id="bc865-232">Requer a proteção em tempo real do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="bc865-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="bc865-233">antivirusRequired</span></span>|<span data-ttu-id="bc865-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-234">Boolean</span></span>|<span data-ttu-id="bc865-235">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="bc865-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="bc865-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="bc865-236">antiSpywareRequired</span></span>|<span data-ttu-id="bc865-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-237">Boolean</span></span>|<span data-ttu-id="bc865-238">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="bc865-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="bc865-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="bc865-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="bc865-240">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="bc865-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="bc865-241">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="bc865-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="bc865-242">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc865-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bc865-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bc865-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bc865-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-244">Boolean</span></span>|<span data-ttu-id="bc865-245">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="bc865-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="bc865-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bc865-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bc865-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bc865-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bc865-248">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="bc865-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bc865-249">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="bc865-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bc865-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="bc865-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="bc865-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc865-251">Boolean</span></span>|<span data-ttu-id="bc865-252">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="bc865-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="bc865-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc865-253">Response</span></span>
<span data-ttu-id="bc865-254">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc865-254">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc865-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc865-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc865-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc865-256">Request</span></span>
<span data-ttu-id="bc865-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc865-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

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
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="bc865-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc865-258">Response</span></span>
<span data-ttu-id="bc865-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc865-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

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
  "configurationManagerComplianceRequired": true
}
```




