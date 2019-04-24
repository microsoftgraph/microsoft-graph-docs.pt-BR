---
title: Atualizar androidForWorkCompliancePolicy
description: Atualiza as propriedades de um objeto androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ee4ad9af831d033aee1ac6e54469e5b591e88a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479320"
---
# <a name="update-androidforworkcompliancepolicy"></a><span data-ttu-id="f4880-103">Atualizar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f4880-103">Update androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="f4880-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4880-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4880-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4880-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4880-106">Atualiza as propriedades de um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f4880-106">Update the properties of a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4880-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4880-107">Prerequisites</span></span>
<span data-ttu-id="f4880-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4880-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4880-110">Permission type</span></span>|<span data-ttu-id="f4880-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4880-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4880-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4880-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4880-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4880-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4880-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4880-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4880-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4880-115">Not supported.</span></span>|
|<span data-ttu-id="f4880-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4880-116">Application</span></span>|<span data-ttu-id="f4880-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4880-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4880-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4880-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f4880-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4880-119">Request headers</span></span>
|<span data-ttu-id="f4880-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4880-120">Header</span></span>|<span data-ttu-id="f4880-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4880-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4880-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4880-122">Authorization</span></span>|<span data-ttu-id="f4880-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4880-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4880-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4880-124">Accept</span></span>|<span data-ttu-id="f4880-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4880-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4880-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4880-126">Request body</span></span>
<span data-ttu-id="f4880-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f4880-127">In the request body, supply a JSON representation for the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

<span data-ttu-id="f4880-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f4880-128">The following table shows the properties that are required when you create the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span></span>

