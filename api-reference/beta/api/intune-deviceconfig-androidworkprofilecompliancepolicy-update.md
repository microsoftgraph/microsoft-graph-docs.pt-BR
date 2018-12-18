---
title: Atualizar androidWorkProfileCompliancePolicy
description: Atualize as propriedades de um objeto androidWorkProfileCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 7e7bacd9f926d5a3da1012f29ab511067c037a74
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317553"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="6553d-103">Atualizar androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6553d-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="6553d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6553d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6553d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6553d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6553d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6553d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6553d-107">Atualize as propriedades de um objeto [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6553d-107">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6553d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6553d-108">Prerequisites</span></span>
<span data-ttu-id="6553d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6553d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6553d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6553d-111">Permission type</span></span>|<span data-ttu-id="6553d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6553d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6553d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6553d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6553d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6553d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6553d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6553d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6553d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6553d-116">Not supported.</span></span>|
|<span data-ttu-id="6553d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6553d-117">Application</span></span>|<span data-ttu-id="6553d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6553d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6553d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6553d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6553d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6553d-120">Request headers</span></span>
|<span data-ttu-id="6553d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6553d-121">Header</span></span>|<span data-ttu-id="6553d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6553d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6553d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6553d-123">Authorization</span></span>|<span data-ttu-id="6553d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6553d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6553d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6553d-125">Accept</span></span>|<span data-ttu-id="6553d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6553d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6553d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6553d-127">Request body</span></span>
<span data-ttu-id="6553d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6553d-128">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="6553d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6553d-129">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="6553d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6553d-130">Property</span></span>|<span data-ttu-id="6553d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6553d-131">Type</span></span>|<span data-ttu-id="6553d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6553d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6553d-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6553d-133">roleScopeTagIds</span></span>|<span data-ttu-id="6553d-134">String collection</span><span class="sxs-lookup"><span data-stu-id="6553d-134">String collection</span></span>|<span data-ttu-id="6553d-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="6553d-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6553d-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-137">id</span><span class="sxs-lookup"><span data-stu-id="6553d-137">id</span></span>|<span data-ttu-id="6553d-138">String</span><span class="sxs-lookup"><span data-stu-id="6553d-138">String</span></span>|<span data-ttu-id="6553d-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6553d-139">Key of the entity.</span></span> <span data-ttu-id="6553d-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6553d-141">createdDateTime</span></span>|<span data-ttu-id="6553d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6553d-142">DateTimeOffset</span></span>|<span data-ttu-id="6553d-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6553d-143">DateTime the object was created.</span></span> <span data-ttu-id="6553d-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-145">description</span><span class="sxs-lookup"><span data-stu-id="6553d-145">description</span></span>|<span data-ttu-id="6553d-146">String</span><span class="sxs-lookup"><span data-stu-id="6553d-146">String</span></span>|<span data-ttu-id="6553d-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6553d-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6553d-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6553d-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6553d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6553d-150">DateTimeOffset</span></span>|<span data-ttu-id="6553d-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6553d-151">DateTime the object was last modified.</span></span> <span data-ttu-id="6553d-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6553d-153">displayName</span></span>|<span data-ttu-id="6553d-154">String</span><span class="sxs-lookup"><span data-stu-id="6553d-154">String</span></span>|<span data-ttu-id="6553d-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6553d-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6553d-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-157">version</span><span class="sxs-lookup"><span data-stu-id="6553d-157">version</span></span>|<span data-ttu-id="6553d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6553d-158">Int32</span></span>|<span data-ttu-id="6553d-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6553d-159">Version of the device configuration.</span></span> <span data-ttu-id="6553d-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6553d-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6553d-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6553d-161">passwordRequired</span></span>|<span data-ttu-id="6553d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-162">Boolean</span></span>|<span data-ttu-id="6553d-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6553d-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="6553d-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6553d-164">passwordMinimumLength</span></span>|<span data-ttu-id="6553d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6553d-165">Int32</span></span>|<span data-ttu-id="6553d-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="6553d-166">Minimum password length.</span></span> <span data-ttu-id="6553d-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="6553d-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6553d-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6553d-168">passwordRequiredType</span></span>|[<span data-ttu-id="6553d-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6553d-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="6553d-170">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="6553d-170">Type of characters in password.</span></span> <span data-ttu-id="6553d-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="6553d-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="6553d-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6553d-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6553d-173">Int32</span><span class="sxs-lookup"><span data-stu-id="6553d-173">Int32</span></span>|<span data-ttu-id="6553d-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6553d-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6553d-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6553d-175">passwordExpirationDays</span></span>|<span data-ttu-id="6553d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6553d-176">Int32</span></span>|<span data-ttu-id="6553d-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="6553d-177">Number of days before the password expires.</span></span> <span data-ttu-id="6553d-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="6553d-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6553d-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6553d-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6553d-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6553d-180">Int32</span></span>|<span data-ttu-id="6553d-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6553d-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="6553d-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6553d-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="6553d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-183">Boolean</span></span>|<span data-ttu-id="6553d-184">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="6553d-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="6553d-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="6553d-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="6553d-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-186">Boolean</span></span>|<span data-ttu-id="6553d-187">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="6553d-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="6553d-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6553d-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="6553d-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-189">Boolean</span></span>|<span data-ttu-id="6553d-190">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="6553d-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="6553d-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6553d-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6553d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-192">Boolean</span></span>|<span data-ttu-id="6553d-193">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="6553d-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6553d-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6553d-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6553d-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6553d-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6553d-196">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="6553d-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6553d-197">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6553d-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6553d-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6553d-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6553d-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-199">Boolean</span></span>|<span data-ttu-id="6553d-200">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="6553d-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6553d-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6553d-201">osMinimumVersion</span></span>|<span data-ttu-id="6553d-202">String</span><span class="sxs-lookup"><span data-stu-id="6553d-202">String</span></span>|<span data-ttu-id="6553d-203">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="6553d-203">Minimum Android version.</span></span>|
|<span data-ttu-id="6553d-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6553d-204">osMaximumVersion</span></span>|<span data-ttu-id="6553d-205">String</span><span class="sxs-lookup"><span data-stu-id="6553d-205">String</span></span>|<span data-ttu-id="6553d-206">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="6553d-206">Maximum Android version.</span></span>|
|<span data-ttu-id="6553d-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6553d-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="6553d-208">String</span><span class="sxs-lookup"><span data-stu-id="6553d-208">String</span></span>|<span data-ttu-id="6553d-209">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="6553d-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="6553d-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6553d-210">storageRequireEncryption</span></span>|<span data-ttu-id="6553d-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-211">Boolean</span></span>|<span data-ttu-id="6553d-212">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="6553d-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="6553d-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="6553d-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="6553d-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-214">Boolean</span></span>|<span data-ttu-id="6553d-215">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6553d-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="6553d-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="6553d-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="6553d-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-217">Boolean</span></span>|<span data-ttu-id="6553d-218">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6553d-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="6553d-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="6553d-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="6553d-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-220">Boolean</span></span>|<span data-ttu-id="6553d-221">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6553d-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="6553d-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="6553d-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="6553d-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-223">Boolean</span></span>|<span data-ttu-id="6553d-224">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="6553d-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="6553d-225">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="6553d-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="6553d-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="6553d-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="6553d-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="6553d-227">Boolean</span></span>|<span data-ttu-id="6553d-228">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="6553d-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="6553d-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="6553d-229">Response</span></span>
<span data-ttu-id="6553d-230">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6553d-230">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6553d-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6553d-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="6553d-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6553d-232">Request</span></span>
<span data-ttu-id="6553d-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6553d-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1223

{
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

### <a name="response"></a><span data-ttu-id="6553d-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="6553d-234">Response</span></span>
<span data-ttu-id="6553d-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6553d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1404

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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





