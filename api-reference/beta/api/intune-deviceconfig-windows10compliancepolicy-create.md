---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e69151a5f0b7a0bc8c0558fc9f178714e7520d1c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792636"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="95797-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="95797-103">Create windows10CompliancePolicy</span></span>

<span data-ttu-id="95797-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95797-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95797-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95797-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95797-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95797-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95797-107">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95797-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95797-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95797-108">Prerequisites</span></span>
<span data-ttu-id="95797-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="95797-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="95797-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95797-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95797-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95797-111">Permission type</span></span>|<span data-ttu-id="95797-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95797-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95797-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95797-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95797-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95797-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95797-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95797-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95797-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95797-116">Not supported.</span></span>|
|<span data-ttu-id="95797-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95797-117">Application</span></span>|<span data-ttu-id="95797-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95797-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95797-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95797-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="95797-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95797-120">Request headers</span></span>
|<span data-ttu-id="95797-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95797-121">Header</span></span>|<span data-ttu-id="95797-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95797-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95797-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95797-123">Authorization</span></span>|<span data-ttu-id="95797-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95797-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95797-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95797-125">Accept</span></span>|<span data-ttu-id="95797-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95797-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95797-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95797-127">Request body</span></span>
<span data-ttu-id="95797-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="95797-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="95797-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="95797-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="95797-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95797-130">Property</span></span>|<span data-ttu-id="95797-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="95797-131">Type</span></span>|<span data-ttu-id="95797-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="95797-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95797-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95797-133">roleScopeTagIds</span></span>|<span data-ttu-id="95797-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="95797-134">String collection</span></span>|<span data-ttu-id="95797-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="95797-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95797-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-137">id</span><span class="sxs-lookup"><span data-stu-id="95797-137">id</span></span>|<span data-ttu-id="95797-138">String</span><span class="sxs-lookup"><span data-stu-id="95797-138">String</span></span>|<span data-ttu-id="95797-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95797-139">Key of the entity.</span></span> <span data-ttu-id="95797-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95797-141">createdDateTime</span></span>|<span data-ttu-id="95797-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95797-142">DateTimeOffset</span></span>|<span data-ttu-id="95797-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="95797-143">DateTime the object was created.</span></span> <span data-ttu-id="95797-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-145">description</span><span class="sxs-lookup"><span data-stu-id="95797-145">description</span></span>|<span data-ttu-id="95797-146">String</span><span class="sxs-lookup"><span data-stu-id="95797-146">String</span></span>|<span data-ttu-id="95797-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95797-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95797-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95797-149">lastModifiedDateTime</span></span>|<span data-ttu-id="95797-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95797-150">DateTimeOffset</span></span>|<span data-ttu-id="95797-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="95797-151">DateTime the object was last modified.</span></span> <span data-ttu-id="95797-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-153">displayName</span><span class="sxs-lookup"><span data-stu-id="95797-153">displayName</span></span>|<span data-ttu-id="95797-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95797-154">String</span></span>|<span data-ttu-id="95797-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95797-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95797-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-157">version</span><span class="sxs-lookup"><span data-stu-id="95797-157">version</span></span>|<span data-ttu-id="95797-158">Int32</span><span class="sxs-lookup"><span data-stu-id="95797-158">Int32</span></span>|<span data-ttu-id="95797-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95797-159">Version of the device configuration.</span></span> <span data-ttu-id="95797-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95797-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95797-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="95797-161">passwordRequired</span></span>|<span data-ttu-id="95797-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-162">Boolean</span></span>|<span data-ttu-id="95797-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="95797-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="95797-164">passwordBlockSimple</span></span>|<span data-ttu-id="95797-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-165">Boolean</span></span>|<span data-ttu-id="95797-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="95797-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="95797-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="95797-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="95797-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-168">Boolean</span></span>|<span data-ttu-id="95797-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="95797-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="95797-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="95797-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="95797-171">Int32</span><span class="sxs-lookup"><span data-stu-id="95797-171">Int32</span></span>|<span data-ttu-id="95797-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="95797-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="95797-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="95797-173">passwordExpirationDays</span></span>|<span data-ttu-id="95797-174">Int32</span><span class="sxs-lookup"><span data-stu-id="95797-174">Int32</span></span>|<span data-ttu-id="95797-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="95797-175">The password expiration in days.</span></span>|
|<span data-ttu-id="95797-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="95797-176">passwordMinimumLength</span></span>|<span data-ttu-id="95797-177">Int32</span><span class="sxs-lookup"><span data-stu-id="95797-177">Int32</span></span>|<span data-ttu-id="95797-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="95797-178">The minimum password length.</span></span>|
|<span data-ttu-id="95797-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="95797-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="95797-180">Int32</span><span class="sxs-lookup"><span data-stu-id="95797-180">Int32</span></span>|<span data-ttu-id="95797-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="95797-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="95797-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="95797-182">passwordRequiredType</span></span>|[<span data-ttu-id="95797-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="95797-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="95797-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="95797-184">The required password type.</span></span> <span data-ttu-id="95797-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="95797-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="95797-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="95797-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="95797-187">Int32</span><span class="sxs-lookup"><span data-stu-id="95797-187">Int32</span></span>|<span data-ttu-id="95797-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="95797-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="95797-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="95797-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="95797-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-190">Boolean</span></span>|<span data-ttu-id="95797-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="95797-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="95797-192">osMinimumVersion</span></span>|<span data-ttu-id="95797-193">String</span><span class="sxs-lookup"><span data-stu-id="95797-193">String</span></span>|<span data-ttu-id="95797-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="95797-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="95797-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="95797-195">osMaximumVersion</span></span>|<span data-ttu-id="95797-196">String</span><span class="sxs-lookup"><span data-stu-id="95797-196">String</span></span>|<span data-ttu-id="95797-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="95797-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="95797-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="95797-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="95797-199">String</span><span class="sxs-lookup"><span data-stu-id="95797-199">String</span></span>|<span data-ttu-id="95797-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="95797-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="95797-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="95797-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="95797-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95797-202">String</span></span>|<span data-ttu-id="95797-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="95797-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="95797-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="95797-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-205">Boolean</span></span>|<span data-ttu-id="95797-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="95797-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="95797-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-207">bitLockerEnabled</span></span>|<span data-ttu-id="95797-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-208">Boolean</span></span>|<span data-ttu-id="95797-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="95797-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="95797-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-210">secureBootEnabled</span></span>|<span data-ttu-id="95797-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-211">Boolean</span></span>|<span data-ttu-id="95797-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="95797-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="95797-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="95797-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-214">Boolean</span></span>|<span data-ttu-id="95797-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="95797-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="95797-216">storageRequireEncryption</span></span>|<span data-ttu-id="95797-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-217">Boolean</span></span>|<span data-ttu-id="95797-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="95797-219">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="95797-219">activeFirewallRequired</span></span>|<span data-ttu-id="95797-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-220">Boolean</span></span>|<span data-ttu-id="95797-221">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="95797-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-222">defenderEnabled</span></span>|<span data-ttu-id="95797-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-223">Boolean</span></span>|<span data-ttu-id="95797-224">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="95797-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="95797-225">defenderVersion</span></span>|<span data-ttu-id="95797-226">String</span><span class="sxs-lookup"><span data-stu-id="95797-226">String</span></span>|<span data-ttu-id="95797-227">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="95797-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="95797-228">signatureOutOfDate</span></span>|<span data-ttu-id="95797-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-229">Boolean</span></span>|<span data-ttu-id="95797-230">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="95797-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-231">rtpEnabled</span></span>|<span data-ttu-id="95797-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-232">Boolean</span></span>|<span data-ttu-id="95797-233">Requer a proteção em tempo real do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="95797-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="95797-234">antivirusRequired</span></span>|<span data-ttu-id="95797-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-235">Boolean</span></span>|<span data-ttu-id="95797-236">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="95797-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="95797-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="95797-237">antiSpywareRequired</span></span>|<span data-ttu-id="95797-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-238">Boolean</span></span>|<span data-ttu-id="95797-239">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="95797-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="95797-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="95797-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="95797-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="95797-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="95797-242">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="95797-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="95797-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="95797-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="95797-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="95797-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="95797-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-245">Boolean</span></span>|<span data-ttu-id="95797-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="95797-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="95797-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95797-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="95797-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="95797-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="95797-249">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="95797-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="95797-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="95797-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="95797-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="95797-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="95797-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-252">Boolean</span></span>|<span data-ttu-id="95797-253">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="95797-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="95797-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="95797-254">tpmRequired</span></span>|<span data-ttu-id="95797-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="95797-255">Boolean</span></span>|<span data-ttu-id="95797-256">Requer o módulo de plataforma confiável (TPM) para estar presente.</span><span class="sxs-lookup"><span data-stu-id="95797-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="95797-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="95797-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="95797-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="95797-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="95797-259">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="95797-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="95797-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="95797-260">Response</span></span>
<span data-ttu-id="95797-261">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95797-261">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95797-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95797-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="95797-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95797-263">Request</span></span>
<span data-ttu-id="95797-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95797-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1911

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
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="95797-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="95797-265">Response</span></span>
<span data-ttu-id="95797-266">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="95797-266">Here is an example of the response.</span></span> <span data-ttu-id="95797-267">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="95797-267">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="95797-268">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="95797-268">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2083

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
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```



