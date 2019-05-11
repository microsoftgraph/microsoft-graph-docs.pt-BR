---
title: Criar na entidadeandroidworkprofilecompliancepolicy
description: Criar um novo objeto na entidadeandroidworkprofilecompliancepolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d5ec5bd4b37da58b62a28f8b05f5fa7933051cf8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928656"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="0b4ea-103">Criar na entidadeandroidworkprofilecompliancepolicy</span><span class="sxs-lookup"><span data-stu-id="0b4ea-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="0b4ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b4ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b4ea-106">Criar um novo objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0b4ea-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b4ea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b4ea-107">Prerequisites</span></span>
<span data-ttu-id="0b4ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b4ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b4ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b4ea-110">Permission type</span></span>|<span data-ttu-id="0b4ea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b4ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b4ea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b4ea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b4ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b4ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-115">Not supported.</span></span>|
|<span data-ttu-id="0b4ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b4ea-116">Application</span></span>|<span data-ttu-id="0b4ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b4ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b4ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0b4ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b4ea-119">Request headers</span></span>
|<span data-ttu-id="0b4ea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b4ea-120">Header</span></span>|<span data-ttu-id="0b4ea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b4ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b4ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b4ea-122">Authorization</span></span>|<span data-ttu-id="0b4ea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b4ea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b4ea-124">Accept</span></span>|<span data-ttu-id="0b4ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b4ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b4ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b4ea-126">Request body</span></span>
<span data-ttu-id="0b4ea-127">No corpo da solicitação, forneça uma representação JSON do objeto na entidadeandroidworkprofilecompliancepolicy.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="0b4ea-128">A tabela a seguir mostra as propriedades que são necessárias ao criar na entidadeandroidworkprofilecompliancepolicy.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="0b4ea-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b4ea-129">Property</span></span>|<span data-ttu-id="0b4ea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b4ea-130">Type</span></span>|<span data-ttu-id="0b4ea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b4ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b4ea-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b4ea-132">roleScopeTagIds</span></span>|<span data-ttu-id="0b4ea-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b4ea-133">String collection</span></span>|<span data-ttu-id="0b4ea-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b4ea-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-136">id</span><span class="sxs-lookup"><span data-stu-id="0b4ea-136">id</span></span>|<span data-ttu-id="0b4ea-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b4ea-137">String</span></span>|<span data-ttu-id="0b4ea-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-138">Key of the entity.</span></span> <span data-ttu-id="0b4ea-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b4ea-140">createdDateTime</span></span>|<span data-ttu-id="0b4ea-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b4ea-141">DateTimeOffset</span></span>|<span data-ttu-id="0b4ea-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-142">DateTime the object was created.</span></span> <span data-ttu-id="0b4ea-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-144">description</span><span class="sxs-lookup"><span data-stu-id="0b4ea-144">description</span></span>|<span data-ttu-id="0b4ea-145">String</span><span class="sxs-lookup"><span data-stu-id="0b4ea-145">String</span></span>|<span data-ttu-id="0b4ea-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b4ea-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b4ea-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0b4ea-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b4ea-149">DateTimeOffset</span></span>|<span data-ttu-id="0b4ea-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-150">DateTime the object was last modified.</span></span> <span data-ttu-id="0b4ea-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-152">displayName</span><span class="sxs-lookup"><span data-stu-id="0b4ea-152">displayName</span></span>|<span data-ttu-id="0b4ea-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b4ea-153">String</span></span>|<span data-ttu-id="0b4ea-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b4ea-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-156">version</span><span class="sxs-lookup"><span data-stu-id="0b4ea-156">version</span></span>|<span data-ttu-id="0b4ea-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0b4ea-157">Int32</span></span>|<span data-ttu-id="0b4ea-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-158">Version of the device configuration.</span></span> <span data-ttu-id="0b4ea-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0b4ea-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0b4ea-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0b4ea-160">passwordRequired</span></span>|<span data-ttu-id="0b4ea-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-161">Boolean</span></span>|<span data-ttu-id="0b4ea-162">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="0b4ea-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0b4ea-163">passwordMinimumLength</span></span>|<span data-ttu-id="0b4ea-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0b4ea-164">Int32</span></span>|<span data-ttu-id="0b4ea-165">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-165">Minimum password length.</span></span> <span data-ttu-id="0b4ea-166">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="0b4ea-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0b4ea-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0b4ea-167">passwordRequiredType</span></span>|[<span data-ttu-id="0b4ea-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0b4ea-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="0b4ea-169">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-169">Type of characters in password.</span></span> <span data-ttu-id="0b4ea-170">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="0b4ea-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0b4ea-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0b4ea-172">Int32</span><span class="sxs-lookup"><span data-stu-id="0b4ea-172">Int32</span></span>|<span data-ttu-id="0b4ea-173">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0b4ea-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0b4ea-174">passwordExpirationDays</span></span>|<span data-ttu-id="0b4ea-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0b4ea-175">Int32</span></span>|<span data-ttu-id="0b4ea-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-176">Number of days before the password expires.</span></span> <span data-ttu-id="0b4ea-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="0b4ea-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="0b4ea-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0b4ea-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0b4ea-179">Int32</span><span class="sxs-lookup"><span data-stu-id="0b4ea-179">Int32</span></span>|<span data-ttu-id="0b4ea-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-180">Number of previous passwords to block.</span></span> <span data-ttu-id="0b4ea-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="0b4ea-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0b4ea-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0b4ea-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0b4ea-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0b4ea-183">Int32</span></span>|<span data-ttu-id="0b4ea-184">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="0b4ea-185">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="0b4ea-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="0b4ea-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="0b4ea-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="0b4ea-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-187">Boolean</span></span>|<span data-ttu-id="0b4ea-188">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="0b4ea-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="0b4ea-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="0b4ea-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-190">Boolean</span></span>|<span data-ttu-id="0b4ea-191">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="0b4ea-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="0b4ea-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="0b4ea-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-193">Boolean</span></span>|<span data-ttu-id="0b4ea-194">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="0b4ea-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0b4ea-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0b4ea-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-196">Boolean</span></span>|<span data-ttu-id="0b4ea-197">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0b4ea-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0b4ea-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0b4ea-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0b4ea-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0b4ea-200">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0b4ea-201">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0b4ea-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="0b4ea-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="0b4ea-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-203">Boolean</span></span>|<span data-ttu-id="0b4ea-204">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="0b4ea-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0b4ea-205">osMinimumVersion</span></span>|<span data-ttu-id="0b4ea-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b4ea-206">String</span></span>|<span data-ttu-id="0b4ea-207">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-207">Minimum Android version.</span></span>|
|<span data-ttu-id="0b4ea-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0b4ea-208">osMaximumVersion</span></span>|<span data-ttu-id="0b4ea-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b4ea-209">String</span></span>|<span data-ttu-id="0b4ea-210">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-210">Maximum Android version.</span></span>|
|<span data-ttu-id="0b4ea-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0b4ea-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="0b4ea-212">String</span><span class="sxs-lookup"><span data-stu-id="0b4ea-212">String</span></span>|<span data-ttu-id="0b4ea-213">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="0b4ea-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0b4ea-214">storageRequireEncryption</span></span>|<span data-ttu-id="0b4ea-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-215">Boolean</span></span>|<span data-ttu-id="0b4ea-216">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="0b4ea-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="0b4ea-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="0b4ea-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-218">Boolean</span></span>|<span data-ttu-id="0b4ea-219">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="0b4ea-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="0b4ea-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="0b4ea-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-221">Boolean</span></span>|<span data-ttu-id="0b4ea-222">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="0b4ea-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="0b4ea-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="0b4ea-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b4ea-224">Boolean</span></span>|<span data-ttu-id="0b4ea-225">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="0b4ea-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="0b4ea-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="0b4ea-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b4ea-227">Boolean</span></span>|<span data-ttu-id="0b4ea-228">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="0b4ea-229">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="0b4ea-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="0b4ea-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="0b4ea-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b4ea-231">Boolean</span></span>|<span data-ttu-id="0b4ea-232">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="0b4ea-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b4ea-233">Response</span></span>
<span data-ttu-id="0b4ea-234">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-234">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b4ea-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b4ea-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b4ea-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b4ea-236">Request</span></span>
<span data-ttu-id="0b4ea-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="0b4ea-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b4ea-238">Response</span></span>
<span data-ttu-id="0b4ea-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b4ea-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

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




