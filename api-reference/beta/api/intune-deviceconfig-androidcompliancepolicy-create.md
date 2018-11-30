---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
ms.openlocfilehash: dd483b057379f6f3c5fbf27c42507da0cd54f9b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040615"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="af316-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="af316-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="af316-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af316-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af316-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af316-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af316-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af316-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af316-107">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="af316-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af316-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af316-108">Prerequisites</span></span>
<span data-ttu-id="af316-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af316-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af316-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af316-111">Permission type</span></span>|<span data-ttu-id="af316-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af316-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af316-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af316-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af316-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af316-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af316-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af316-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af316-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af316-116">Not supported.</span></span>|
|<span data-ttu-id="af316-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af316-117">Application</span></span>|<span data-ttu-id="af316-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af316-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af316-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af316-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="af316-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af316-120">Request headers</span></span>
|<span data-ttu-id="af316-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af316-121">Header</span></span>|<span data-ttu-id="af316-122">Valor</span><span class="sxs-lookup"><span data-stu-id="af316-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af316-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="af316-123">Authorization</span></span>|<span data-ttu-id="af316-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af316-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af316-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af316-125">Accept</span></span>|<span data-ttu-id="af316-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af316-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af316-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af316-127">Request body</span></span>
<span data-ttu-id="af316-128">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="af316-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="af316-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="af316-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="af316-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af316-130">Property</span></span>|<span data-ttu-id="af316-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="af316-131">Type</span></span>|<span data-ttu-id="af316-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="af316-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af316-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af316-133">roleScopeTagIds</span></span>|<span data-ttu-id="af316-134">String collection</span><span class="sxs-lookup"><span data-stu-id="af316-134">String collection</span></span>|<span data-ttu-id="af316-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="af316-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="af316-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-137">id</span><span class="sxs-lookup"><span data-stu-id="af316-137">id</span></span>|<span data-ttu-id="af316-138">String</span><span class="sxs-lookup"><span data-stu-id="af316-138">String</span></span>|<span data-ttu-id="af316-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="af316-139">Key of the entity.</span></span> <span data-ttu-id="af316-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af316-141">createdDateTime</span></span>|<span data-ttu-id="af316-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af316-142">DateTimeOffset</span></span>|<span data-ttu-id="af316-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="af316-143">DateTime the object was created.</span></span> <span data-ttu-id="af316-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-145">description</span><span class="sxs-lookup"><span data-stu-id="af316-145">description</span></span>|<span data-ttu-id="af316-146">String</span><span class="sxs-lookup"><span data-stu-id="af316-146">String</span></span>|<span data-ttu-id="af316-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af316-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af316-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af316-149">lastModifiedDateTime</span></span>|<span data-ttu-id="af316-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af316-150">DateTimeOffset</span></span>|<span data-ttu-id="af316-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="af316-151">DateTime the object was last modified.</span></span> <span data-ttu-id="af316-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-153">displayName</span><span class="sxs-lookup"><span data-stu-id="af316-153">displayName</span></span>|<span data-ttu-id="af316-154">String</span><span class="sxs-lookup"><span data-stu-id="af316-154">String</span></span>|<span data-ttu-id="af316-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af316-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af316-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-157">version</span><span class="sxs-lookup"><span data-stu-id="af316-157">version</span></span>|<span data-ttu-id="af316-158">Int32</span><span class="sxs-lookup"><span data-stu-id="af316-158">Int32</span></span>|<span data-ttu-id="af316-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af316-159">Version of the device configuration.</span></span> <span data-ttu-id="af316-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af316-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af316-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="af316-161">passwordRequired</span></span>|<span data-ttu-id="af316-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-162">Boolean</span></span>|<span data-ttu-id="af316-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af316-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="af316-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="af316-164">passwordMinimumLength</span></span>|<span data-ttu-id="af316-165">Int32</span><span class="sxs-lookup"><span data-stu-id="af316-165">Int32</span></span>|<span data-ttu-id="af316-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="af316-166">Minimum password length.</span></span> <span data-ttu-id="af316-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="af316-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="af316-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="af316-168">passwordRequiredType</span></span>|[<span data-ttu-id="af316-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="af316-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="af316-170">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="af316-170">Type of characters in password.</span></span> <span data-ttu-id="af316-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="af316-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="af316-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="af316-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="af316-173">Int32</span><span class="sxs-lookup"><span data-stu-id="af316-173">Int32</span></span>|<span data-ttu-id="af316-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="af316-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="af316-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="af316-175">passwordExpirationDays</span></span>|<span data-ttu-id="af316-176">Int32</span><span class="sxs-lookup"><span data-stu-id="af316-176">Int32</span></span>|<span data-ttu-id="af316-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="af316-177">Number of days before the password expires.</span></span> <span data-ttu-id="af316-178">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="af316-178">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="af316-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="af316-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="af316-180">Int32</span><span class="sxs-lookup"><span data-stu-id="af316-180">Int32</span></span>|<span data-ttu-id="af316-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="af316-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="af316-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="af316-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="af316-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-183">Boolean</span></span>|<span data-ttu-id="af316-184">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="af316-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="af316-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="af316-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="af316-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-186">Boolean</span></span>|<span data-ttu-id="af316-187">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="af316-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="af316-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="af316-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="af316-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-189">Boolean</span></span>|<span data-ttu-id="af316-190">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="af316-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="af316-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="af316-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="af316-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-192">Boolean</span></span>|<span data-ttu-id="af316-193">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="af316-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="af316-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="af316-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="af316-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="af316-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="af316-196">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="af316-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="af316-197">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="af316-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="af316-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="af316-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="af316-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-199">Boolean</span></span>|<span data-ttu-id="af316-200">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="af316-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="af316-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="af316-201">osMinimumVersion</span></span>|<span data-ttu-id="af316-202">String</span><span class="sxs-lookup"><span data-stu-id="af316-202">String</span></span>|<span data-ttu-id="af316-203">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="af316-203">Minimum Android version.</span></span>|
|<span data-ttu-id="af316-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="af316-204">osMaximumVersion</span></span>|<span data-ttu-id="af316-205">String</span><span class="sxs-lookup"><span data-stu-id="af316-205">String</span></span>|<span data-ttu-id="af316-206">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="af316-206">Maximum Android version.</span></span>|
|<span data-ttu-id="af316-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="af316-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="af316-208">String</span><span class="sxs-lookup"><span data-stu-id="af316-208">String</span></span>|<span data-ttu-id="af316-209">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="af316-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="af316-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="af316-210">storageRequireEncryption</span></span>|<span data-ttu-id="af316-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-211">Boolean</span></span>|<span data-ttu-id="af316-212">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="af316-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="af316-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="af316-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="af316-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-214">Boolean</span></span>|<span data-ttu-id="af316-215">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="af316-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="af316-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="af316-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="af316-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-217">Boolean</span></span>|<span data-ttu-id="af316-218">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="af316-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="af316-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="af316-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="af316-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-220">Boolean</span></span>|<span data-ttu-id="af316-221">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="af316-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="af316-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="af316-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="af316-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-223">Boolean</span></span>|<span data-ttu-id="af316-224">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="af316-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="af316-225">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="af316-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="af316-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="af316-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="af316-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="af316-227">Boolean</span></span>|<span data-ttu-id="af316-228">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="af316-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="af316-229">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="af316-229">conditionStatementId</span></span>|<span data-ttu-id="af316-230">String</span><span class="sxs-lookup"><span data-stu-id="af316-230">String</span></span>|<span data-ttu-id="af316-231">Id de declaração de condição.</span><span class="sxs-lookup"><span data-stu-id="af316-231">Condition statement id.</span></span>|
|<span data-ttu-id="af316-232">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="af316-232">restrictedApps</span></span>|<span data-ttu-id="af316-233">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="af316-233">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="af316-234">Exigir o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="af316-234">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="af316-235">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="af316-235">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="af316-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="af316-236">Response</span></span>
<span data-ttu-id="af316-237">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af316-237">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af316-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af316-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="af316-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af316-239">Request</span></span>
<span data-ttu-id="af316-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af316-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1597

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="af316-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="af316-241">Response</span></span>
<span data-ttu-id="af316-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af316-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1705

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```





