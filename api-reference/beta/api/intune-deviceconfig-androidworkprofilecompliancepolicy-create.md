---
title: Criar androidWorkProfileCompliancePolicy
description: Crie um novo objeto androidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d81935d6080f4bf3b7546a28cdef111266220fbf
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666377"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="c6679-103">Criar androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c6679-103">Create androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="c6679-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6679-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6679-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6679-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6679-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6679-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6679-107">Crie um novo [objeto androidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6679-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6679-108">Prerequisites</span></span>
<span data-ttu-id="c6679-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6679-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6679-111">Permission type</span></span>|<span data-ttu-id="c6679-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6679-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6679-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6679-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6679-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6679-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6679-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6679-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6679-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6679-116">Not supported.</span></span>|
|<span data-ttu-id="c6679-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6679-117">Application</span></span>|<span data-ttu-id="c6679-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6679-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6679-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6679-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c6679-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6679-120">Request headers</span></span>
|<span data-ttu-id="c6679-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6679-121">Header</span></span>|<span data-ttu-id="c6679-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c6679-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6679-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6679-123">Authorization</span></span>|<span data-ttu-id="c6679-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6679-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6679-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6679-125">Accept</span></span>|<span data-ttu-id="c6679-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6679-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6679-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6679-127">Request body</span></span>
<span data-ttu-id="c6679-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c6679-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="c6679-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c6679-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="c6679-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6679-130">Property</span></span>|<span data-ttu-id="c6679-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6679-131">Type</span></span>|<span data-ttu-id="c6679-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6679-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6679-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c6679-133">roleScopeTagIds</span></span>|<span data-ttu-id="c6679-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6679-134">String collection</span></span>|<span data-ttu-id="c6679-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="c6679-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c6679-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-137">id</span><span class="sxs-lookup"><span data-stu-id="c6679-137">id</span></span>|<span data-ttu-id="c6679-138">String</span><span class="sxs-lookup"><span data-stu-id="c6679-138">String</span></span>|<span data-ttu-id="c6679-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c6679-139">Key of the entity.</span></span> <span data-ttu-id="c6679-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6679-141">createdDateTime</span></span>|<span data-ttu-id="c6679-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6679-142">DateTimeOffset</span></span>|<span data-ttu-id="c6679-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c6679-143">DateTime the object was created.</span></span> <span data-ttu-id="c6679-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-145">descrição</span><span class="sxs-lookup"><span data-stu-id="c6679-145">description</span></span>|<span data-ttu-id="c6679-146">String</span><span class="sxs-lookup"><span data-stu-id="c6679-146">String</span></span>|<span data-ttu-id="c6679-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6679-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c6679-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6679-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c6679-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6679-150">DateTimeOffset</span></span>|<span data-ttu-id="c6679-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c6679-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c6679-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c6679-153">displayName</span></span>|<span data-ttu-id="c6679-154">String</span><span class="sxs-lookup"><span data-stu-id="c6679-154">String</span></span>|<span data-ttu-id="c6679-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6679-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c6679-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-157">version</span><span class="sxs-lookup"><span data-stu-id="c6679-157">version</span></span>|<span data-ttu-id="c6679-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c6679-158">Int32</span></span>|<span data-ttu-id="c6679-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6679-159">Version of the device configuration.</span></span> <span data-ttu-id="c6679-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c6679-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c6679-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c6679-161">passwordRequired</span></span>|<span data-ttu-id="c6679-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-162">Boolean</span></span>|<span data-ttu-id="c6679-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6679-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="c6679-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c6679-164">passwordMinimumLength</span></span>|<span data-ttu-id="c6679-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c6679-165">Int32</span></span>|<span data-ttu-id="c6679-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="c6679-166">Minimum password length.</span></span> <span data-ttu-id="c6679-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="c6679-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c6679-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c6679-168">passwordRequiredType</span></span>|[<span data-ttu-id="c6679-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c6679-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c6679-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="c6679-170">Type of characters in password.</span></span> <span data-ttu-id="c6679-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c6679-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c6679-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c6679-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c6679-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c6679-173">Int32</span></span>|<span data-ttu-id="c6679-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="c6679-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c6679-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c6679-175">passwordExpirationDays</span></span>|<span data-ttu-id="c6679-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c6679-176">Int32</span></span>|<span data-ttu-id="c6679-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="c6679-177">Number of days before the password expires.</span></span> <span data-ttu-id="c6679-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="c6679-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c6679-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c6679-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c6679-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c6679-180">Int32</span></span>|<span data-ttu-id="c6679-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="c6679-181">Number of previous passwords to block.</span></span> <span data-ttu-id="c6679-182">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="c6679-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c6679-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c6679-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c6679-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c6679-184">Int32</span></span>|<span data-ttu-id="c6679-185">Número de falhas de login permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="c6679-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="c6679-186">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c6679-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c6679-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c6679-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="c6679-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-188">Boolean</span></span>|<span data-ttu-id="c6679-189">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="c6679-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="c6679-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="c6679-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="c6679-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-191">Boolean</span></span>|<span data-ttu-id="c6679-192">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="c6679-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="c6679-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c6679-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="c6679-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-194">Boolean</span></span>|<span data-ttu-id="c6679-195">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="c6679-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c6679-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c6679-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c6679-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-197">Boolean</span></span>|<span data-ttu-id="c6679-198">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="c6679-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c6679-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c6679-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c6679-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c6679-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c6679-201">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="c6679-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c6679-202">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c6679-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c6679-203">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c6679-203">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c6679-204">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c6679-204">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c6679-205">MDATP Exigir nível mínimo de risco da Proteção contra Ameaças Móveis para relatar o descumprimento.</span><span class="sxs-lookup"><span data-stu-id="c6679-205">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c6679-206">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c6679-206">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c6679-207">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c6679-207">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c6679-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-208">Boolean</span></span>|<span data-ttu-id="c6679-209">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="c6679-209">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c6679-210">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c6679-210">osMinimumVersion</span></span>|<span data-ttu-id="c6679-211">String</span><span class="sxs-lookup"><span data-stu-id="c6679-211">String</span></span>|<span data-ttu-id="c6679-212">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="c6679-212">Minimum Android version.</span></span>|
|<span data-ttu-id="c6679-213">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c6679-213">osMaximumVersion</span></span>|<span data-ttu-id="c6679-214">String</span><span class="sxs-lookup"><span data-stu-id="c6679-214">String</span></span>|<span data-ttu-id="c6679-215">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="c6679-215">Maximum Android version.</span></span>|
|<span data-ttu-id="c6679-216">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c6679-216">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="c6679-217">String</span><span class="sxs-lookup"><span data-stu-id="c6679-217">String</span></span>|<span data-ttu-id="c6679-218">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="c6679-218">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="c6679-219">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c6679-219">storageRequireEncryption</span></span>|<span data-ttu-id="c6679-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-220">Boolean</span></span>|<span data-ttu-id="c6679-221">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="c6679-221">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="c6679-222">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c6679-222">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="c6679-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-223">Boolean</span></span>|<span data-ttu-id="c6679-224">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c6679-224">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="c6679-225">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="c6679-225">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="c6679-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-226">Boolean</span></span>|<span data-ttu-id="c6679-227">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c6679-227">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="c6679-228">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="c6679-228">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="c6679-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-229">Boolean</span></span>|<span data-ttu-id="c6679-230">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6679-230">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="c6679-231">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="c6679-231">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="c6679-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-232">Boolean</span></span>|<span data-ttu-id="c6679-233">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="c6679-233">Require the device to have up to date security providers.</span></span> <span data-ttu-id="c6679-234">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="c6679-234">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="c6679-235">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="c6679-235">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="c6679-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6679-236">Boolean</span></span>|<span data-ttu-id="c6679-237">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="c6679-237">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="c6679-238">securityRequiredAndroidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="c6679-238">securityRequiredAndroidSafetyNetEvaluationType</span></span>|[<span data-ttu-id="c6679-239">androidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="c6679-239">androidSafetyNetEvaluationType</span></span>](../resources/intune-deviceconfig-androidsafetynetevaluationtype.md)|<span data-ttu-id="c6679-240">Exigir um tipo de avaliação SafetyNet específico para conformidade.</span><span class="sxs-lookup"><span data-stu-id="c6679-240">Require a specific SafetyNet evaluation type for compliance.</span></span> <span data-ttu-id="c6679-241">Os valores possíveis são: `basic` e `hardwareBacked`.</span><span class="sxs-lookup"><span data-stu-id="c6679-241">Possible values are: `basic`, `hardwareBacked`.</span></span>|



## <a name="response"></a><span data-ttu-id="c6679-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6679-242">Response</span></span>
<span data-ttu-id="c6679-243">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6679-243">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6679-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6679-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6679-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6679-245">Request</span></span>
<span data-ttu-id="c6679-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6679-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1421

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```

### <a name="response"></a><span data-ttu-id="c6679-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6679-247">Response</span></span>
<span data-ttu-id="c6679-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6679-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1593

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```




