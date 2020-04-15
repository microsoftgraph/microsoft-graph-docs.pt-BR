---
title: Criar na entidadeandroidworkprofilecompliancepolicy
description: Criar um novo objeto na entidadeandroidworkprofilecompliancepolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd48640a1dd0b6a7dd3e0b8e972d352f797e4774
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470443"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="16654-103">Criar na entidadeandroidworkprofilecompliancepolicy</span><span class="sxs-lookup"><span data-stu-id="16654-103">Create androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="16654-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16654-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16654-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16654-106">Criar um novo objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="16654-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16654-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16654-107">Prerequisites</span></span>
<span data-ttu-id="16654-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16654-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16654-110">Permission type</span></span>|<span data-ttu-id="16654-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16654-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16654-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16654-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16654-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16654-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16654-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16654-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16654-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16654-115">Not supported.</span></span>|
|<span data-ttu-id="16654-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16654-116">Application</span></span>|<span data-ttu-id="16654-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16654-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16654-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16654-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="16654-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16654-119">Request headers</span></span>
|<span data-ttu-id="16654-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16654-120">Header</span></span>|<span data-ttu-id="16654-121">Valor</span><span class="sxs-lookup"><span data-stu-id="16654-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16654-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16654-122">Authorization</span></span>|<span data-ttu-id="16654-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16654-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16654-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16654-124">Accept</span></span>|<span data-ttu-id="16654-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16654-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16654-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16654-126">Request body</span></span>
<span data-ttu-id="16654-127">No corpo da solicitação, forneça uma representação JSON do objeto na entidadeandroidworkprofilecompliancepolicy.</span><span class="sxs-lookup"><span data-stu-id="16654-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="16654-128">A tabela a seguir mostra as propriedades que são necessárias ao criar na entidadeandroidworkprofilecompliancepolicy.</span><span class="sxs-lookup"><span data-stu-id="16654-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="16654-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16654-129">Property</span></span>|<span data-ttu-id="16654-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16654-130">Type</span></span>|<span data-ttu-id="16654-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16654-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16654-132">id</span><span class="sxs-lookup"><span data-stu-id="16654-132">id</span></span>|<span data-ttu-id="16654-133">String</span><span class="sxs-lookup"><span data-stu-id="16654-133">String</span></span>|<span data-ttu-id="16654-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16654-134">Key of the entity.</span></span> <span data-ttu-id="16654-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16654-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="16654-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16654-136">createdDateTime</span></span>|<span data-ttu-id="16654-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16654-137">DateTimeOffset</span></span>|<span data-ttu-id="16654-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="16654-138">DateTime the object was created.</span></span> <span data-ttu-id="16654-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16654-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="16654-140">description</span><span class="sxs-lookup"><span data-stu-id="16654-140">description</span></span>|<span data-ttu-id="16654-141">String</span><span class="sxs-lookup"><span data-stu-id="16654-141">String</span></span>|<span data-ttu-id="16654-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16654-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16654-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16654-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="16654-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16654-144">lastModifiedDateTime</span></span>|<span data-ttu-id="16654-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16654-145">DateTimeOffset</span></span>|<span data-ttu-id="16654-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="16654-146">DateTime the object was last modified.</span></span> <span data-ttu-id="16654-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16654-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="16654-148">displayName</span><span class="sxs-lookup"><span data-stu-id="16654-148">displayName</span></span>|<span data-ttu-id="16654-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16654-149">String</span></span>|<span data-ttu-id="16654-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16654-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16654-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16654-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="16654-152">version</span><span class="sxs-lookup"><span data-stu-id="16654-152">version</span></span>|<span data-ttu-id="16654-153">Int32</span><span class="sxs-lookup"><span data-stu-id="16654-153">Int32</span></span>|<span data-ttu-id="16654-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16654-154">Version of the device configuration.</span></span> <span data-ttu-id="16654-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16654-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="16654-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="16654-156">passwordRequired</span></span>|<span data-ttu-id="16654-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-157">Boolean</span></span>|<span data-ttu-id="16654-158">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16654-158">Require a password to unlock device.</span></span>|
|<span data-ttu-id="16654-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="16654-159">passwordMinimumLength</span></span>|<span data-ttu-id="16654-160">Int32</span><span class="sxs-lookup"><span data-stu-id="16654-160">Int32</span></span>|<span data-ttu-id="16654-161">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="16654-161">Minimum password length.</span></span> <span data-ttu-id="16654-162">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="16654-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="16654-163">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="16654-163">passwordRequiredType</span></span>|[<span data-ttu-id="16654-164">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="16654-164">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="16654-165">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="16654-165">Type of characters in password.</span></span> <span data-ttu-id="16654-166">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="16654-166">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="16654-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="16654-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="16654-168">Int32</span><span class="sxs-lookup"><span data-stu-id="16654-168">Int32</span></span>|<span data-ttu-id="16654-169">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="16654-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="16654-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="16654-170">passwordExpirationDays</span></span>|<span data-ttu-id="16654-171">Int32</span><span class="sxs-lookup"><span data-stu-id="16654-171">Int32</span></span>|<span data-ttu-id="16654-172">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="16654-172">Number of days before the password expires.</span></span> <span data-ttu-id="16654-173">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="16654-173">Valid values 1 to 365</span></span>|
|<span data-ttu-id="16654-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="16654-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="16654-175">Int32</span><span class="sxs-lookup"><span data-stu-id="16654-175">Int32</span></span>|<span data-ttu-id="16654-176">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="16654-176">Number of previous passwords to block.</span></span> <span data-ttu-id="16654-177">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="16654-177">Valid values 1 to 24</span></span>|
|<span data-ttu-id="16654-178">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="16654-178">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="16654-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-179">Boolean</span></span>|<span data-ttu-id="16654-180">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="16654-180">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="16654-181">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="16654-181">securityDisableUsbDebugging</span></span>|<span data-ttu-id="16654-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-182">Boolean</span></span>|<span data-ttu-id="16654-183">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="16654-183">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="16654-184">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="16654-184">securityRequireVerifyApps</span></span>|<span data-ttu-id="16654-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-185">Boolean</span></span>|<span data-ttu-id="16654-186">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="16654-186">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="16654-187">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="16654-187">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="16654-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-188">Boolean</span></span>|<span data-ttu-id="16654-189">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="16654-189">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="16654-190">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="16654-190">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="16654-191">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="16654-191">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="16654-192">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="16654-192">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="16654-193">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="16654-193">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="16654-194">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="16654-194">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="16654-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-195">Boolean</span></span>|<span data-ttu-id="16654-196">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="16654-196">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="16654-197">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="16654-197">osMinimumVersion</span></span>|<span data-ttu-id="16654-198">String</span><span class="sxs-lookup"><span data-stu-id="16654-198">String</span></span>|<span data-ttu-id="16654-199">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="16654-199">Minimum Android version.</span></span>|
|<span data-ttu-id="16654-200">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="16654-200">osMaximumVersion</span></span>|<span data-ttu-id="16654-201">String</span><span class="sxs-lookup"><span data-stu-id="16654-201">String</span></span>|<span data-ttu-id="16654-202">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="16654-202">Maximum Android version.</span></span>|
|<span data-ttu-id="16654-203">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="16654-203">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="16654-204">String</span><span class="sxs-lookup"><span data-stu-id="16654-204">String</span></span>|<span data-ttu-id="16654-205">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="16654-205">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="16654-206">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="16654-206">storageRequireEncryption</span></span>|<span data-ttu-id="16654-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-207">Boolean</span></span>|<span data-ttu-id="16654-208">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="16654-208">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="16654-209">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="16654-209">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="16654-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-210">Boolean</span></span>|<span data-ttu-id="16654-211">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="16654-211">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="16654-212">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="16654-212">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="16654-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-213">Boolean</span></span>|<span data-ttu-id="16654-214">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="16654-214">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="16654-215">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="16654-215">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="16654-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-216">Boolean</span></span>|<span data-ttu-id="16654-217">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16654-217">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="16654-218">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="16654-218">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="16654-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="16654-219">Boolean</span></span>|<span data-ttu-id="16654-220">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="16654-220">Require the device to have up to date security providers.</span></span> <span data-ttu-id="16654-221">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="16654-221">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="16654-222">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="16654-222">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="16654-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="16654-223">Boolean</span></span>|<span data-ttu-id="16654-224">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="16654-224">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="16654-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="16654-225">Response</span></span>
<span data-ttu-id="16654-226">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16654-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16654-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16654-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="16654-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16654-228">Request</span></span>
<span data-ttu-id="16654-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16654-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="16654-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="16654-230">Response</span></span>
<span data-ttu-id="16654-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16654-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






