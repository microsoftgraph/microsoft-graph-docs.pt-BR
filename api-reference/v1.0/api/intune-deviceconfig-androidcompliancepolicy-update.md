---
title: Atualizar androidCompliancePolicy
description: Atualizar as propriedades de um objeto androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74d63c0e6b1285ef22b300cd6ff652d2d2fafcb5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759368"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="74db8-103">Atualizar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="74db8-103">Update androidCompliancePolicy</span></span>

<span data-ttu-id="74db8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74db8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74db8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74db8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74db8-106">Atualizar as propriedades de um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74db8-106">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74db8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74db8-107">Prerequisites</span></span>
<span data-ttu-id="74db8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74db8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74db8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74db8-110">Permission type</span></span>|<span data-ttu-id="74db8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74db8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74db8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74db8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74db8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74db8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74db8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74db8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74db8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74db8-115">Not supported.</span></span>|
|<span data-ttu-id="74db8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74db8-116">Application</span></span>|<span data-ttu-id="74db8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74db8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74db8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74db8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="74db8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74db8-119">Request headers</span></span>
|<span data-ttu-id="74db8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74db8-120">Header</span></span>|<span data-ttu-id="74db8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="74db8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74db8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74db8-122">Authorization</span></span>|<span data-ttu-id="74db8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74db8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74db8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74db8-124">Accept</span></span>|<span data-ttu-id="74db8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74db8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74db8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74db8-126">Request body</span></span>
<span data-ttu-id="74db8-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74db8-127">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="74db8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="74db8-128">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="74db8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74db8-129">Property</span></span>|<span data-ttu-id="74db8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="74db8-130">Type</span></span>|<span data-ttu-id="74db8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="74db8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74db8-132">id</span><span class="sxs-lookup"><span data-stu-id="74db8-132">id</span></span>|<span data-ttu-id="74db8-133">String</span><span class="sxs-lookup"><span data-stu-id="74db8-133">String</span></span>|<span data-ttu-id="74db8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="74db8-134">Key of the entity.</span></span> <span data-ttu-id="74db8-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74db8-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="74db8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74db8-136">createdDateTime</span></span>|<span data-ttu-id="74db8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74db8-137">DateTimeOffset</span></span>|<span data-ttu-id="74db8-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="74db8-138">DateTime the object was created.</span></span> <span data-ttu-id="74db8-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74db8-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="74db8-140">description</span><span class="sxs-lookup"><span data-stu-id="74db8-140">description</span></span>|<span data-ttu-id="74db8-141">String</span><span class="sxs-lookup"><span data-stu-id="74db8-141">String</span></span>|<span data-ttu-id="74db8-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74db8-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74db8-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74db8-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="74db8-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74db8-144">lastModifiedDateTime</span></span>|<span data-ttu-id="74db8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74db8-145">DateTimeOffset</span></span>|<span data-ttu-id="74db8-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="74db8-146">DateTime the object was last modified.</span></span> <span data-ttu-id="74db8-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74db8-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="74db8-148">displayName</span><span class="sxs-lookup"><span data-stu-id="74db8-148">displayName</span></span>|<span data-ttu-id="74db8-149">String</span><span class="sxs-lookup"><span data-stu-id="74db8-149">String</span></span>|<span data-ttu-id="74db8-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74db8-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74db8-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74db8-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="74db8-152">version</span><span class="sxs-lookup"><span data-stu-id="74db8-152">version</span></span>|<span data-ttu-id="74db8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="74db8-153">Int32</span></span>|<span data-ttu-id="74db8-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74db8-154">Version of the device configuration.</span></span> <span data-ttu-id="74db8-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74db8-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="74db8-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="74db8-156">passwordRequired</span></span>|<span data-ttu-id="74db8-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-157">Boolean</span></span>|<span data-ttu-id="74db8-158">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74db8-158">Require a password to unlock device.</span></span>|
|<span data-ttu-id="74db8-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="74db8-159">passwordMinimumLength</span></span>|<span data-ttu-id="74db8-160">Int32</span><span class="sxs-lookup"><span data-stu-id="74db8-160">Int32</span></span>|<span data-ttu-id="74db8-161">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="74db8-161">Minimum password length.</span></span> <span data-ttu-id="74db8-162">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="74db8-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="74db8-163">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="74db8-163">passwordRequiredType</span></span>|[<span data-ttu-id="74db8-164">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="74db8-164">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="74db8-165">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="74db8-165">Type of characters in password.</span></span> <span data-ttu-id="74db8-166">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="74db8-166">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="74db8-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="74db8-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="74db8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="74db8-168">Int32</span></span>|<span data-ttu-id="74db8-169">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="74db8-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="74db8-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="74db8-170">passwordExpirationDays</span></span>|<span data-ttu-id="74db8-171">Int32</span><span class="sxs-lookup"><span data-stu-id="74db8-171">Int32</span></span>|<span data-ttu-id="74db8-172">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="74db8-172">Number of days before the password expires.</span></span> <span data-ttu-id="74db8-173">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="74db8-173">Valid values 1 to 365</span></span>|
|<span data-ttu-id="74db8-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="74db8-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="74db8-175">Int32</span><span class="sxs-lookup"><span data-stu-id="74db8-175">Int32</span></span>|<span data-ttu-id="74db8-176">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="74db8-176">Number of previous passwords to block.</span></span> <span data-ttu-id="74db8-177">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="74db8-177">Valid values 1 to 24</span></span>|
|<span data-ttu-id="74db8-178">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="74db8-178">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="74db8-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-179">Boolean</span></span>|<span data-ttu-id="74db8-180">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="74db8-180">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="74db8-181">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="74db8-181">securityDisableUsbDebugging</span></span>|<span data-ttu-id="74db8-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-182">Boolean</span></span>|<span data-ttu-id="74db8-183">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="74db8-183">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="74db8-184">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="74db8-184">securityRequireVerifyApps</span></span>|<span data-ttu-id="74db8-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-185">Boolean</span></span>|<span data-ttu-id="74db8-186">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="74db8-186">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="74db8-187">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="74db8-187">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="74db8-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-188">Boolean</span></span>|<span data-ttu-id="74db8-189">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="74db8-189">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="74db8-190">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="74db8-190">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="74db8-191">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="74db8-191">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="74db8-192">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="74db8-192">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="74db8-193">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="74db8-193">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="74db8-194">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="74db8-194">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="74db8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-195">Boolean</span></span>|<span data-ttu-id="74db8-196">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="74db8-196">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="74db8-197">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="74db8-197">osMinimumVersion</span></span>|<span data-ttu-id="74db8-198">String</span><span class="sxs-lookup"><span data-stu-id="74db8-198">String</span></span>|<span data-ttu-id="74db8-199">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="74db8-199">Minimum Android version.</span></span>|
|<span data-ttu-id="74db8-200">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="74db8-200">osMaximumVersion</span></span>|<span data-ttu-id="74db8-201">String</span><span class="sxs-lookup"><span data-stu-id="74db8-201">String</span></span>|<span data-ttu-id="74db8-202">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="74db8-202">Maximum Android version.</span></span>|
|<span data-ttu-id="74db8-203">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="74db8-203">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="74db8-204">String</span><span class="sxs-lookup"><span data-stu-id="74db8-204">String</span></span>|<span data-ttu-id="74db8-205">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="74db8-205">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="74db8-206">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="74db8-206">storageRequireEncryption</span></span>|<span data-ttu-id="74db8-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-207">Boolean</span></span>|<span data-ttu-id="74db8-208">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="74db8-208">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="74db8-209">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="74db8-209">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="74db8-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-210">Boolean</span></span>|<span data-ttu-id="74db8-211">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="74db8-211">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="74db8-212">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="74db8-212">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="74db8-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-213">Boolean</span></span>|<span data-ttu-id="74db8-214">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="74db8-214">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="74db8-215">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="74db8-215">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="74db8-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-216">Boolean</span></span>|<span data-ttu-id="74db8-217">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="74db8-217">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="74db8-218">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="74db8-218">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="74db8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-219">Boolean</span></span>|<span data-ttu-id="74db8-220">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="74db8-220">Require the device to have up to date security providers.</span></span> <span data-ttu-id="74db8-221">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="74db8-221">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="74db8-222">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="74db8-222">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="74db8-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="74db8-223">Boolean</span></span>|<span data-ttu-id="74db8-224">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="74db8-224">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="74db8-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="74db8-225">Response</span></span>
<span data-ttu-id="74db8-226">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74db8-226">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74db8-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74db8-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="74db8-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74db8-228">Request</span></span>
<span data-ttu-id="74db8-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74db8-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74db8-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="74db8-230">Response</span></span>
<span data-ttu-id="74db8-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74db8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




