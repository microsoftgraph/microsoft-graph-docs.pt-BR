---
title: Atualizar androidForWorkCompliancePolicy
description: Atualize as propriedades de um objeto androidForWorkCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 96f2bbe66e7f136166586c8d22d309fbea141475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412818"
---
# <a name="update-androidforworkcompliancepolicy"></a><span data-ttu-id="9a236-103">Atualizar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9a236-103">Update androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="9a236-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a236-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a236-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a236-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a236-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a236-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a236-107">Atualize as propriedades de um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9a236-107">Update the properties of a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a236-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a236-108">Prerequisites</span></span>
<span data-ttu-id="9a236-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a236-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a236-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a236-111">Permission type</span></span>|<span data-ttu-id="9a236-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a236-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a236-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a236-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a236-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a236-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a236-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a236-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a236-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a236-116">Not supported.</span></span>|
|<span data-ttu-id="9a236-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a236-117">Application</span></span>|<span data-ttu-id="9a236-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a236-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a236-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a236-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9a236-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a236-120">Request headers</span></span>
|<span data-ttu-id="9a236-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a236-121">Header</span></span>|<span data-ttu-id="9a236-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a236-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a236-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a236-123">Authorization</span></span>|<span data-ttu-id="9a236-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a236-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a236-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a236-125">Accept</span></span>|<span data-ttu-id="9a236-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a236-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a236-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a236-127">Request body</span></span>
<span data-ttu-id="9a236-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9a236-128">In the request body, supply a JSON representation for the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

<span data-ttu-id="9a236-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9a236-129">The following table shows the properties that are required when you create the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span></span>

