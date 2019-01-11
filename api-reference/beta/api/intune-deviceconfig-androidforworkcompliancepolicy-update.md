---
title: Atualizar androidForWorkCompliancePolicy
description: Atualize as propriedades de um objeto androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b02e7f54d5281478c2489dd86eb4f2d25f27fc7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812730"
---
# <a name="update-androidforworkcompliancepolicy"></a><span data-ttu-id="22ee5-103">Atualizar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="22ee5-103">Update androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="22ee5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="22ee5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22ee5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22ee5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22ee5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22ee5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22ee5-107">Atualize as propriedades de um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="22ee5-107">Update the properties of a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22ee5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22ee5-108">Prerequisites</span></span>
<span data-ttu-id="22ee5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22ee5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ee5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22ee5-111">Permission type</span></span>|<span data-ttu-id="22ee5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22ee5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22ee5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22ee5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22ee5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22ee5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22ee5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22ee5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22ee5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22ee5-116">Not supported.</span></span>|
|<span data-ttu-id="22ee5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22ee5-117">Application</span></span>|<span data-ttu-id="22ee5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22ee5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22ee5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22ee5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="22ee5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22ee5-120">Request headers</span></span>
|<span data-ttu-id="22ee5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22ee5-121">Header</span></span>|<span data-ttu-id="22ee5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22ee5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22ee5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22ee5-123">Authorization</span></span>|<span data-ttu-id="22ee5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22ee5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22ee5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22ee5-125">Accept</span></span>|<span data-ttu-id="22ee5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22ee5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22ee5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22ee5-127">Request body</span></span>
<span data-ttu-id="22ee5-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="22ee5-128">In the request body, supply a JSON representation for the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

<span data-ttu-id="22ee5-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="22ee5-129">The following table shows the properties that are required when you create the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span></span>

