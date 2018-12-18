---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 50d1230a6e1580008e501745f9c7918da5031187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360911"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="5187e-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5187e-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="5187e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5187e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5187e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5187e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5187e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5187e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5187e-107">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5187e-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5187e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5187e-108">Prerequisites</span></span>
<span data-ttu-id="5187e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5187e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5187e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5187e-111">Permission type</span></span>|<span data-ttu-id="5187e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5187e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5187e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5187e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5187e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5187e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5187e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5187e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5187e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5187e-116">Not supported.</span></span>|
|<span data-ttu-id="5187e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5187e-117">Application</span></span>|<span data-ttu-id="5187e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5187e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5187e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5187e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5187e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5187e-120">Request headers</span></span>
|<span data-ttu-id="5187e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5187e-121">Header</span></span>|<span data-ttu-id="5187e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5187e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5187e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5187e-123">Authorization</span></span>|<span data-ttu-id="5187e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5187e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5187e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5187e-125">Accept</span></span>|<span data-ttu-id="5187e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5187e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5187e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5187e-127">Request body</span></span>
<span data-ttu-id="5187e-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5187e-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="5187e-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5187e-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="5187e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5187e-130">Property</span></span>|<span data-ttu-id="5187e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5187e-131">Type</span></span>|<span data-ttu-id="5187e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5187e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5187e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5187e-133">roleScopeTagIds</span></span>|<span data-ttu-id="5187e-134">String collection</span><span class="sxs-lookup"><span data-stu-id="5187e-134">String collection</span></span>|<span data-ttu-id="5187e-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="5187e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5187e-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-137">id</span><span class="sxs-lookup"><span data-stu-id="5187e-137">id</span></span>|<span data-ttu-id="5187e-138">String</span><span class="sxs-lookup"><span data-stu-id="5187e-138">String</span></span>|<span data-ttu-id="5187e-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5187e-139">Key of the entity.</span></span> <span data-ttu-id="5187e-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5187e-141">createdDateTime</span></span>|<span data-ttu-id="5187e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5187e-142">DateTimeOffset</span></span>|<span data-ttu-id="5187e-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5187e-143">DateTime the object was created.</span></span> <span data-ttu-id="5187e-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-145">description</span><span class="sxs-lookup"><span data-stu-id="5187e-145">description</span></span>|<span data-ttu-id="5187e-146">String</span><span class="sxs-lookup"><span data-stu-id="5187e-146">String</span></span>|<span data-ttu-id="5187e-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5187e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5187e-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5187e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="5187e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5187e-150">DateTimeOffset</span></span>|<span data-ttu-id="5187e-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5187e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="5187e-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="5187e-153">displayName</span></span>|<span data-ttu-id="5187e-154">String</span><span class="sxs-lookup"><span data-stu-id="5187e-154">String</span></span>|<span data-ttu-id="5187e-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5187e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5187e-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-157">version</span><span class="sxs-lookup"><span data-stu-id="5187e-157">version</span></span>|<span data-ttu-id="5187e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5187e-158">Int32</span></span>|<span data-ttu-id="5187e-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5187e-159">Version of the device configuration.</span></span> <span data-ttu-id="5187e-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5187e-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5187e-161">passwordRequired</span></span>|<span data-ttu-id="5187e-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="5187e-162">Boolean</span></span>|<span data-ttu-id="5187e-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="5187e-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5187e-164">passwordBlockSimple</span></span>|<span data-ttu-id="5187e-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="5187e-165">Boolean</span></span>|<span data-ttu-id="5187e-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="5187e-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="5187e-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="5187e-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="5187e-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="5187e-168">Boolean</span></span>|<span data-ttu-id="5187e-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="5187e-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="5187e-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5187e-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5187e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5187e-171">Int32</span></span>|<span data-ttu-id="5187e-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="5187e-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5187e-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5187e-173">passwordExpirationDays</span></span>|<span data-ttu-id="5187e-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5187e-174">Int32</span></span>|<span data-ttu-id="5187e-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="5187e-175">The password expiration in days.</span></span>|
|<span data-ttu-id="5187e-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5187e-176">passwordMinimumLength</span></span>|<span data-ttu-id="5187e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5187e-177">Int32</span></span>|<span data-ttu-id="5187e-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="5187e-178">The minimum password length.</span></span>|
|<span data-ttu-id="5187e-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5187e-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5187e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="5187e-180">Int32</span></span>|<span data-ttu-id="5187e-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="5187e-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5187e-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5187e-182">passwordRequiredType</span></span>|[<span data-ttu-id="5187e-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5187e-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5187e-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="5187e-184">The required password type.</span></span> <span data-ttu-id="5187e-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5187e-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5187e-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5187e-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5187e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="5187e-187">Int32</span></span>|<span data-ttu-id="5187e-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="5187e-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="5187e-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="5187e-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="5187e-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="5187e-190">Boolean</span></span>|<span data-ttu-id="5187e-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5187e-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5187e-192">osMinimumVersion</span></span>|<span data-ttu-id="5187e-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5187e-193">String</span></span>|<span data-ttu-id="5187e-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5187e-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="5187e-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5187e-195">osMaximumVersion</span></span>|<span data-ttu-id="5187e-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5187e-196">String</span></span>|<span data-ttu-id="5187e-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5187e-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="5187e-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5187e-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="5187e-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5187e-199">String</span></span>|<span data-ttu-id="5187e-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="5187e-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="5187e-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5187e-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="5187e-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5187e-202">String</span></span>|<span data-ttu-id="5187e-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="5187e-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="5187e-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="5187e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-205">Boolean</span></span>|<span data-ttu-id="5187e-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="5187e-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="5187e-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-207">bitLockerEnabled</span></span>|<span data-ttu-id="5187e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-208">Boolean</span></span>|<span data-ttu-id="5187e-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="5187e-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="5187e-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-210">secureBootEnabled</span></span>|<span data-ttu-id="5187e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-211">Boolean</span></span>|<span data-ttu-id="5187e-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="5187e-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="5187e-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="5187e-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-214">Boolean</span></span>|<span data-ttu-id="5187e-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5187e-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5187e-216">storageRequireEncryption</span></span>|<span data-ttu-id="5187e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-217">Boolean</span></span>|<span data-ttu-id="5187e-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="5187e-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="5187e-219">activeFirewallRequired</span></span>|<span data-ttu-id="5187e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-220">Boolean</span></span>|<span data-ttu-id="5187e-221">Exigir um firewall ativas em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="5187e-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-222">defenderEnabled</span></span>|<span data-ttu-id="5187e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-223">Boolean</span></span>|<span data-ttu-id="5187e-224">Exigem o Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="5187e-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="5187e-225">defenderVersion</span></span>|<span data-ttu-id="5187e-226">String</span><span class="sxs-lookup"><span data-stu-id="5187e-226">String</span></span>|<span data-ttu-id="5187e-227">Exigem a versão mínima do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="5187e-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="5187e-228">signatureOutOfDate</span></span>|<span data-ttu-id="5187e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-229">Boolean</span></span>|<span data-ttu-id="5187e-230">Exigem o Windows Defender Antimalware assinatura a ser atualizado em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="5187e-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-231">rtpEnabled</span></span>|<span data-ttu-id="5187e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-232">Boolean</span></span>|<span data-ttu-id="5187e-233">Exigem proteção em tempo real do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="5187e-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="5187e-234">antivirusRequired</span></span>|<span data-ttu-id="5187e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-235">Boolean</span></span>|<span data-ttu-id="5187e-236">Exigir qualquer solução antivírus registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="5187e-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="5187e-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="5187e-237">antiSpywareRequired</span></span>|<span data-ttu-id="5187e-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-238">Boolean</span></span>|<span data-ttu-id="5187e-239">Exigir qualquer solução de AntiSpyware registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="5187e-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="5187e-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="5187e-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="5187e-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="5187e-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="5187e-242">O sistema operacional válido criar intervalos em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="5187e-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="5187e-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="5187e-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="5187e-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5187e-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5187e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-245">Boolean</span></span>|<span data-ttu-id="5187e-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="5187e-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5187e-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5187e-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5187e-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="5187e-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5187e-249">Exigir o nível de risco mínimo de proteção contra ameaças de dispositivo a ser relatado não-conformidade.</span><span class="sxs-lookup"><span data-stu-id="5187e-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5187e-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5187e-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5187e-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="5187e-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="5187e-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="5187e-252">Boolean</span></span>|<span data-ttu-id="5187e-253">Exigem a considerar o estado de conformidade do SCCM em consideração para Intune estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="5187e-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="5187e-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="5187e-254">Response</span></span>
<span data-ttu-id="5187e-255">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5187e-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5187e-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5187e-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="5187e-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5187e-257">Request</span></span>
<span data-ttu-id="5187e-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5187e-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1730

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="5187e-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="5187e-259">Response</span></span>
<span data-ttu-id="5187e-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5187e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