|<span data-ttu-id="9a236-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a236-130">Property</span></span>|<span data-ttu-id="9a236-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a236-131">Type</span></span>|<span data-ttu-id="9a236-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a236-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a236-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a236-133">roleScopeTagIds</span></span>|<span data-ttu-id="9a236-134">String collection</span><span class="sxs-lookup"><span data-stu-id="9a236-134">String collection</span></span>|<span data-ttu-id="9a236-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a236-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a236-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-137">id</span><span class="sxs-lookup"><span data-stu-id="9a236-137">id</span></span>|<span data-ttu-id="9a236-138">String</span><span class="sxs-lookup"><span data-stu-id="9a236-138">String</span></span>|<span data-ttu-id="9a236-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a236-139">Key of the entity.</span></span> <span data-ttu-id="9a236-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a236-141">createdDateTime</span></span>|<span data-ttu-id="9a236-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a236-142">DateTimeOffset</span></span>|<span data-ttu-id="9a236-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9a236-143">DateTime the object was created.</span></span> <span data-ttu-id="9a236-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-145">description</span><span class="sxs-lookup"><span data-stu-id="9a236-145">description</span></span>|<span data-ttu-id="9a236-146">String</span><span class="sxs-lookup"><span data-stu-id="9a236-146">String</span></span>|<span data-ttu-id="9a236-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a236-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a236-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a236-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9a236-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a236-150">DateTimeOffset</span></span>|<span data-ttu-id="9a236-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9a236-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9a236-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9a236-153">displayName</span></span>|<span data-ttu-id="9a236-154">String</span><span class="sxs-lookup"><span data-stu-id="9a236-154">String</span></span>|<span data-ttu-id="9a236-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a236-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a236-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-157">version</span><span class="sxs-lookup"><span data-stu-id="9a236-157">version</span></span>|<span data-ttu-id="9a236-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9a236-158">Int32</span></span>|<span data-ttu-id="9a236-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a236-159">Version of the device configuration.</span></span> <span data-ttu-id="9a236-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a236-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a236-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9a236-161">passwordRequired</span></span>|<span data-ttu-id="9a236-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-162">Boolean</span></span>|<span data-ttu-id="9a236-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a236-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="9a236-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9a236-164">passwordMinimumLength</span></span>|<span data-ttu-id="9a236-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9a236-165">Int32</span></span>|<span data-ttu-id="9a236-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="9a236-166">Minimum password length.</span></span> <span data-ttu-id="9a236-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="9a236-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9a236-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9a236-168">passwordRequiredType</span></span>|[<span data-ttu-id="9a236-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9a236-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="9a236-170">Tipo de caracteres na senha.</span><span class="sxs-lookup"><span data-stu-id="9a236-170">Type of characters in password.</span></span> <span data-ttu-id="9a236-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="9a236-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="9a236-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9a236-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9a236-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9a236-173">Int32</span></span>|<span data-ttu-id="9a236-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="9a236-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9a236-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9a236-175">passwordExpirationDays</span></span>|<span data-ttu-id="9a236-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9a236-176">Int32</span></span>|<span data-ttu-id="9a236-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="9a236-177">Number of days before the password expires.</span></span> <span data-ttu-id="9a236-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="9a236-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9a236-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9a236-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9a236-180">Int32</span><span class="sxs-lookup"><span data-stu-id="9a236-180">Int32</span></span>|<span data-ttu-id="9a236-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="9a236-181">Number of previous passwords to block.</span></span> <span data-ttu-id="9a236-182">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="9a236-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9a236-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9a236-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9a236-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9a236-184">Int32</span></span>|<span data-ttu-id="9a236-185">Número de falhas de entrar permitidas antes da restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="9a236-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="9a236-186">Valores válidos 1 a 16</span><span class="sxs-lookup"><span data-stu-id="9a236-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9a236-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="9a236-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="9a236-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-188">Boolean</span></span>|<span data-ttu-id="9a236-189">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="9a236-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="9a236-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="9a236-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="9a236-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-191">Boolean</span></span>|<span data-ttu-id="9a236-192">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="9a236-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="9a236-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="9a236-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="9a236-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-194">Boolean</span></span>|<span data-ttu-id="9a236-195">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="9a236-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="9a236-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9a236-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9a236-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-197">Boolean</span></span>|<span data-ttu-id="9a236-198">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="9a236-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="9a236-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9a236-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9a236-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9a236-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9a236-201">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="9a236-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9a236-202">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="9a236-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9a236-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="9a236-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="9a236-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-204">Boolean</span></span>|<span data-ttu-id="9a236-205">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="9a236-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="9a236-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9a236-206">osMinimumVersion</span></span>|<span data-ttu-id="9a236-207">String</span><span class="sxs-lookup"><span data-stu-id="9a236-207">String</span></span>|<span data-ttu-id="9a236-208">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="9a236-208">Minimum Android version.</span></span>|
|<span data-ttu-id="9a236-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9a236-209">osMaximumVersion</span></span>|<span data-ttu-id="9a236-210">String</span><span class="sxs-lookup"><span data-stu-id="9a236-210">String</span></span>|<span data-ttu-id="9a236-211">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="9a236-211">Maximum Android version.</span></span>|
|<span data-ttu-id="9a236-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9a236-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="9a236-213">String</span><span class="sxs-lookup"><span data-stu-id="9a236-213">String</span></span>|<span data-ttu-id="9a236-214">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="9a236-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="9a236-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9a236-215">storageRequireEncryption</span></span>|<span data-ttu-id="9a236-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-216">Boolean</span></span>|<span data-ttu-id="9a236-217">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="9a236-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="9a236-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="9a236-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="9a236-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-219">Boolean</span></span>|<span data-ttu-id="9a236-220">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="9a236-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="9a236-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="9a236-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="9a236-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-222">Boolean</span></span>|<span data-ttu-id="9a236-223">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="9a236-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="9a236-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="9a236-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="9a236-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-225">Boolean</span></span>|<span data-ttu-id="9a236-226">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a236-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="9a236-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="9a236-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="9a236-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-228">Boolean</span></span>|<span data-ttu-id="9a236-229">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="9a236-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="9a236-230">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="9a236-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="9a236-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="9a236-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="9a236-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a236-232">Boolean</span></span>|<span data-ttu-id="9a236-233">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="9a236-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="9a236-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a236-234">Response</span></span>
<span data-ttu-id="9a236-235">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a236-235">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a236-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a236-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a236-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a236-237">Request</span></span>
<span data-ttu-id="9a236-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a236-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1283

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="9a236-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a236-239">Response</span></span>
<span data-ttu-id="9a236-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a236-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1455

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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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