|<span data-ttu-id="22ee5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22ee5-130">Property</span></span>|<span data-ttu-id="22ee5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22ee5-131">Type</span></span>|<span data-ttu-id="22ee5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22ee5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ee5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22ee5-133">roleScopeTagIds</span></span>|<span data-ttu-id="22ee5-134">String collection</span><span class="sxs-lookup"><span data-stu-id="22ee5-134">String collection</span></span>|<span data-ttu-id="22ee5-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="22ee5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22ee5-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-137">id</span><span class="sxs-lookup"><span data-stu-id="22ee5-137">id</span></span>|<span data-ttu-id="22ee5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ee5-138">String</span></span>|<span data-ttu-id="22ee5-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22ee5-139">Key of the entity.</span></span> <span data-ttu-id="22ee5-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22ee5-141">createdDateTime</span></span>|<span data-ttu-id="22ee5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ee5-142">DateTimeOffset</span></span>|<span data-ttu-id="22ee5-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22ee5-143">DateTime the object was created.</span></span> <span data-ttu-id="22ee5-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-145">description</span><span class="sxs-lookup"><span data-stu-id="22ee5-145">description</span></span>|<span data-ttu-id="22ee5-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ee5-146">String</span></span>|<span data-ttu-id="22ee5-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22ee5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22ee5-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22ee5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="22ee5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ee5-150">DateTimeOffset</span></span>|<span data-ttu-id="22ee5-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22ee5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="22ee5-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="22ee5-153">displayName</span></span>|<span data-ttu-id="22ee5-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ee5-154">String</span></span>|<span data-ttu-id="22ee5-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22ee5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22ee5-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-157">version</span><span class="sxs-lookup"><span data-stu-id="22ee5-157">version</span></span>|<span data-ttu-id="22ee5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="22ee5-158">Int32</span></span>|<span data-ttu-id="22ee5-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22ee5-159">Version of the device configuration.</span></span> <span data-ttu-id="22ee5-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="22ee5-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="22ee5-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="22ee5-161">passwordRequired</span></span>|<span data-ttu-id="22ee5-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-162">Boolean</span></span>|<span data-ttu-id="22ee5-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22ee5-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="22ee5-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="22ee5-164">passwordMinimumLength</span></span>|<span data-ttu-id="22ee5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="22ee5-165">Int32</span></span>|<span data-ttu-id="22ee5-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="22ee5-166">Minimum password length.</span></span> <span data-ttu-id="22ee5-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="22ee5-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="22ee5-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="22ee5-168">passwordRequiredType</span></span>|[<span data-ttu-id="22ee5-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="22ee5-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="22ee5-170">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="22ee5-170">Type of characters in password.</span></span> <span data-ttu-id="22ee5-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="22ee5-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="22ee5-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="22ee5-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="22ee5-173">Int32</span><span class="sxs-lookup"><span data-stu-id="22ee5-173">Int32</span></span>|<span data-ttu-id="22ee5-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="22ee5-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="22ee5-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="22ee5-175">passwordExpirationDays</span></span>|<span data-ttu-id="22ee5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="22ee5-176">Int32</span></span>|<span data-ttu-id="22ee5-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="22ee5-177">Number of days before the password expires.</span></span> <span data-ttu-id="22ee5-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="22ee5-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="22ee5-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="22ee5-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="22ee5-180">Int32</span><span class="sxs-lookup"><span data-stu-id="22ee5-180">Int32</span></span>|<span data-ttu-id="22ee5-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="22ee5-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="22ee5-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="22ee5-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="22ee5-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-183">Boolean</span></span>|<span data-ttu-id="22ee5-184">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="22ee5-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="22ee5-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="22ee5-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="22ee5-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-186">Boolean</span></span>|<span data-ttu-id="22ee5-187">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="22ee5-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="22ee5-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="22ee5-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="22ee5-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-189">Boolean</span></span>|<span data-ttu-id="22ee5-190">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="22ee5-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="22ee5-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="22ee5-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="22ee5-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-192">Boolean</span></span>|<span data-ttu-id="22ee5-193">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="22ee5-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="22ee5-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="22ee5-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="22ee5-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="22ee5-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="22ee5-196">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="22ee5-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="22ee5-197">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="22ee5-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="22ee5-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="22ee5-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="22ee5-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-199">Boolean</span></span>|<span data-ttu-id="22ee5-200">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="22ee5-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="22ee5-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="22ee5-201">osMinimumVersion</span></span>|<span data-ttu-id="22ee5-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ee5-202">String</span></span>|<span data-ttu-id="22ee5-203">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="22ee5-203">Minimum Android version.</span></span>|
|<span data-ttu-id="22ee5-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="22ee5-204">osMaximumVersion</span></span>|<span data-ttu-id="22ee5-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ee5-205">String</span></span>|<span data-ttu-id="22ee5-206">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="22ee5-206">Maximum Android version.</span></span>|
|<span data-ttu-id="22ee5-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="22ee5-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="22ee5-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ee5-208">String</span></span>|<span data-ttu-id="22ee5-209">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="22ee5-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="22ee5-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="22ee5-210">storageRequireEncryption</span></span>|<span data-ttu-id="22ee5-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-211">Boolean</span></span>|<span data-ttu-id="22ee5-212">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="22ee5-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="22ee5-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="22ee5-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="22ee5-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-214">Boolean</span></span>|<span data-ttu-id="22ee5-215">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="22ee5-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="22ee5-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="22ee5-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="22ee5-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-217">Boolean</span></span>|<span data-ttu-id="22ee5-218">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="22ee5-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="22ee5-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="22ee5-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="22ee5-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-220">Boolean</span></span>|<span data-ttu-id="22ee5-221">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22ee5-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="22ee5-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="22ee5-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="22ee5-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-223">Boolean</span></span>|<span data-ttu-id="22ee5-224">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="22ee5-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="22ee5-225">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="22ee5-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="22ee5-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="22ee5-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="22ee5-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="22ee5-227">Boolean</span></span>|<span data-ttu-id="22ee5-228">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="22ee5-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="22ee5-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ee5-229">Response</span></span>
<span data-ttu-id="22ee5-230">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22ee5-230">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22ee5-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22ee5-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="22ee5-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22ee5-232">Request</span></span>
<span data-ttu-id="22ee5-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22ee5-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22ee5-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ee5-234">Response</span></span>
<span data-ttu-id="22ee5-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22ee5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