|<span data-ttu-id="f4880-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4880-129">Property</span></span>|<span data-ttu-id="f4880-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4880-130">Type</span></span>|<span data-ttu-id="f4880-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4880-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4880-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4880-132">roleScopeTagIds</span></span>|<span data-ttu-id="f4880-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4880-133">String collection</span></span>|<span data-ttu-id="f4880-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f4880-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4880-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-136">id</span><span class="sxs-lookup"><span data-stu-id="f4880-136">id</span></span>|<span data-ttu-id="f4880-137">String</span><span class="sxs-lookup"><span data-stu-id="f4880-137">String</span></span>|<span data-ttu-id="f4880-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4880-138">Key of the entity.</span></span> <span data-ttu-id="f4880-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4880-140">createdDateTime</span></span>|<span data-ttu-id="f4880-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4880-141">DateTimeOffset</span></span>|<span data-ttu-id="f4880-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f4880-142">DateTime the object was created.</span></span> <span data-ttu-id="f4880-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-144">description</span><span class="sxs-lookup"><span data-stu-id="f4880-144">description</span></span>|<span data-ttu-id="f4880-145">String</span><span class="sxs-lookup"><span data-stu-id="f4880-145">String</span></span>|<span data-ttu-id="f4880-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4880-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4880-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4880-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f4880-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4880-149">DateTimeOffset</span></span>|<span data-ttu-id="f4880-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f4880-150">DateTime the object was last modified.</span></span> <span data-ttu-id="f4880-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f4880-152">displayName</span></span>|<span data-ttu-id="f4880-153">String</span><span class="sxs-lookup"><span data-stu-id="f4880-153">String</span></span>|<span data-ttu-id="f4880-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4880-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4880-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-156">version</span><span class="sxs-lookup"><span data-stu-id="f4880-156">version</span></span>|<span data-ttu-id="f4880-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f4880-157">Int32</span></span>|<span data-ttu-id="f4880-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4880-158">Version of the device configuration.</span></span> <span data-ttu-id="f4880-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f4880-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f4880-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f4880-160">passwordRequired</span></span>|<span data-ttu-id="f4880-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-161">Boolean</span></span>|<span data-ttu-id="f4880-162">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4880-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="f4880-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f4880-163">passwordMinimumLength</span></span>|<span data-ttu-id="f4880-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f4880-164">Int32</span></span>|<span data-ttu-id="f4880-165">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="f4880-165">Minimum password length.</span></span> <span data-ttu-id="f4880-166">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="f4880-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f4880-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f4880-167">passwordRequiredType</span></span>|[<span data-ttu-id="f4880-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f4880-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="f4880-169">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="f4880-169">Type of characters in password.</span></span> <span data-ttu-id="f4880-170">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="f4880-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="f4880-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f4880-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f4880-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f4880-172">Int32</span></span>|<span data-ttu-id="f4880-173">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="f4880-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f4880-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f4880-174">passwordExpirationDays</span></span>|<span data-ttu-id="f4880-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f4880-175">Int32</span></span>|<span data-ttu-id="f4880-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f4880-176">Number of days before the password expires.</span></span> <span data-ttu-id="f4880-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="f4880-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f4880-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f4880-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f4880-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f4880-179">Int32</span></span>|<span data-ttu-id="f4880-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f4880-180">Number of previous passwords to block.</span></span> <span data-ttu-id="f4880-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="f4880-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f4880-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f4880-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f4880-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f4880-183">Int32</span></span>|<span data-ttu-id="f4880-184">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="f4880-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="f4880-185">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="f4880-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f4880-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f4880-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="f4880-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-187">Boolean</span></span>|<span data-ttu-id="f4880-188">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="f4880-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="f4880-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="f4880-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="f4880-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-190">Boolean</span></span>|<span data-ttu-id="f4880-191">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="f4880-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="f4880-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f4880-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="f4880-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-193">Boolean</span></span>|<span data-ttu-id="f4880-194">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="f4880-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f4880-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f4880-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f4880-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-196">Boolean</span></span>|<span data-ttu-id="f4880-197">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="f4880-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="f4880-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f4880-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f4880-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f4880-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f4880-200">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="f4880-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f4880-201">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="f4880-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f4880-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f4880-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f4880-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-203">Boolean</span></span>|<span data-ttu-id="f4880-204">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="f4880-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f4880-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f4880-205">osMinimumVersion</span></span>|<span data-ttu-id="f4880-206">String</span><span class="sxs-lookup"><span data-stu-id="f4880-206">String</span></span>|<span data-ttu-id="f4880-207">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="f4880-207">Minimum Android version.</span></span>|
|<span data-ttu-id="f4880-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f4880-208">osMaximumVersion</span></span>|<span data-ttu-id="f4880-209">String</span><span class="sxs-lookup"><span data-stu-id="f4880-209">String</span></span>|<span data-ttu-id="f4880-210">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="f4880-210">Maximum Android version.</span></span>|
|<span data-ttu-id="f4880-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f4880-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="f4880-212">String</span><span class="sxs-lookup"><span data-stu-id="f4880-212">String</span></span>|<span data-ttu-id="f4880-213">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="f4880-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="f4880-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f4880-214">storageRequireEncryption</span></span>|<span data-ttu-id="f4880-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-215">Boolean</span></span>|<span data-ttu-id="f4880-216">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="f4880-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="f4880-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="f4880-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="f4880-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-218">Boolean</span></span>|<span data-ttu-id="f4880-219">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="f4880-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="f4880-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="f4880-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="f4880-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-221">Boolean</span></span>|<span data-ttu-id="f4880-222">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="f4880-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="f4880-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="f4880-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="f4880-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4880-224">Boolean</span></span>|<span data-ttu-id="f4880-225">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4880-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="f4880-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="f4880-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="f4880-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4880-227">Boolean</span></span>|<span data-ttu-id="f4880-228">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="f4880-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="f4880-229">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="f4880-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="f4880-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="f4880-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="f4880-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4880-231">Boolean</span></span>|<span data-ttu-id="f4880-232">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="f4880-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="f4880-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4880-233">Response</span></span>
<span data-ttu-id="f4880-234">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4880-234">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4880-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4880-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4880-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4880-236">Request</span></span>
<span data-ttu-id="f4880-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4880-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4880-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4880-238">Response</span></span>
<span data-ttu-id="f4880-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4880-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





