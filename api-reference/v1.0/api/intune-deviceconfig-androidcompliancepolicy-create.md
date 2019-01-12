---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a42bce7b3cede18b7443b0de91d4e1b09dae910c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966948"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="1d257-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1d257-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="1d257-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1d257-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d257-105">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1d257-105">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d257-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d257-106">Prerequisites</span></span>
<span data-ttu-id="1d257-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d257-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d257-109">Permission type</span></span>|<span data-ttu-id="1d257-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d257-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d257-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d257-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d257-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d257-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d257-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d257-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d257-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d257-114">Not supported.</span></span>|
|<span data-ttu-id="1d257-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d257-115">Application</span></span>|<span data-ttu-id="1d257-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d257-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d257-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d257-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1d257-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d257-118">Request headers</span></span>
|<span data-ttu-id="1d257-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d257-119">Header</span></span>|<span data-ttu-id="1d257-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1d257-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d257-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d257-121">Authorization</span></span>|<span data-ttu-id="1d257-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d257-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d257-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d257-123">Accept</span></span>|<span data-ttu-id="1d257-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1d257-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d257-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d257-125">Request body</span></span>
<span data-ttu-id="1d257-126">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="1d257-126">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="1d257-127">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="1d257-127">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="1d257-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d257-128">Property</span></span>|<span data-ttu-id="1d257-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d257-129">Type</span></span>|<span data-ttu-id="1d257-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d257-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d257-131">id</span><span class="sxs-lookup"><span data-stu-id="1d257-131">id</span></span>|<span data-ttu-id="1d257-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d257-132">String</span></span>|<span data-ttu-id="1d257-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d257-133">Key of the entity.</span></span> <span data-ttu-id="1d257-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1d257-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d257-135">createdDateTime</span></span>|<span data-ttu-id="1d257-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d257-136">DateTimeOffset</span></span>|<span data-ttu-id="1d257-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1d257-137">DateTime the object was created.</span></span> <span data-ttu-id="1d257-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1d257-139">description</span><span class="sxs-lookup"><span data-stu-id="1d257-139">description</span></span>|<span data-ttu-id="1d257-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d257-140">String</span></span>|<span data-ttu-id="1d257-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d257-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d257-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1d257-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d257-143">lastModifiedDateTime</span></span>|<span data-ttu-id="1d257-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d257-144">DateTimeOffset</span></span>|<span data-ttu-id="1d257-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1d257-145">DateTime the object was last modified.</span></span> <span data-ttu-id="1d257-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1d257-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1d257-147">displayName</span></span>|<span data-ttu-id="1d257-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d257-148">String</span></span>|<span data-ttu-id="1d257-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d257-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d257-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1d257-151">version</span><span class="sxs-lookup"><span data-stu-id="1d257-151">version</span></span>|<span data-ttu-id="1d257-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1d257-152">Int32</span></span>|<span data-ttu-id="1d257-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d257-153">Version of the device configuration.</span></span> <span data-ttu-id="1d257-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1d257-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1d257-155">passwordRequired</span></span>|<span data-ttu-id="1d257-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-156">Boolean</span></span>|<span data-ttu-id="1d257-157">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d257-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="1d257-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1d257-158">passwordMinimumLength</span></span>|<span data-ttu-id="1d257-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1d257-159">Int32</span></span>|<span data-ttu-id="1d257-160">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="1d257-160">Minimum password length.</span></span> <span data-ttu-id="1d257-161">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="1d257-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1d257-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1d257-162">passwordRequiredType</span></span>|[<span data-ttu-id="1d257-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1d257-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="1d257-164">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="1d257-164">Type of characters in password.</span></span> <span data-ttu-id="1d257-165">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="1d257-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="1d257-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1d257-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1d257-167">Int32</span><span class="sxs-lookup"><span data-stu-id="1d257-167">Int32</span></span>|<span data-ttu-id="1d257-168">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="1d257-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1d257-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1d257-169">passwordExpirationDays</span></span>|<span data-ttu-id="1d257-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1d257-170">Int32</span></span>|<span data-ttu-id="1d257-171">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="1d257-171">Number of days before the password expires.</span></span> <span data-ttu-id="1d257-172">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="1d257-172">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="1d257-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1d257-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1d257-174">Int32</span><span class="sxs-lookup"><span data-stu-id="1d257-174">Int32</span></span>|<span data-ttu-id="1d257-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="1d257-175">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="1d257-176">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1d257-176">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="1d257-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-177">Boolean</span></span>|<span data-ttu-id="1d257-178">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="1d257-178">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="1d257-179">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="1d257-179">securityDisableUsbDebugging</span></span>|<span data-ttu-id="1d257-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-180">Boolean</span></span>|<span data-ttu-id="1d257-181">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="1d257-181">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="1d257-182">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1d257-182">securityRequireVerifyApps</span></span>|<span data-ttu-id="1d257-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-183">Boolean</span></span>|<span data-ttu-id="1d257-184">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="1d257-184">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="1d257-185">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1d257-185">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="1d257-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-186">Boolean</span></span>|<span data-ttu-id="1d257-187">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="1d257-187">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="1d257-188">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="1d257-188">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="1d257-189">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="1d257-189">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="1d257-190">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="1d257-190">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1d257-191">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1d257-191">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1d257-192">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="1d257-192">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="1d257-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-193">Boolean</span></span>|<span data-ttu-id="1d257-194">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="1d257-194">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="1d257-195">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1d257-195">osMinimumVersion</span></span>|<span data-ttu-id="1d257-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d257-196">String</span></span>|<span data-ttu-id="1d257-197">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="1d257-197">Minimum Android version.</span></span>|
|<span data-ttu-id="1d257-198">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1d257-198">osMaximumVersion</span></span>|<span data-ttu-id="1d257-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d257-199">String</span></span>|<span data-ttu-id="1d257-200">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="1d257-200">Maximum Android version.</span></span>|
|<span data-ttu-id="1d257-201">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1d257-201">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="1d257-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d257-202">String</span></span>|<span data-ttu-id="1d257-203">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="1d257-203">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="1d257-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1d257-204">storageRequireEncryption</span></span>|<span data-ttu-id="1d257-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-205">Boolean</span></span>|<span data-ttu-id="1d257-206">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="1d257-206">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="1d257-207">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="1d257-207">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="1d257-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-208">Boolean</span></span>|<span data-ttu-id="1d257-209">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="1d257-209">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="1d257-210">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="1d257-210">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="1d257-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-211">Boolean</span></span>|<span data-ttu-id="1d257-212">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="1d257-212">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="1d257-213">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="1d257-213">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="1d257-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-214">Boolean</span></span>|<span data-ttu-id="1d257-215">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d257-215">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="1d257-216">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="1d257-216">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="1d257-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-217">Boolean</span></span>|<span data-ttu-id="1d257-218">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="1d257-218">Require the device to have up to date security providers.</span></span> <span data-ttu-id="1d257-219">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="1d257-219">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="1d257-220">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="1d257-220">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="1d257-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d257-221">Boolean</span></span>|<span data-ttu-id="1d257-222">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="1d257-222">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="1d257-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d257-223">Response</span></span>
<span data-ttu-id="1d257-224">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d257-224">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d257-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d257-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d257-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d257-226">Request</span></span>
<span data-ttu-id="1d257-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d257-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="1d257-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d257-228">Response</span></span>
<span data-ttu-id="1d257-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d257-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```



