---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb83507aa28ec859939e846312539656d81b3f69
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165328"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="ce038-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ce038-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="ce038-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce038-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce038-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce038-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce038-106">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ce038-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce038-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce038-107">Prerequisites</span></span>
<span data-ttu-id="ce038-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce038-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce038-110">Permission type</span></span>|<span data-ttu-id="ce038-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce038-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce038-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce038-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce038-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce038-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce038-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce038-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce038-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce038-115">Not supported.</span></span>|
|<span data-ttu-id="ce038-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce038-116">Application</span></span>|<span data-ttu-id="ce038-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce038-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce038-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce038-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ce038-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce038-119">Request headers</span></span>
|<span data-ttu-id="ce038-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce038-120">Header</span></span>|<span data-ttu-id="ce038-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ce038-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce038-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce038-122">Authorization</span></span>|<span data-ttu-id="ce038-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce038-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce038-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce038-124">Accept</span></span>|<span data-ttu-id="ce038-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce038-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce038-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce038-126">Request body</span></span>
<span data-ttu-id="ce038-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="ce038-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="ce038-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="ce038-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="ce038-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce038-129">Property</span></span>|<span data-ttu-id="ce038-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce038-130">Type</span></span>|<span data-ttu-id="ce038-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce038-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce038-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce038-132">roleScopeTagIds</span></span>|<span data-ttu-id="ce038-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce038-133">String collection</span></span>|<span data-ttu-id="ce038-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ce038-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce038-135">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-136">id</span><span class="sxs-lookup"><span data-stu-id="ce038-136">id</span></span>|<span data-ttu-id="ce038-137">String</span><span class="sxs-lookup"><span data-stu-id="ce038-137">String</span></span>|<span data-ttu-id="ce038-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce038-138">Key of the entity.</span></span> <span data-ttu-id="ce038-139">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce038-140">createdDateTime</span></span>|<span data-ttu-id="ce038-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce038-141">DateTimeOffset</span></span>|<span data-ttu-id="ce038-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ce038-142">DateTime the object was created.</span></span> <span data-ttu-id="ce038-143">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-144">description</span><span class="sxs-lookup"><span data-stu-id="ce038-144">description</span></span>|<span data-ttu-id="ce038-145">String</span><span class="sxs-lookup"><span data-stu-id="ce038-145">String</span></span>|<span data-ttu-id="ce038-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce038-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce038-147">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce038-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ce038-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce038-149">DateTimeOffset</span></span>|<span data-ttu-id="ce038-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ce038-150">DateTime the object was last modified.</span></span> <span data-ttu-id="ce038-151">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ce038-152">displayName</span></span>|<span data-ttu-id="ce038-153">String</span><span class="sxs-lookup"><span data-stu-id="ce038-153">String</span></span>|<span data-ttu-id="ce038-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce038-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce038-155">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-156">version</span><span class="sxs-lookup"><span data-stu-id="ce038-156">version</span></span>|<span data-ttu-id="ce038-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ce038-157">Int32</span></span>|<span data-ttu-id="ce038-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce038-158">Version of the device configuration.</span></span> <span data-ttu-id="ce038-159">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ce038-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ce038-160">passwordRequired</span></span>|<span data-ttu-id="ce038-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-161">Boolean</span></span>|<span data-ttu-id="ce038-162">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="ce038-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ce038-163">passwordBlockSimple</span></span>|<span data-ttu-id="ce038-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce038-164">Boolean</span></span>|<span data-ttu-id="ce038-165">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ce038-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="ce038-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="ce038-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="ce038-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-167">Boolean</span></span>|<span data-ttu-id="ce038-168">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="ce038-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="ce038-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ce038-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ce038-170">Int32</span><span class="sxs-lookup"><span data-stu-id="ce038-170">Int32</span></span>|<span data-ttu-id="ce038-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="ce038-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ce038-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ce038-172">passwordExpirationDays</span></span>|<span data-ttu-id="ce038-173">Int32</span><span class="sxs-lookup"><span data-stu-id="ce038-173">Int32</span></span>|<span data-ttu-id="ce038-174">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="ce038-174">The password expiration in days.</span></span>|
|<span data-ttu-id="ce038-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ce038-175">passwordMinimumLength</span></span>|<span data-ttu-id="ce038-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ce038-176">Int32</span></span>|<span data-ttu-id="ce038-177">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="ce038-177">The minimum password length.</span></span>|
|<span data-ttu-id="ce038-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ce038-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ce038-179">Int32</span><span class="sxs-lookup"><span data-stu-id="ce038-179">Int32</span></span>|<span data-ttu-id="ce038-180">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="ce038-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ce038-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ce038-181">passwordRequiredType</span></span>|[<span data-ttu-id="ce038-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ce038-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ce038-183">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="ce038-183">The required password type.</span></span> <span data-ttu-id="ce038-184">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ce038-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ce038-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ce038-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ce038-186">Int32</span><span class="sxs-lookup"><span data-stu-id="ce038-186">Int32</span></span>|<span data-ttu-id="ce038-187">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="ce038-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="ce038-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="ce038-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="ce038-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-189">Boolean</span></span>|<span data-ttu-id="ce038-190">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="ce038-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ce038-191">osMinimumVersion</span></span>|<span data-ttu-id="ce038-192">String</span><span class="sxs-lookup"><span data-stu-id="ce038-192">String</span></span>|<span data-ttu-id="ce038-193">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ce038-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="ce038-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ce038-194">osMaximumVersion</span></span>|<span data-ttu-id="ce038-195">String</span><span class="sxs-lookup"><span data-stu-id="ce038-195">String</span></span>|<span data-ttu-id="ce038-196">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ce038-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="ce038-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ce038-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="ce038-198">String</span><span class="sxs-lookup"><span data-stu-id="ce038-198">String</span></span>|<span data-ttu-id="ce038-199">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="ce038-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="ce038-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ce038-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="ce038-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce038-201">String</span></span>|<span data-ttu-id="ce038-202">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="ce038-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="ce038-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="ce038-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-204">Boolean</span></span>|<span data-ttu-id="ce038-205">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="ce038-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="ce038-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-206">bitLockerEnabled</span></span>|<span data-ttu-id="ce038-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-207">Boolean</span></span>|<span data-ttu-id="ce038-208">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce038-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="ce038-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-209">secureBootEnabled</span></span>|<span data-ttu-id="ce038-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-210">Boolean</span></span>|<span data-ttu-id="ce038-211">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="ce038-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="ce038-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="ce038-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-213">Boolean</span></span>|<span data-ttu-id="ce038-214">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="ce038-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ce038-215">storageRequireEncryption</span></span>|<span data-ttu-id="ce038-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce038-216">Boolean</span></span>|<span data-ttu-id="ce038-217">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="ce038-218">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="ce038-218">activeFirewallRequired</span></span>|<span data-ttu-id="ce038-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-219">Boolean</span></span>|<span data-ttu-id="ce038-220">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="ce038-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-221">defenderEnabled</span></span>|<span data-ttu-id="ce038-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-222">Boolean</span></span>|<span data-ttu-id="ce038-223">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="ce038-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="ce038-224">defenderVersion</span></span>|<span data-ttu-id="ce038-225">String</span><span class="sxs-lookup"><span data-stu-id="ce038-225">String</span></span>|<span data-ttu-id="ce038-226">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="ce038-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="ce038-227">signatureOutOfDate</span></span>|<span data-ttu-id="ce038-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-228">Boolean</span></span>|<span data-ttu-id="ce038-229">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="ce038-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-230">rtpEnabled</span></span>|<span data-ttu-id="ce038-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-231">Boolean</span></span>|<span data-ttu-id="ce038-232">Requer a proteção em tempo real do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="ce038-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="ce038-233">antivirusRequired</span></span>|<span data-ttu-id="ce038-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-234">Boolean</span></span>|<span data-ttu-id="ce038-235">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="ce038-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="ce038-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="ce038-236">antiSpywareRequired</span></span>|<span data-ttu-id="ce038-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-237">Boolean</span></span>|<span data-ttu-id="ce038-238">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="ce038-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="ce038-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="ce038-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="ce038-240">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="ce038-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="ce038-241">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="ce038-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="ce038-242">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ce038-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ce038-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ce038-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ce038-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-244">Boolean</span></span>|<span data-ttu-id="ce038-245">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="ce038-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ce038-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ce038-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ce038-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ce038-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ce038-248">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="ce038-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ce038-249">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ce038-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ce038-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="ce038-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="ce038-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce038-251">Boolean</span></span>|<span data-ttu-id="ce038-252">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="ce038-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="ce038-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce038-253">Response</span></span>
<span data-ttu-id="ce038-254">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce038-254">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce038-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce038-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce038-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce038-256">Request</span></span>
<span data-ttu-id="ce038-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce038-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="ce038-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce038-258">Response</span></span>
<span data-ttu-id="ce038-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce038-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




