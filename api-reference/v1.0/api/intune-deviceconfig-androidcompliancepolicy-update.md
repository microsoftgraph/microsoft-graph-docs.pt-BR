---
title: Atualizar androidCompliancePolicy
description: Atualizar as propriedades de um objeto androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbd709c0b0111240fd2e6b7f79e2888f3f94dd8e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262255"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="548a7-103">Atualizar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="548a7-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="548a7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="548a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="548a7-105">Atualizar as propriedades de um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="548a7-105">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="548a7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="548a7-106">Prerequisites</span></span>
<span data-ttu-id="548a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="548a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="548a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="548a7-109">Permission type</span></span>|<span data-ttu-id="548a7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="548a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="548a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="548a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="548a7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="548a7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="548a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="548a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="548a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="548a7-114">Not supported.</span></span>|
|<span data-ttu-id="548a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="548a7-115">Application</span></span>|<span data-ttu-id="548a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="548a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="548a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="548a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="548a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="548a7-118">Request headers</span></span>
|<span data-ttu-id="548a7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="548a7-119">Header</span></span>|<span data-ttu-id="548a7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="548a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="548a7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="548a7-121">Authorization</span></span>|<span data-ttu-id="548a7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="548a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="548a7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="548a7-123">Accept</span></span>|<span data-ttu-id="548a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="548a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="548a7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="548a7-125">Request body</span></span>
<span data-ttu-id="548a7-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="548a7-126">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="548a7-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="548a7-127">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="548a7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="548a7-128">Property</span></span>|<span data-ttu-id="548a7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="548a7-129">Type</span></span>|<span data-ttu-id="548a7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="548a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="548a7-131">id</span><span class="sxs-lookup"><span data-stu-id="548a7-131">id</span></span>|<span data-ttu-id="548a7-132">String</span><span class="sxs-lookup"><span data-stu-id="548a7-132">String</span></span>|<span data-ttu-id="548a7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="548a7-133">Key of the entity.</span></span> <span data-ttu-id="548a7-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="548a7-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="548a7-135">createdDateTime</span></span>|<span data-ttu-id="548a7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548a7-136">DateTimeOffset</span></span>|<span data-ttu-id="548a7-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="548a7-137">DateTime the object was created.</span></span> <span data-ttu-id="548a7-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="548a7-139">description</span><span class="sxs-lookup"><span data-stu-id="548a7-139">description</span></span>|<span data-ttu-id="548a7-140">String</span><span class="sxs-lookup"><span data-stu-id="548a7-140">String</span></span>|<span data-ttu-id="548a7-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="548a7-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="548a7-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="548a7-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="548a7-143">lastModifiedDateTime</span></span>|<span data-ttu-id="548a7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548a7-144">DateTimeOffset</span></span>|<span data-ttu-id="548a7-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="548a7-145">DateTime the object was last modified.</span></span> <span data-ttu-id="548a7-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="548a7-147">displayName</span><span class="sxs-lookup"><span data-stu-id="548a7-147">displayName</span></span>|<span data-ttu-id="548a7-148">String</span><span class="sxs-lookup"><span data-stu-id="548a7-148">String</span></span>|<span data-ttu-id="548a7-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="548a7-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="548a7-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="548a7-151">version</span><span class="sxs-lookup"><span data-stu-id="548a7-151">version</span></span>|<span data-ttu-id="548a7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="548a7-152">Int32</span></span>|<span data-ttu-id="548a7-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="548a7-153">Version of the device configuration.</span></span> <span data-ttu-id="548a7-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="548a7-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="548a7-155">passwordRequired</span></span>|<span data-ttu-id="548a7-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-156">Boolean</span></span>|<span data-ttu-id="548a7-157">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="548a7-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="548a7-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="548a7-158">passwordMinimumLength</span></span>|<span data-ttu-id="548a7-159">Int32</span><span class="sxs-lookup"><span data-stu-id="548a7-159">Int32</span></span>|<span data-ttu-id="548a7-160">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="548a7-160">Minimum password length.</span></span> <span data-ttu-id="548a7-161">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="548a7-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="548a7-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="548a7-162">passwordRequiredType</span></span>|[<span data-ttu-id="548a7-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="548a7-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="548a7-164">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="548a7-164">Type of characters in password.</span></span> <span data-ttu-id="548a7-165">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="548a7-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="548a7-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="548a7-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="548a7-167">Int32</span><span class="sxs-lookup"><span data-stu-id="548a7-167">Int32</span></span>|<span data-ttu-id="548a7-168">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="548a7-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="548a7-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="548a7-169">passwordExpirationDays</span></span>|<span data-ttu-id="548a7-170">Int32</span><span class="sxs-lookup"><span data-stu-id="548a7-170">Int32</span></span>|<span data-ttu-id="548a7-171">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="548a7-171">Number of days before the password expires.</span></span> <span data-ttu-id="548a7-172">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="548a7-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="548a7-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="548a7-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="548a7-174">Int32</span><span class="sxs-lookup"><span data-stu-id="548a7-174">Int32</span></span>|<span data-ttu-id="548a7-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="548a7-175">Number of previous passwords to block.</span></span> <span data-ttu-id="548a7-176">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="548a7-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="548a7-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="548a7-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="548a7-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-178">Boolean</span></span>|<span data-ttu-id="548a7-179">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="548a7-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="548a7-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="548a7-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="548a7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-181">Boolean</span></span>|<span data-ttu-id="548a7-182">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="548a7-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="548a7-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="548a7-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="548a7-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-184">Boolean</span></span>|<span data-ttu-id="548a7-185">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="548a7-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="548a7-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="548a7-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="548a7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-187">Boolean</span></span>|<span data-ttu-id="548a7-188">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="548a7-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="548a7-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="548a7-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="548a7-190">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="548a7-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="548a7-191">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="548a7-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="548a7-192">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="548a7-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="548a7-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="548a7-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="548a7-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="548a7-194">Boolean</span></span>|<span data-ttu-id="548a7-195">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="548a7-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="548a7-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="548a7-196">osMinimumVersion</span></span>|<span data-ttu-id="548a7-197">String</span><span class="sxs-lookup"><span data-stu-id="548a7-197">String</span></span>|<span data-ttu-id="548a7-198">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="548a7-198">Minimum Android version.</span></span>|
|<span data-ttu-id="548a7-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="548a7-199">osMaximumVersion</span></span>|<span data-ttu-id="548a7-200">String</span><span class="sxs-lookup"><span data-stu-id="548a7-200">String</span></span>|<span data-ttu-id="548a7-201">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="548a7-201">Maximum Android version.</span></span>|
|<span data-ttu-id="548a7-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="548a7-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="548a7-203">String</span><span class="sxs-lookup"><span data-stu-id="548a7-203">String</span></span>|<span data-ttu-id="548a7-204">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="548a7-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="548a7-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="548a7-205">storageRequireEncryption</span></span>|<span data-ttu-id="548a7-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-206">Boolean</span></span>|<span data-ttu-id="548a7-207">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="548a7-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="548a7-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="548a7-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="548a7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-209">Boolean</span></span>|<span data-ttu-id="548a7-210">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="548a7-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="548a7-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="548a7-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="548a7-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-212">Boolean</span></span>|<span data-ttu-id="548a7-213">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="548a7-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="548a7-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="548a7-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="548a7-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-215">Boolean</span></span>|<span data-ttu-id="548a7-216">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="548a7-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="548a7-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="548a7-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="548a7-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-218">Boolean</span></span>|<span data-ttu-id="548a7-219">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="548a7-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="548a7-220">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="548a7-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="548a7-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="548a7-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="548a7-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="548a7-222">Boolean</span></span>|<span data-ttu-id="548a7-223">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="548a7-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="548a7-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="548a7-224">Response</span></span>
<span data-ttu-id="548a7-225">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="548a7-225">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="548a7-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="548a7-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="548a7-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="548a7-227">Request</span></span>
<span data-ttu-id="548a7-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="548a7-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="548a7-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="548a7-229">Response</span></span>
<span data-ttu-id="548a7-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="548a7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



