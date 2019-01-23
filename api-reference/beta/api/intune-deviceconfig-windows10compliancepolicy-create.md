---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2eba67635ea4e596dd9bf1881b5b5c0d7b9743df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422737"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="aad55-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="aad55-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="aad55-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="aad55-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aad55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aad55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aad55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="aad55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aad55-107">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aad55-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aad55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aad55-108">Prerequisites</span></span>
<span data-ttu-id="aad55-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aad55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aad55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aad55-111">Permission type</span></span>|<span data-ttu-id="aad55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aad55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aad55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aad55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aad55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aad55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aad55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aad55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aad55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aad55-116">Not supported.</span></span>|
|<span data-ttu-id="aad55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aad55-117">Application</span></span>|<span data-ttu-id="aad55-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aad55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aad55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aad55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="aad55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aad55-120">Request headers</span></span>
|<span data-ttu-id="aad55-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aad55-121">Header</span></span>|<span data-ttu-id="aad55-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aad55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aad55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aad55-123">Authorization</span></span>|<span data-ttu-id="aad55-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aad55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aad55-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aad55-125">Accept</span></span>|<span data-ttu-id="aad55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aad55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aad55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aad55-127">Request body</span></span>
<span data-ttu-id="aad55-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="aad55-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="aad55-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="aad55-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="aad55-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aad55-130">Property</span></span>|<span data-ttu-id="aad55-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aad55-131">Type</span></span>|<span data-ttu-id="aad55-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aad55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aad55-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aad55-133">roleScopeTagIds</span></span>|<span data-ttu-id="aad55-134">String collection</span><span class="sxs-lookup"><span data-stu-id="aad55-134">String collection</span></span>|<span data-ttu-id="aad55-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="aad55-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aad55-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-137">id</span><span class="sxs-lookup"><span data-stu-id="aad55-137">id</span></span>|<span data-ttu-id="aad55-138">String</span><span class="sxs-lookup"><span data-stu-id="aad55-138">String</span></span>|<span data-ttu-id="aad55-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aad55-139">Key of the entity.</span></span> <span data-ttu-id="aad55-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aad55-141">createdDateTime</span></span>|<span data-ttu-id="aad55-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad55-142">DateTimeOffset</span></span>|<span data-ttu-id="aad55-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aad55-143">DateTime the object was created.</span></span> <span data-ttu-id="aad55-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-145">description</span><span class="sxs-lookup"><span data-stu-id="aad55-145">description</span></span>|<span data-ttu-id="aad55-146">String</span><span class="sxs-lookup"><span data-stu-id="aad55-146">String</span></span>|<span data-ttu-id="aad55-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aad55-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aad55-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aad55-149">lastModifiedDateTime</span></span>|<span data-ttu-id="aad55-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aad55-150">DateTimeOffset</span></span>|<span data-ttu-id="aad55-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aad55-151">DateTime the object was last modified.</span></span> <span data-ttu-id="aad55-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-153">displayName</span><span class="sxs-lookup"><span data-stu-id="aad55-153">displayName</span></span>|<span data-ttu-id="aad55-154">String</span><span class="sxs-lookup"><span data-stu-id="aad55-154">String</span></span>|<span data-ttu-id="aad55-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aad55-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aad55-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-157">version</span><span class="sxs-lookup"><span data-stu-id="aad55-157">version</span></span>|<span data-ttu-id="aad55-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aad55-158">Int32</span></span>|<span data-ttu-id="aad55-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aad55-159">Version of the device configuration.</span></span> <span data-ttu-id="aad55-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aad55-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aad55-161">passwordRequired</span></span>|<span data-ttu-id="aad55-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="aad55-162">Boolean</span></span>|<span data-ttu-id="aad55-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="aad55-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="aad55-164">passwordBlockSimple</span></span>|<span data-ttu-id="aad55-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="aad55-165">Boolean</span></span>|<span data-ttu-id="aad55-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="aad55-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="aad55-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="aad55-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="aad55-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="aad55-168">Boolean</span></span>|<span data-ttu-id="aad55-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="aad55-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="aad55-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="aad55-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="aad55-171">Int32</span><span class="sxs-lookup"><span data-stu-id="aad55-171">Int32</span></span>|<span data-ttu-id="aad55-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="aad55-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="aad55-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aad55-173">passwordExpirationDays</span></span>|<span data-ttu-id="aad55-174">Int32</span><span class="sxs-lookup"><span data-stu-id="aad55-174">Int32</span></span>|<span data-ttu-id="aad55-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="aad55-175">The password expiration in days.</span></span>|
|<span data-ttu-id="aad55-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aad55-176">passwordMinimumLength</span></span>|<span data-ttu-id="aad55-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aad55-177">Int32</span></span>|<span data-ttu-id="aad55-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="aad55-178">The minimum password length.</span></span>|
|<span data-ttu-id="aad55-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="aad55-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="aad55-180">Int32</span><span class="sxs-lookup"><span data-stu-id="aad55-180">Int32</span></span>|<span data-ttu-id="aad55-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="aad55-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="aad55-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aad55-182">passwordRequiredType</span></span>|[<span data-ttu-id="aad55-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aad55-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="aad55-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="aad55-184">The required password type.</span></span> <span data-ttu-id="aad55-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="aad55-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="aad55-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aad55-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aad55-187">Int32</span><span class="sxs-lookup"><span data-stu-id="aad55-187">Int32</span></span>|<span data-ttu-id="aad55-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="aad55-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="aad55-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="aad55-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="aad55-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="aad55-190">Boolean</span></span>|<span data-ttu-id="aad55-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="aad55-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aad55-192">osMinimumVersion</span></span>|<span data-ttu-id="aad55-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad55-193">String</span></span>|<span data-ttu-id="aad55-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aad55-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="aad55-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aad55-195">osMaximumVersion</span></span>|<span data-ttu-id="aad55-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad55-196">String</span></span>|<span data-ttu-id="aad55-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aad55-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="aad55-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aad55-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="aad55-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad55-199">String</span></span>|<span data-ttu-id="aad55-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aad55-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="aad55-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aad55-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="aad55-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aad55-202">String</span></span>|<span data-ttu-id="aad55-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aad55-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="aad55-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="aad55-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-205">Boolean</span></span>|<span data-ttu-id="aad55-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="aad55-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="aad55-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-207">bitLockerEnabled</span></span>|<span data-ttu-id="aad55-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-208">Boolean</span></span>|<span data-ttu-id="aad55-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="aad55-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="aad55-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-210">secureBootEnabled</span></span>|<span data-ttu-id="aad55-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-211">Boolean</span></span>|<span data-ttu-id="aad55-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="aad55-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="aad55-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="aad55-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-214">Boolean</span></span>|<span data-ttu-id="aad55-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="aad55-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="aad55-216">storageRequireEncryption</span></span>|<span data-ttu-id="aad55-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-217">Boolean</span></span>|<span data-ttu-id="aad55-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="aad55-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="aad55-219">activeFirewallRequired</span></span>|<span data-ttu-id="aad55-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-220">Boolean</span></span>|<span data-ttu-id="aad55-221">Exigir um firewall ativas em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="aad55-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-222">defenderEnabled</span></span>|<span data-ttu-id="aad55-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-223">Boolean</span></span>|<span data-ttu-id="aad55-224">Exigem o Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="aad55-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="aad55-225">defenderVersion</span></span>|<span data-ttu-id="aad55-226">String</span><span class="sxs-lookup"><span data-stu-id="aad55-226">String</span></span>|<span data-ttu-id="aad55-227">Exigem a versão mínima do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="aad55-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="aad55-228">signatureOutOfDate</span></span>|<span data-ttu-id="aad55-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-229">Boolean</span></span>|<span data-ttu-id="aad55-230">Exigem o Windows Defender Antimalware assinatura a ser atualizado em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="aad55-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-231">rtpEnabled</span></span>|<span data-ttu-id="aad55-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-232">Boolean</span></span>|<span data-ttu-id="aad55-233">Exigem proteção em tempo real do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="aad55-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="aad55-234">antivirusRequired</span></span>|<span data-ttu-id="aad55-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-235">Boolean</span></span>|<span data-ttu-id="aad55-236">Exigir qualquer solução antivírus registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="aad55-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="aad55-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="aad55-237">antiSpywareRequired</span></span>|<span data-ttu-id="aad55-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-238">Boolean</span></span>|<span data-ttu-id="aad55-239">Exigir qualquer solução de AntiSpyware registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="aad55-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="aad55-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="aad55-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="aad55-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="aad55-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="aad55-242">O sistema operacional válido criar intervalos em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="aad55-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="aad55-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="aad55-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="aad55-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="aad55-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="aad55-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-245">Boolean</span></span>|<span data-ttu-id="aad55-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="aad55-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="aad55-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="aad55-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="aad55-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="aad55-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="aad55-249">Exigir o nível de risco mínimo de proteção contra ameaças de dispositivo a ser relatado não-conformidade.</span><span class="sxs-lookup"><span data-stu-id="aad55-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="aad55-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="aad55-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="aad55-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="aad55-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="aad55-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="aad55-252">Boolean</span></span>|<span data-ttu-id="aad55-253">Exigem a considerar o estado de conformidade do SCCM em consideração para Intune estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="aad55-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="aad55-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="aad55-254">Response</span></span>
<span data-ttu-id="aad55-255">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aad55-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aad55-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aad55-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="aad55-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aad55-257">Request</span></span>
<span data-ttu-id="aad55-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aad55-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aad55-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="aad55-259">Response</span></span>
<span data-ttu-id="aad55-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aad55-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




