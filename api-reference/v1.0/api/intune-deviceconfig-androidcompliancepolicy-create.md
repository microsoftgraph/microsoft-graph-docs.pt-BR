---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0515e73d4e348fd9bc413aa1f52319cf7e31bb15
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43316730"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="ba5d2-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ba5d2-103">Create androidCompliancePolicy</span></span>

<span data-ttu-id="ba5d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba5d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba5d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba5d2-106">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ba5d2-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba5d2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba5d2-107">Prerequisites</span></span>
<span data-ttu-id="ba5d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba5d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba5d2-110">Permission type</span></span>|<span data-ttu-id="ba5d2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba5d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba5d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba5d2-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba5d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-115">Not supported.</span></span>|
|<span data-ttu-id="ba5d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba5d2-116">Application</span></span>|<span data-ttu-id="ba5d2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba5d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba5d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ba5d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba5d2-119">Request headers</span></span>
|<span data-ttu-id="ba5d2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba5d2-120">Header</span></span>|<span data-ttu-id="ba5d2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ba5d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba5d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba5d2-122">Authorization</span></span>|<span data-ttu-id="ba5d2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba5d2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba5d2-124">Accept</span></span>|<span data-ttu-id="ba5d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba5d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba5d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba5d2-126">Request body</span></span>
<span data-ttu-id="ba5d2-127">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="ba5d2-128">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="ba5d2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba5d2-129">Property</span></span>|<span data-ttu-id="ba5d2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba5d2-130">Type</span></span>|<span data-ttu-id="ba5d2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba5d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba5d2-132">id</span><span class="sxs-lookup"><span data-stu-id="ba5d2-132">id</span></span>|<span data-ttu-id="ba5d2-133">String</span><span class="sxs-lookup"><span data-stu-id="ba5d2-133">String</span></span>|<span data-ttu-id="ba5d2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-134">Key of the entity.</span></span> <span data-ttu-id="ba5d2-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba5d2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba5d2-136">createdDateTime</span></span>|<span data-ttu-id="ba5d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba5d2-137">DateTimeOffset</span></span>|<span data-ttu-id="ba5d2-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-138">DateTime the object was created.</span></span> <span data-ttu-id="ba5d2-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba5d2-140">description</span><span class="sxs-lookup"><span data-stu-id="ba5d2-140">description</span></span>|<span data-ttu-id="ba5d2-141">String</span><span class="sxs-lookup"><span data-stu-id="ba5d2-141">String</span></span>|<span data-ttu-id="ba5d2-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ba5d2-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba5d2-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba5d2-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ba5d2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba5d2-145">DateTimeOffset</span></span>|<span data-ttu-id="ba5d2-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-146">DateTime the object was last modified.</span></span> <span data-ttu-id="ba5d2-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba5d2-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ba5d2-148">displayName</span></span>|<span data-ttu-id="ba5d2-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba5d2-149">String</span></span>|<span data-ttu-id="ba5d2-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ba5d2-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba5d2-152">version</span><span class="sxs-lookup"><span data-stu-id="ba5d2-152">version</span></span>|<span data-ttu-id="ba5d2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d2-153">Int32</span></span>|<span data-ttu-id="ba5d2-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-154">Version of the device configuration.</span></span> <span data-ttu-id="ba5d2-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d2-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ba5d2-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ba5d2-156">passwordRequired</span></span>|<span data-ttu-id="ba5d2-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-157">Boolean</span></span>|<span data-ttu-id="ba5d2-158">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-158">Require a password to unlock device.</span></span>|
|<span data-ttu-id="ba5d2-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ba5d2-159">passwordMinimumLength</span></span>|<span data-ttu-id="ba5d2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d2-160">Int32</span></span>|<span data-ttu-id="ba5d2-161">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-161">Minimum password length.</span></span> <span data-ttu-id="ba5d2-162">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="ba5d2-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ba5d2-163">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ba5d2-163">passwordRequiredType</span></span>|[<span data-ttu-id="ba5d2-164">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ba5d2-164">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="ba5d2-165">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-165">Type of characters in password.</span></span> <span data-ttu-id="ba5d2-166">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-166">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="ba5d2-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ba5d2-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ba5d2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d2-168">Int32</span></span>|<span data-ttu-id="ba5d2-169">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ba5d2-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ba5d2-170">passwordExpirationDays</span></span>|<span data-ttu-id="ba5d2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d2-171">Int32</span></span>|<span data-ttu-id="ba5d2-172">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-172">Number of days before the password expires.</span></span> <span data-ttu-id="ba5d2-173">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="ba5d2-173">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ba5d2-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ba5d2-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ba5d2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d2-175">Int32</span></span>|<span data-ttu-id="ba5d2-176">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-176">Number of previous passwords to block.</span></span> <span data-ttu-id="ba5d2-177">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="ba5d2-177">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ba5d2-178">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="ba5d2-178">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="ba5d2-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-179">Boolean</span></span>|<span data-ttu-id="ba5d2-180">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-180">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="ba5d2-181">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="ba5d2-181">securityDisableUsbDebugging</span></span>|<span data-ttu-id="ba5d2-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-182">Boolean</span></span>|<span data-ttu-id="ba5d2-183">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-183">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="ba5d2-184">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="ba5d2-184">securityRequireVerifyApps</span></span>|<span data-ttu-id="ba5d2-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-185">Boolean</span></span>|<span data-ttu-id="ba5d2-186">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-186">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="ba5d2-187">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ba5d2-187">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ba5d2-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-188">Boolean</span></span>|<span data-ttu-id="ba5d2-189">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-189">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ba5d2-190">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ba5d2-190">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ba5d2-191">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ba5d2-191">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ba5d2-192">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-192">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ba5d2-193">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-193">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ba5d2-194">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="ba5d2-194">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="ba5d2-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-195">Boolean</span></span>|<span data-ttu-id="ba5d2-196">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-196">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="ba5d2-197">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ba5d2-197">osMinimumVersion</span></span>|<span data-ttu-id="ba5d2-198">String</span><span class="sxs-lookup"><span data-stu-id="ba5d2-198">String</span></span>|<span data-ttu-id="ba5d2-199">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-199">Minimum Android version.</span></span>|
|<span data-ttu-id="ba5d2-200">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ba5d2-200">osMaximumVersion</span></span>|<span data-ttu-id="ba5d2-201">String</span><span class="sxs-lookup"><span data-stu-id="ba5d2-201">String</span></span>|<span data-ttu-id="ba5d2-202">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-202">Maximum Android version.</span></span>|
|<span data-ttu-id="ba5d2-203">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ba5d2-203">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="ba5d2-204">String</span><span class="sxs-lookup"><span data-stu-id="ba5d2-204">String</span></span>|<span data-ttu-id="ba5d2-205">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-205">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="ba5d2-206">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ba5d2-206">storageRequireEncryption</span></span>|<span data-ttu-id="ba5d2-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-207">Boolean</span></span>|<span data-ttu-id="ba5d2-208">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-208">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="ba5d2-209">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="ba5d2-209">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="ba5d2-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-210">Boolean</span></span>|<span data-ttu-id="ba5d2-211">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-211">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="ba5d2-212">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="ba5d2-212">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="ba5d2-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-213">Boolean</span></span>|<span data-ttu-id="ba5d2-214">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-214">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="ba5d2-215">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="ba5d2-215">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="ba5d2-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-216">Boolean</span></span>|<span data-ttu-id="ba5d2-217">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-217">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="ba5d2-218">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="ba5d2-218">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="ba5d2-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba5d2-219">Boolean</span></span>|<span data-ttu-id="ba5d2-220">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-220">Require the device to have up to date security providers.</span></span> <span data-ttu-id="ba5d2-221">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-221">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="ba5d2-222">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="ba5d2-222">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="ba5d2-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba5d2-223">Boolean</span></span>|<span data-ttu-id="ba5d2-224">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-224">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="ba5d2-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba5d2-225">Response</span></span>
<span data-ttu-id="ba5d2-226">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-226">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba5d2-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba5d2-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba5d2-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba5d2-228">Request</span></span>
<span data-ttu-id="ba5d2-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba5d2-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba5d2-230">Response</span></span>
<span data-ttu-id="ba5d2-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba5d2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






