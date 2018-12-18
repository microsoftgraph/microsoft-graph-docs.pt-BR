---
title: Criar androidForWorkCompliancePolicy
description: Crie um novo objeto de androidForWorkCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 45bce6c48c3b230a9ee751ee28a721323b2a5a29
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362724"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="4dffd-103">Criar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4dffd-103">Create androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="4dffd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4dffd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dffd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4dffd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4dffd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4dffd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dffd-107">Crie um novo objeto de [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4dffd-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4dffd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4dffd-108">Prerequisites</span></span>
<span data-ttu-id="4dffd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dffd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dffd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dffd-111">Permission type</span></span>|<span data-ttu-id="4dffd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4dffd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dffd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dffd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4dffd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dffd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dffd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dffd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dffd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dffd-116">Not supported.</span></span>|
|<span data-ttu-id="4dffd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dffd-117">Application</span></span>|<span data-ttu-id="4dffd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dffd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dffd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dffd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4dffd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dffd-120">Request headers</span></span>
|<span data-ttu-id="4dffd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dffd-121">Header</span></span>|<span data-ttu-id="4dffd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4dffd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dffd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dffd-123">Authorization</span></span>|<span data-ttu-id="4dffd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dffd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dffd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4dffd-125">Accept</span></span>|<span data-ttu-id="4dffd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4dffd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dffd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dffd-127">Request body</span></span>
<span data-ttu-id="4dffd-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="4dffd-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="4dffd-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="4dffd-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="4dffd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dffd-130">Property</span></span>|<span data-ttu-id="4dffd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dffd-131">Type</span></span>|<span data-ttu-id="4dffd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dffd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dffd-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4dffd-133">roleScopeTagIds</span></span>|<span data-ttu-id="4dffd-134">String collection</span><span class="sxs-lookup"><span data-stu-id="4dffd-134">String collection</span></span>|<span data-ttu-id="4dffd-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="4dffd-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4dffd-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-137">id</span><span class="sxs-lookup"><span data-stu-id="4dffd-137">id</span></span>|<span data-ttu-id="4dffd-138">String</span><span class="sxs-lookup"><span data-stu-id="4dffd-138">String</span></span>|<span data-ttu-id="4dffd-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4dffd-139">Key of the entity.</span></span> <span data-ttu-id="4dffd-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4dffd-141">createdDateTime</span></span>|<span data-ttu-id="4dffd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dffd-142">DateTimeOffset</span></span>|<span data-ttu-id="4dffd-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4dffd-143">DateTime the object was created.</span></span> <span data-ttu-id="4dffd-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-145">description</span><span class="sxs-lookup"><span data-stu-id="4dffd-145">description</span></span>|<span data-ttu-id="4dffd-146">String</span><span class="sxs-lookup"><span data-stu-id="4dffd-146">String</span></span>|<span data-ttu-id="4dffd-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dffd-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4dffd-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dffd-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4dffd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dffd-150">DateTimeOffset</span></span>|<span data-ttu-id="4dffd-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4dffd-151">DateTime the object was last modified.</span></span> <span data-ttu-id="4dffd-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4dffd-153">displayName</span></span>|<span data-ttu-id="4dffd-154">String</span><span class="sxs-lookup"><span data-stu-id="4dffd-154">String</span></span>|<span data-ttu-id="4dffd-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dffd-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4dffd-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-157">version</span><span class="sxs-lookup"><span data-stu-id="4dffd-157">version</span></span>|<span data-ttu-id="4dffd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4dffd-158">Int32</span></span>|<span data-ttu-id="4dffd-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dffd-159">Version of the device configuration.</span></span> <span data-ttu-id="4dffd-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dffd-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dffd-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4dffd-161">passwordRequired</span></span>|<span data-ttu-id="4dffd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-162">Boolean</span></span>|<span data-ttu-id="4dffd-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dffd-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="4dffd-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4dffd-164">passwordMinimumLength</span></span>|<span data-ttu-id="4dffd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4dffd-165">Int32</span></span>|<span data-ttu-id="4dffd-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="4dffd-166">Minimum password length.</span></span> <span data-ttu-id="4dffd-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="4dffd-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4dffd-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4dffd-168">passwordRequiredType</span></span>|[<span data-ttu-id="4dffd-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4dffd-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="4dffd-170">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="4dffd-170">Type of characters in password.</span></span> <span data-ttu-id="4dffd-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="4dffd-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="4dffd-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4dffd-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4dffd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="4dffd-173">Int32</span></span>|<span data-ttu-id="4dffd-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="4dffd-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4dffd-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4dffd-175">passwordExpirationDays</span></span>|<span data-ttu-id="4dffd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4dffd-176">Int32</span></span>|<span data-ttu-id="4dffd-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="4dffd-177">Number of days before the password expires.</span></span> <span data-ttu-id="4dffd-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="4dffd-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4dffd-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4dffd-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4dffd-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4dffd-180">Int32</span></span>|<span data-ttu-id="4dffd-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="4dffd-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="4dffd-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="4dffd-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="4dffd-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-183">Boolean</span></span>|<span data-ttu-id="4dffd-184">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="4dffd-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="4dffd-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="4dffd-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="4dffd-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-186">Boolean</span></span>|<span data-ttu-id="4dffd-187">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="4dffd-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="4dffd-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4dffd-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="4dffd-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-189">Boolean</span></span>|<span data-ttu-id="4dffd-190">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="4dffd-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="4dffd-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4dffd-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4dffd-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-192">Boolean</span></span>|<span data-ttu-id="4dffd-193">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="4dffd-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4dffd-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4dffd-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4dffd-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4dffd-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4dffd-196">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="4dffd-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4dffd-197">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4dffd-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4dffd-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4dffd-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4dffd-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-199">Boolean</span></span>|<span data-ttu-id="4dffd-200">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="4dffd-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4dffd-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4dffd-201">osMinimumVersion</span></span>|<span data-ttu-id="4dffd-202">String</span><span class="sxs-lookup"><span data-stu-id="4dffd-202">String</span></span>|<span data-ttu-id="4dffd-203">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="4dffd-203">Minimum Android version.</span></span>|
|<span data-ttu-id="4dffd-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4dffd-204">osMaximumVersion</span></span>|<span data-ttu-id="4dffd-205">String</span><span class="sxs-lookup"><span data-stu-id="4dffd-205">String</span></span>|<span data-ttu-id="4dffd-206">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="4dffd-206">Maximum Android version.</span></span>|
|<span data-ttu-id="4dffd-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4dffd-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="4dffd-208">String</span><span class="sxs-lookup"><span data-stu-id="4dffd-208">String</span></span>|<span data-ttu-id="4dffd-209">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="4dffd-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="4dffd-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4dffd-210">storageRequireEncryption</span></span>|<span data-ttu-id="4dffd-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-211">Boolean</span></span>|<span data-ttu-id="4dffd-212">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="4dffd-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="4dffd-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="4dffd-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="4dffd-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-214">Boolean</span></span>|<span data-ttu-id="4dffd-215">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="4dffd-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="4dffd-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="4dffd-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="4dffd-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-217">Boolean</span></span>|<span data-ttu-id="4dffd-218">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="4dffd-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="4dffd-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="4dffd-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="4dffd-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-220">Boolean</span></span>|<span data-ttu-id="4dffd-221">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dffd-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="4dffd-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="4dffd-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="4dffd-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-223">Boolean</span></span>|<span data-ttu-id="4dffd-224">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="4dffd-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="4dffd-225">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="4dffd-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="4dffd-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="4dffd-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="4dffd-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dffd-227">Boolean</span></span>|<span data-ttu-id="4dffd-228">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="4dffd-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="4dffd-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dffd-229">Response</span></span>
<span data-ttu-id="4dffd-230">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dffd-230">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dffd-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dffd-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="4dffd-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dffd-232">Request</span></span>
<span data-ttu-id="4dffd-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dffd-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1292

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="4dffd-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dffd-234">Response</span></span>
<span data-ttu-id="4dffd-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dffd-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1400

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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





