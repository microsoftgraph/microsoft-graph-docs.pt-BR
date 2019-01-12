---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5d09c30c9219ea3a9d927b6d550f98130a38ecbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950141"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="53bbc-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="53bbc-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="53bbc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53bbc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53bbc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53bbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53bbc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53bbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53bbc-107">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="53bbc-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53bbc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53bbc-108">Prerequisites</span></span>
<span data-ttu-id="53bbc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53bbc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53bbc-111">Permission type</span></span>|<span data-ttu-id="53bbc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53bbc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53bbc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53bbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53bbc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53bbc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53bbc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53bbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53bbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53bbc-116">Not supported.</span></span>|
|<span data-ttu-id="53bbc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53bbc-117">Application</span></span>|<span data-ttu-id="53bbc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53bbc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53bbc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53bbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="53bbc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53bbc-120">Request headers</span></span>
|<span data-ttu-id="53bbc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53bbc-121">Header</span></span>|<span data-ttu-id="53bbc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53bbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53bbc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53bbc-123">Authorization</span></span>|<span data-ttu-id="53bbc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53bbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53bbc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53bbc-125">Accept</span></span>|<span data-ttu-id="53bbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53bbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53bbc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53bbc-127">Request body</span></span>
<span data-ttu-id="53bbc-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="53bbc-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="53bbc-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="53bbc-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="53bbc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53bbc-130">Property</span></span>|<span data-ttu-id="53bbc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53bbc-131">Type</span></span>|<span data-ttu-id="53bbc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53bbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bbc-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53bbc-133">roleScopeTagIds</span></span>|<span data-ttu-id="53bbc-134">String collection</span><span class="sxs-lookup"><span data-stu-id="53bbc-134">String collection</span></span>|<span data-ttu-id="53bbc-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="53bbc-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="53bbc-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-137">id</span><span class="sxs-lookup"><span data-stu-id="53bbc-137">id</span></span>|<span data-ttu-id="53bbc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-138">String</span></span>|<span data-ttu-id="53bbc-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53bbc-139">Key of the entity.</span></span> <span data-ttu-id="53bbc-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53bbc-141">createdDateTime</span></span>|<span data-ttu-id="53bbc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bbc-142">DateTimeOffset</span></span>|<span data-ttu-id="53bbc-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="53bbc-143">DateTime the object was created.</span></span> <span data-ttu-id="53bbc-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-145">description</span><span class="sxs-lookup"><span data-stu-id="53bbc-145">description</span></span>|<span data-ttu-id="53bbc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-146">String</span></span>|<span data-ttu-id="53bbc-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53bbc-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53bbc-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53bbc-149">lastModifiedDateTime</span></span>|<span data-ttu-id="53bbc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bbc-150">DateTimeOffset</span></span>|<span data-ttu-id="53bbc-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="53bbc-151">DateTime the object was last modified.</span></span> <span data-ttu-id="53bbc-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="53bbc-153">displayName</span></span>|<span data-ttu-id="53bbc-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-154">String</span></span>|<span data-ttu-id="53bbc-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53bbc-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53bbc-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-157">version</span><span class="sxs-lookup"><span data-stu-id="53bbc-157">version</span></span>|<span data-ttu-id="53bbc-158">Int32</span><span class="sxs-lookup"><span data-stu-id="53bbc-158">Int32</span></span>|<span data-ttu-id="53bbc-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53bbc-159">Version of the device configuration.</span></span> <span data-ttu-id="53bbc-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="53bbc-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="53bbc-161">passwordRequired</span></span>|<span data-ttu-id="53bbc-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-162">Boolean</span></span>|<span data-ttu-id="53bbc-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="53bbc-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="53bbc-164">passwordBlockSimple</span></span>|<span data-ttu-id="53bbc-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-165">Boolean</span></span>|<span data-ttu-id="53bbc-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="53bbc-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="53bbc-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="53bbc-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="53bbc-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-168">Boolean</span></span>|<span data-ttu-id="53bbc-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="53bbc-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="53bbc-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="53bbc-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="53bbc-171">Int32</span><span class="sxs-lookup"><span data-stu-id="53bbc-171">Int32</span></span>|<span data-ttu-id="53bbc-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="53bbc-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="53bbc-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="53bbc-173">passwordExpirationDays</span></span>|<span data-ttu-id="53bbc-174">Int32</span><span class="sxs-lookup"><span data-stu-id="53bbc-174">Int32</span></span>|<span data-ttu-id="53bbc-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="53bbc-175">The password expiration in days.</span></span>|
|<span data-ttu-id="53bbc-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="53bbc-176">passwordMinimumLength</span></span>|<span data-ttu-id="53bbc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="53bbc-177">Int32</span></span>|<span data-ttu-id="53bbc-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="53bbc-178">The minimum password length.</span></span>|
|<span data-ttu-id="53bbc-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="53bbc-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="53bbc-180">Int32</span><span class="sxs-lookup"><span data-stu-id="53bbc-180">Int32</span></span>|<span data-ttu-id="53bbc-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="53bbc-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="53bbc-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="53bbc-182">passwordRequiredType</span></span>|[<span data-ttu-id="53bbc-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="53bbc-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="53bbc-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="53bbc-184">The required password type.</span></span> <span data-ttu-id="53bbc-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="53bbc-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="53bbc-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="53bbc-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="53bbc-187">Int32</span><span class="sxs-lookup"><span data-stu-id="53bbc-187">Int32</span></span>|<span data-ttu-id="53bbc-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="53bbc-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="53bbc-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="53bbc-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="53bbc-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-190">Boolean</span></span>|<span data-ttu-id="53bbc-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="53bbc-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="53bbc-192">osMinimumVersion</span></span>|<span data-ttu-id="53bbc-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-193">String</span></span>|<span data-ttu-id="53bbc-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="53bbc-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="53bbc-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="53bbc-195">osMaximumVersion</span></span>|<span data-ttu-id="53bbc-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-196">String</span></span>|<span data-ttu-id="53bbc-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="53bbc-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="53bbc-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="53bbc-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="53bbc-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-199">String</span></span>|<span data-ttu-id="53bbc-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="53bbc-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="53bbc-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="53bbc-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="53bbc-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-202">String</span></span>|<span data-ttu-id="53bbc-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="53bbc-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="53bbc-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="53bbc-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-205">Boolean</span></span>|<span data-ttu-id="53bbc-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="53bbc-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="53bbc-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-207">bitLockerEnabled</span></span>|<span data-ttu-id="53bbc-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-208">Boolean</span></span>|<span data-ttu-id="53bbc-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="53bbc-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="53bbc-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-210">secureBootEnabled</span></span>|<span data-ttu-id="53bbc-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-211">Boolean</span></span>|<span data-ttu-id="53bbc-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="53bbc-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="53bbc-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="53bbc-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-214">Boolean</span></span>|<span data-ttu-id="53bbc-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="53bbc-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="53bbc-216">storageRequireEncryption</span></span>|<span data-ttu-id="53bbc-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-217">Boolean</span></span>|<span data-ttu-id="53bbc-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="53bbc-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="53bbc-219">activeFirewallRequired</span></span>|<span data-ttu-id="53bbc-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-220">Boolean</span></span>|<span data-ttu-id="53bbc-221">Exigir um firewall ativas em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="53bbc-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-222">defenderEnabled</span></span>|<span data-ttu-id="53bbc-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-223">Boolean</span></span>|<span data-ttu-id="53bbc-224">Exigem o Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="53bbc-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="53bbc-225">defenderVersion</span></span>|<span data-ttu-id="53bbc-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53bbc-226">String</span></span>|<span data-ttu-id="53bbc-227">Exigem a versão mínima do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="53bbc-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="53bbc-228">signatureOutOfDate</span></span>|<span data-ttu-id="53bbc-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-229">Boolean</span></span>|<span data-ttu-id="53bbc-230">Exigem o Windows Defender Antimalware assinatura a ser atualizado em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="53bbc-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-231">rtpEnabled</span></span>|<span data-ttu-id="53bbc-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-232">Boolean</span></span>|<span data-ttu-id="53bbc-233">Exigem proteção em tempo real do Windows Defender Antimalware em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="53bbc-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="53bbc-234">antivirusRequired</span></span>|<span data-ttu-id="53bbc-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-235">Boolean</span></span>|<span data-ttu-id="53bbc-236">Exigir qualquer solução antivírus registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="53bbc-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="53bbc-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="53bbc-237">antiSpywareRequired</span></span>|<span data-ttu-id="53bbc-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-238">Boolean</span></span>|<span data-ttu-id="53bbc-239">Exigir qualquer solução de AntiSpyware registrado na Central de Decurity do Windows para estar ligado e monitoramento (ex.: Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="53bbc-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="53bbc-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="53bbc-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="53bbc-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="53bbc-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="53bbc-242">O sistema operacional válido criar intervalos em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="53bbc-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="53bbc-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="53bbc-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="53bbc-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="53bbc-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="53bbc-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-245">Boolean</span></span>|<span data-ttu-id="53bbc-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="53bbc-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="53bbc-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="53bbc-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="53bbc-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="53bbc-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="53bbc-249">Exigir o nível de risco mínimo de proteção contra ameaças de dispositivo a ser relatado não-conformidade.</span><span class="sxs-lookup"><span data-stu-id="53bbc-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="53bbc-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="53bbc-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="53bbc-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="53bbc-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="53bbc-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="53bbc-252">Boolean</span></span>|<span data-ttu-id="53bbc-253">Exigem a considerar o estado de conformidade do SCCM em consideração para Intune estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="53bbc-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="53bbc-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="53bbc-254">Response</span></span>
<span data-ttu-id="53bbc-255">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53bbc-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53bbc-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53bbc-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="53bbc-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53bbc-257">Request</span></span>
<span data-ttu-id="53bbc-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53bbc-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53bbc-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="53bbc-259">Response</span></span>
<span data-ttu-id="53bbc-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53bbc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





