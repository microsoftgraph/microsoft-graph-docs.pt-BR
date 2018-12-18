---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: d09040d1db8d2516cf186b72e26ad24782b76328
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322565"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="0c1be-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0c1be-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="0c1be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c1be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c1be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c1be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c1be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c1be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c1be-107">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0c1be-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c1be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c1be-108">Prerequisites</span></span>
<span data-ttu-id="0c1be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c1be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c1be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c1be-111">Permission type</span></span>|<span data-ttu-id="0c1be-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c1be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c1be-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c1be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c1be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c1be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c1be-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c1be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c1be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c1be-116">Not supported.</span></span>|
|<span data-ttu-id="0c1be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c1be-117">Application</span></span>|<span data-ttu-id="0c1be-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c1be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c1be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c1be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0c1be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c1be-120">Request headers</span></span>
|<span data-ttu-id="0c1be-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c1be-121">Header</span></span>|<span data-ttu-id="0c1be-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0c1be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c1be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c1be-123">Authorization</span></span>|<span data-ttu-id="0c1be-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c1be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c1be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c1be-125">Accept</span></span>|<span data-ttu-id="0c1be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c1be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c1be-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c1be-127">Request body</span></span>
<span data-ttu-id="0c1be-128">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0c1be-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="0c1be-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0c1be-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="0c1be-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c1be-130">Property</span></span>|<span data-ttu-id="0c1be-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c1be-131">Type</span></span>|<span data-ttu-id="0c1be-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c1be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c1be-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c1be-133">roleScopeTagIds</span></span>|<span data-ttu-id="0c1be-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0c1be-134">String collection</span></span>|<span data-ttu-id="0c1be-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c1be-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0c1be-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-137">id</span><span class="sxs-lookup"><span data-stu-id="0c1be-137">id</span></span>|<span data-ttu-id="0c1be-138">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-138">String</span></span>|<span data-ttu-id="0c1be-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c1be-139">Key of the entity.</span></span> <span data-ttu-id="0c1be-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c1be-141">createdDateTime</span></span>|<span data-ttu-id="0c1be-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c1be-142">DateTimeOffset</span></span>|<span data-ttu-id="0c1be-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0c1be-143">DateTime the object was created.</span></span> <span data-ttu-id="0c1be-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-145">description</span><span class="sxs-lookup"><span data-stu-id="0c1be-145">description</span></span>|<span data-ttu-id="0c1be-146">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-146">String</span></span>|<span data-ttu-id="0c1be-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c1be-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c1be-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c1be-149">lastModifiedDateTime</span></span>|<span data-ttu-id="0c1be-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c1be-150">DateTimeOffset</span></span>|<span data-ttu-id="0c1be-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0c1be-151">DateTime the object was last modified.</span></span> <span data-ttu-id="0c1be-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0c1be-153">displayName</span></span>|<span data-ttu-id="0c1be-154">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-154">String</span></span>|<span data-ttu-id="0c1be-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c1be-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c1be-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-157">version</span><span class="sxs-lookup"><span data-stu-id="0c1be-157">version</span></span>|<span data-ttu-id="0c1be-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0c1be-158">Int32</span></span>|<span data-ttu-id="0c1be-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c1be-159">Version of the device configuration.</span></span> <span data-ttu-id="0c1be-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0c1be-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0c1be-161">passwordRequired</span></span>|<span data-ttu-id="0c1be-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-162">Boolean</span></span>|<span data-ttu-id="0c1be-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c1be-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="0c1be-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0c1be-164">passwordMinimumLength</span></span>|<span data-ttu-id="0c1be-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0c1be-165">Int32</span></span>|<span data-ttu-id="0c1be-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0c1be-166">Minimum password length.</span></span> <span data-ttu-id="0c1be-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="0c1be-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0c1be-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0c1be-168">passwordRequiredType</span></span>|[<span data-ttu-id="0c1be-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0c1be-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="0c1be-170">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="0c1be-170">Type of characters in password.</span></span> <span data-ttu-id="0c1be-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="0c1be-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="0c1be-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0c1be-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0c1be-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0c1be-173">Int32</span></span>|<span data-ttu-id="0c1be-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0c1be-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0c1be-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0c1be-175">passwordExpirationDays</span></span>|<span data-ttu-id="0c1be-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0c1be-176">Int32</span></span>|<span data-ttu-id="0c1be-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="0c1be-177">Number of days before the password expires.</span></span> <span data-ttu-id="0c1be-178">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="0c1be-178">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0c1be-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0c1be-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0c1be-180">Int32</span><span class="sxs-lookup"><span data-stu-id="0c1be-180">Int32</span></span>|<span data-ttu-id="0c1be-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="0c1be-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="0c1be-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="0c1be-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="0c1be-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-183">Boolean</span></span>|<span data-ttu-id="0c1be-184">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="0c1be-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="0c1be-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="0c1be-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="0c1be-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-186">Boolean</span></span>|<span data-ttu-id="0c1be-187">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="0c1be-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="0c1be-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="0c1be-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="0c1be-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-189">Boolean</span></span>|<span data-ttu-id="0c1be-190">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="0c1be-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="0c1be-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0c1be-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0c1be-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-192">Boolean</span></span>|<span data-ttu-id="0c1be-193">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="0c1be-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0c1be-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0c1be-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0c1be-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0c1be-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0c1be-196">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="0c1be-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0c1be-197">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0c1be-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0c1be-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="0c1be-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="0c1be-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-199">Boolean</span></span>|<span data-ttu-id="0c1be-200">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="0c1be-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="0c1be-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0c1be-201">osMinimumVersion</span></span>|<span data-ttu-id="0c1be-202">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-202">String</span></span>|<span data-ttu-id="0c1be-203">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="0c1be-203">Minimum Android version.</span></span>|
|<span data-ttu-id="0c1be-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0c1be-204">osMaximumVersion</span></span>|<span data-ttu-id="0c1be-205">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-205">String</span></span>|<span data-ttu-id="0c1be-206">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="0c1be-206">Maximum Android version.</span></span>|
|<span data-ttu-id="0c1be-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0c1be-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="0c1be-208">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-208">String</span></span>|<span data-ttu-id="0c1be-209">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="0c1be-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="0c1be-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0c1be-210">storageRequireEncryption</span></span>|<span data-ttu-id="0c1be-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-211">Boolean</span></span>|<span data-ttu-id="0c1be-212">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="0c1be-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="0c1be-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="0c1be-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="0c1be-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-214">Boolean</span></span>|<span data-ttu-id="0c1be-215">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="0c1be-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="0c1be-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="0c1be-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="0c1be-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-217">Boolean</span></span>|<span data-ttu-id="0c1be-218">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="0c1be-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="0c1be-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="0c1be-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="0c1be-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-220">Boolean</span></span>|<span data-ttu-id="0c1be-221">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c1be-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="0c1be-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="0c1be-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="0c1be-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-223">Boolean</span></span>|<span data-ttu-id="0c1be-224">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="0c1be-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="0c1be-225">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="0c1be-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="0c1be-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="0c1be-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="0c1be-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1be-227">Boolean</span></span>|<span data-ttu-id="0c1be-228">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="0c1be-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="0c1be-229">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="0c1be-229">conditionStatementId</span></span>|<span data-ttu-id="0c1be-230">String</span><span class="sxs-lookup"><span data-stu-id="0c1be-230">String</span></span>|<span data-ttu-id="0c1be-231">Id de declaração de condição.</span><span class="sxs-lookup"><span data-stu-id="0c1be-231">Condition statement id.</span></span>|
|<span data-ttu-id="0c1be-232">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="0c1be-232">restrictedApps</span></span>|<span data-ttu-id="0c1be-233">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0c1be-233">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0c1be-234">Exigir o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="0c1be-234">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="0c1be-235">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="0c1be-235">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0c1be-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c1be-236">Response</span></span>
<span data-ttu-id="0c1be-237">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c1be-237">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c1be-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c1be-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c1be-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c1be-239">Request</span></span>
<span data-ttu-id="0c1be-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c1be-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c1be-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c1be-241">Response</span></span>
<span data-ttu-id="0c1be-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c1be-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





