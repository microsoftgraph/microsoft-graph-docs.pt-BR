---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ee738bc07ab0d246ecb5a61df244b08287a58d4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847800"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="7d7db-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7d7db-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="7d7db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d7db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d7db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d7db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d7db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d7db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d7db-107">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7d7db-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d7db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d7db-108">Prerequisites</span></span>
<span data-ttu-id="7d7db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d7db-111">Permission type</span></span>|<span data-ttu-id="7d7db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d7db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d7db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d7db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d7db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d7db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d7db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d7db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d7db-116">Not supported.</span></span>|
|<span data-ttu-id="7d7db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d7db-117">Application</span></span>|<span data-ttu-id="7d7db-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d7db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d7db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d7db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7d7db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7db-120">Request headers</span></span>
|<span data-ttu-id="7d7db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d7db-121">Header</span></span>|<span data-ttu-id="7d7db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7d7db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d7db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d7db-123">Authorization</span></span>|<span data-ttu-id="7d7db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d7db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d7db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d7db-125">Accept</span></span>|<span data-ttu-id="7d7db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d7db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7db-127">Request body</span></span>
<span data-ttu-id="7d7db-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7d7db-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="7d7db-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7d7db-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="7d7db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d7db-130">Property</span></span>|<span data-ttu-id="7d7db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d7db-131">Type</span></span>|<span data-ttu-id="7d7db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7db-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d7db-133">roleScopeTagIds</span></span>|<span data-ttu-id="7d7db-134">String collection</span><span class="sxs-lookup"><span data-stu-id="7d7db-134">String collection</span></span>|<span data-ttu-id="7d7db-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d7db-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d7db-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-137">id</span><span class="sxs-lookup"><span data-stu-id="7d7db-137">id</span></span>|<span data-ttu-id="7d7db-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-138">String</span></span>|<span data-ttu-id="7d7db-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d7db-139">Key of the entity.</span></span> <span data-ttu-id="7d7db-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7db-141">createdDateTime</span></span>|<span data-ttu-id="7d7db-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7db-142">DateTimeOffset</span></span>|<span data-ttu-id="7d7db-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7d7db-143">DateTime the object was created.</span></span> <span data-ttu-id="7d7db-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-145">description</span><span class="sxs-lookup"><span data-stu-id="7d7db-145">description</span></span>|<span data-ttu-id="7d7db-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-146">String</span></span>|<span data-ttu-id="7d7db-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7db-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d7db-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7db-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7d7db-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7db-150">DateTimeOffset</span></span>|<span data-ttu-id="7d7db-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7d7db-151">DateTime the object was last modified.</span></span> <span data-ttu-id="7d7db-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-153">displayName</span><span class="sxs-lookup"><span data-stu-id="7d7db-153">displayName</span></span>|<span data-ttu-id="7d7db-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-154">String</span></span>|<span data-ttu-id="7d7db-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7db-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d7db-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-157">version</span><span class="sxs-lookup"><span data-stu-id="7d7db-157">version</span></span>|<span data-ttu-id="7d7db-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7db-158">Int32</span></span>|<span data-ttu-id="7d7db-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7db-159">Version of the device configuration.</span></span> <span data-ttu-id="7d7db-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d7db-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7d7db-161">passwordRequired</span></span>|<span data-ttu-id="7d7db-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-162">Boolean</span></span>|<span data-ttu-id="7d7db-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="7d7db-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7d7db-164">passwordBlockSimple</span></span>|<span data-ttu-id="7d7db-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-165">Boolean</span></span>|<span data-ttu-id="7d7db-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7d7db-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="7d7db-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="7d7db-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="7d7db-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-168">Boolean</span></span>|<span data-ttu-id="7d7db-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="7d7db-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="7d7db-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7d7db-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7d7db-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7db-171">Int32</span></span>|<span data-ttu-id="7d7db-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="7d7db-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7d7db-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7d7db-173">passwordExpirationDays</span></span>|<span data-ttu-id="7d7db-174">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7db-174">Int32</span></span>|<span data-ttu-id="7d7db-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="7d7db-175">The password expiration in days.</span></span>|
|<span data-ttu-id="7d7db-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7d7db-176">passwordMinimumLength</span></span>|<span data-ttu-id="7d7db-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7db-177">Int32</span></span>|<span data-ttu-id="7d7db-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="7d7db-178">The minimum password length.</span></span>|
|<span data-ttu-id="7d7db-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7d7db-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7d7db-180">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7db-180">Int32</span></span>|<span data-ttu-id="7d7db-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="7d7db-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7d7db-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7d7db-182">passwordRequiredType</span></span>|[<span data-ttu-id="7d7db-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7d7db-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7d7db-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="7d7db-184">The required password type.</span></span> <span data-ttu-id="7d7db-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7d7db-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7d7db-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7d7db-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7d7db-187">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7db-187">Int32</span></span>|<span data-ttu-id="7d7db-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="7d7db-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="7d7db-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="7d7db-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="7d7db-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-190">Boolean</span></span>|<span data-ttu-id="7d7db-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7d7db-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7d7db-192">osMinimumVersion</span></span>|<span data-ttu-id="7d7db-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-193">String</span></span>|<span data-ttu-id="7d7db-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7d7db-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="7d7db-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7d7db-195">osMaximumVersion</span></span>|<span data-ttu-id="7d7db-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-196">String</span></span>|<span data-ttu-id="7d7db-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7d7db-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="7d7db-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7d7db-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="7d7db-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-199">String</span></span>|<span data-ttu-id="7d7db-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="7d7db-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7d7db-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7d7db-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="7d7db-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-202">String</span></span>|<span data-ttu-id="7d7db-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="7d7db-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7d7db-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="7d7db-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-205">Boolean</span></span>|<span data-ttu-id="7d7db-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="7d7db-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="7d7db-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-207">bitLockerEnabled</span></span>|<span data-ttu-id="7d7db-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-208">Boolean</span></span>|<span data-ttu-id="7d7db-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="7d7db-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="7d7db-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-210">secureBootEnabled</span></span>|<span data-ttu-id="7d7db-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-211">Boolean</span></span>|<span data-ttu-id="7d7db-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="7d7db-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="7d7db-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="7d7db-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-214">Boolean</span></span>|<span data-ttu-id="7d7db-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7d7db-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7d7db-216">storageRequireEncryption</span></span>|<span data-ttu-id="7d7db-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-217">Boolean</span></span>|<span data-ttu-id="7d7db-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="7d7db-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="7d7db-219">activeFirewallRequired</span></span>|<span data-ttu-id="7d7db-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-220">Boolean</span></span>|<span data-ttu-id="7d7db-221">Exigir um firewall ativas em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="7d7db-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-222">defenderEnabled</span></span>|<span data-ttu-id="7d7db-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-223">Boolean</span></span>|<span data-ttu-id="7d7db-224">Exigem o Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="7d7db-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="7d7db-225">defenderVersion</span></span>|<span data-ttu-id="7d7db-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7db-226">String</span></span>|<span data-ttu-id="7d7db-227">Exigem a versão mínima do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="7d7db-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="7d7db-228">signatureOutOfDate</span></span>|<span data-ttu-id="7d7db-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-229">Boolean</span></span>|<span data-ttu-id="7d7db-230">Exigem o Windows Defender Antimalware assinatura a ser atualizado em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="7d7db-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-231">rtpEnabled</span></span>|<span data-ttu-id="7d7db-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-232">Boolean</span></span>|<span data-ttu-id="7d7db-233">Exigem proteção em tempo real do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="7d7db-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="7d7db-234">antivirusRequired</span></span>|<span data-ttu-id="7d7db-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-235">Boolean</span></span>|<span data-ttu-id="7d7db-236">Exigir qualquer solução antivírus registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="7d7db-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="7d7db-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="7d7db-237">antiSpywareRequired</span></span>|<span data-ttu-id="7d7db-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-238">Boolean</span></span>|<span data-ttu-id="7d7db-239">Exigir qualquer solução de AntiSpyware registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="7d7db-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="7d7db-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="7d7db-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="7d7db-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="7d7db-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="7d7db-242">O sistema operacional válido criar intervalos em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="7d7db-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="7d7db-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7d7db-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7d7db-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7d7db-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="7d7db-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-245">Boolean</span></span>|<span data-ttu-id="7d7db-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="7d7db-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="7d7db-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7d7db-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7d7db-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="7d7db-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7d7db-249">Exigir o nível de risco mínimo de proteção contra ameaças de dispositivo a ser relatado não-conformidade.</span><span class="sxs-lookup"><span data-stu-id="7d7db-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7d7db-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7d7db-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7d7db-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="7d7db-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="7d7db-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d7db-252">Boolean</span></span>|<span data-ttu-id="7d7db-253">Exigem a considerar o estado de conformidade do SCCM em consideração para Intune estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="7d7db-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="7d7db-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7db-254">Response</span></span>
<span data-ttu-id="7d7db-255">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d7db-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7db-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d7db-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d7db-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7db-257">Request</span></span>
<span data-ttu-id="7d7db-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d7db-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d7db-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7db-259">Response</span></span>
<span data-ttu-id="7d7db-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d7db-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





