---
title: Atualizar androidWorkProfileCompliancePolicy
description: Atualize as propriedades de um objeto androidWorkProfileCompliancePolicy.
ms.openlocfilehash: 9871cb06295eef9e80ae5700cf64b3e8bdd48bf3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005041"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="82c75-103">Atualizar androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="82c75-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="82c75-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="82c75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82c75-105">Atualize as propriedades de um objeto [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="82c75-105">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82c75-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82c75-106">Prerequisites</span></span>
<span data-ttu-id="82c75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82c75-109">Permission type</span></span>|<span data-ttu-id="82c75-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82c75-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82c75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82c75-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82c75-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c75-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82c75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82c75-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82c75-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c75-114">Not supported.</span></span>|
|<span data-ttu-id="82c75-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82c75-115">Application</span></span>|<span data-ttu-id="82c75-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82c75-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82c75-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82c75-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="82c75-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82c75-118">Request headers</span></span>
|<span data-ttu-id="82c75-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82c75-119">Header</span></span>|<span data-ttu-id="82c75-120">Valor</span><span class="sxs-lookup"><span data-stu-id="82c75-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82c75-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="82c75-121">Authorization</span></span>|<span data-ttu-id="82c75-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82c75-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82c75-123">Accept</span><span class="sxs-lookup"><span data-stu-id="82c75-123">Accept</span></span>|<span data-ttu-id="82c75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82c75-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82c75-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82c75-125">Request body</span></span>
<span data-ttu-id="82c75-126">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="82c75-126">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="82c75-127">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82c75-127">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="82c75-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82c75-128">Property</span></span>|<span data-ttu-id="82c75-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="82c75-129">Type</span></span>|<span data-ttu-id="82c75-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c75-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c75-131">id</span><span class="sxs-lookup"><span data-stu-id="82c75-131">id</span></span>|<span data-ttu-id="82c75-132">String</span><span class="sxs-lookup"><span data-stu-id="82c75-132">String</span></span>|<span data-ttu-id="82c75-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="82c75-133">Key of the entity.</span></span> <span data-ttu-id="82c75-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82c75-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82c75-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82c75-135">createdDateTime</span></span>|<span data-ttu-id="82c75-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82c75-136">DateTimeOffset</span></span>|<span data-ttu-id="82c75-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="82c75-137">DateTime the object was created.</span></span> <span data-ttu-id="82c75-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82c75-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82c75-139">description</span><span class="sxs-lookup"><span data-stu-id="82c75-139">description</span></span>|<span data-ttu-id="82c75-140">String</span><span class="sxs-lookup"><span data-stu-id="82c75-140">String</span></span>|<span data-ttu-id="82c75-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c75-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82c75-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82c75-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82c75-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82c75-143">lastModifiedDateTime</span></span>|<span data-ttu-id="82c75-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82c75-144">DateTimeOffset</span></span>|<span data-ttu-id="82c75-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="82c75-145">DateTime the object was last modified.</span></span> <span data-ttu-id="82c75-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82c75-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82c75-147">displayName</span><span class="sxs-lookup"><span data-stu-id="82c75-147">displayName</span></span>|<span data-ttu-id="82c75-148">String</span><span class="sxs-lookup"><span data-stu-id="82c75-148">String</span></span>|<span data-ttu-id="82c75-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c75-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82c75-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82c75-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82c75-151">version</span><span class="sxs-lookup"><span data-stu-id="82c75-151">version</span></span>|<span data-ttu-id="82c75-152">Int32</span><span class="sxs-lookup"><span data-stu-id="82c75-152">Int32</span></span>|<span data-ttu-id="82c75-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c75-153">Version of the device configuration.</span></span> <span data-ttu-id="82c75-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="82c75-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="82c75-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="82c75-155">passwordRequired</span></span>|<span data-ttu-id="82c75-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-156">Boolean</span></span>|<span data-ttu-id="82c75-157">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c75-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="82c75-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82c75-158">passwordMinimumLength</span></span>|<span data-ttu-id="82c75-159">Int32</span><span class="sxs-lookup"><span data-stu-id="82c75-159">Int32</span></span>|<span data-ttu-id="82c75-160">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="82c75-160">Minimum password length.</span></span> <span data-ttu-id="82c75-161">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="82c75-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="82c75-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="82c75-162">passwordRequiredType</span></span>|[<span data-ttu-id="82c75-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="82c75-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="82c75-164">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="82c75-164">Type of characters in password.</span></span> <span data-ttu-id="82c75-165">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="82c75-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="82c75-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="82c75-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="82c75-167">Int32</span><span class="sxs-lookup"><span data-stu-id="82c75-167">Int32</span></span>|<span data-ttu-id="82c75-168">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="82c75-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="82c75-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="82c75-169">passwordExpirationDays</span></span>|<span data-ttu-id="82c75-170">Int32</span><span class="sxs-lookup"><span data-stu-id="82c75-170">Int32</span></span>|<span data-ttu-id="82c75-171">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="82c75-171">Number of days before the password expires.</span></span> <span data-ttu-id="82c75-172">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="82c75-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="82c75-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="82c75-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="82c75-174">Int32</span><span class="sxs-lookup"><span data-stu-id="82c75-174">Int32</span></span>|<span data-ttu-id="82c75-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="82c75-175">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="82c75-176">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="82c75-176">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="82c75-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-177">Boolean</span></span>|<span data-ttu-id="82c75-178">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="82c75-178">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="82c75-179">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="82c75-179">securityDisableUsbDebugging</span></span>|<span data-ttu-id="82c75-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-180">Boolean</span></span>|<span data-ttu-id="82c75-181">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="82c75-181">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="82c75-182">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="82c75-182">securityRequireVerifyApps</span></span>|<span data-ttu-id="82c75-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-183">Boolean</span></span>|<span data-ttu-id="82c75-184">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="82c75-184">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="82c75-185">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="82c75-185">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="82c75-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-186">Boolean</span></span>|<span data-ttu-id="82c75-187">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="82c75-187">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="82c75-188">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="82c75-188">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="82c75-189">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="82c75-189">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="82c75-190">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="82c75-190">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="82c75-191">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="82c75-191">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="82c75-192">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="82c75-192">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="82c75-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-193">Boolean</span></span>|<span data-ttu-id="82c75-194">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="82c75-194">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="82c75-195">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="82c75-195">osMinimumVersion</span></span>|<span data-ttu-id="82c75-196">String</span><span class="sxs-lookup"><span data-stu-id="82c75-196">String</span></span>|<span data-ttu-id="82c75-197">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="82c75-197">Minimum Android version.</span></span>|
|<span data-ttu-id="82c75-198">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="82c75-198">osMaximumVersion</span></span>|<span data-ttu-id="82c75-199">String</span><span class="sxs-lookup"><span data-stu-id="82c75-199">String</span></span>|<span data-ttu-id="82c75-200">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="82c75-200">Maximum Android version.</span></span>|
|<span data-ttu-id="82c75-201">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="82c75-201">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="82c75-202">String</span><span class="sxs-lookup"><span data-stu-id="82c75-202">String</span></span>|<span data-ttu-id="82c75-203">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="82c75-203">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="82c75-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="82c75-204">storageRequireEncryption</span></span>|<span data-ttu-id="82c75-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-205">Boolean</span></span>|<span data-ttu-id="82c75-206">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="82c75-206">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="82c75-207">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="82c75-207">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="82c75-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-208">Boolean</span></span>|<span data-ttu-id="82c75-209">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="82c75-209">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="82c75-210">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="82c75-210">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="82c75-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-211">Boolean</span></span>|<span data-ttu-id="82c75-212">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="82c75-212">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="82c75-213">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="82c75-213">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="82c75-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-214">Boolean</span></span>|<span data-ttu-id="82c75-215">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82c75-215">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="82c75-216">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="82c75-216">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="82c75-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-217">Boolean</span></span>|<span data-ttu-id="82c75-218">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="82c75-218">Require the device to have up to date security providers.</span></span> <span data-ttu-id="82c75-219">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="82c75-219">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="82c75-220">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="82c75-220">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="82c75-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c75-221">Boolean</span></span>|<span data-ttu-id="82c75-222">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="82c75-222">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="82c75-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c75-223">Response</span></span>
<span data-ttu-id="82c75-224">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82c75-224">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82c75-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82c75-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="82c75-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82c75-226">Request</span></span>
<span data-ttu-id="82c75-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82c75-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "description": "Description value",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="82c75-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="82c75-228">Response</span></span>
<span data-ttu-id="82c75-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82c75-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```



