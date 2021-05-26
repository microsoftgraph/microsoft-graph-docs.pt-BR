---
title: Criar androidForWorkCompliancePolicy
description: Crie um novo objeto androidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac3affaf984f252e51bcdcf8490dd8294217a6d5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665501"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="5ebe3-103">Criar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5ebe3-103">Create androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="5ebe3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ebe3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ebe3-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ebe3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ebe3-107">Crie um novo [objeto androidForWorkCompliancePolicy.](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ebe3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ebe3-108">Prerequisites</span></span>
<span data-ttu-id="5ebe3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebe3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ebe3-111">Permission type</span></span>|<span data-ttu-id="5ebe3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ebe3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ebe3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebe3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ebe3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ebe3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-116">Not supported.</span></span>|
|<span data-ttu-id="5ebe3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ebe3-117">Application</span></span>|<span data-ttu-id="5ebe3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebe3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ebe3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebe3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5ebe3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebe3-120">Request headers</span></span>
|<span data-ttu-id="5ebe3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ebe3-121">Header</span></span>|<span data-ttu-id="5ebe3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ebe3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ebe3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ebe3-123">Authorization</span></span>|<span data-ttu-id="5ebe3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ebe3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ebe3-125">Accept</span></span>|<span data-ttu-id="5ebe3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ebe3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebe3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebe3-127">Request body</span></span>
<span data-ttu-id="5ebe3-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="5ebe3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="5ebe3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ebe3-130">Property</span></span>|<span data-ttu-id="5ebe3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ebe3-131">Type</span></span>|<span data-ttu-id="5ebe3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ebe3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebe3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ebe3-133">roleScopeTagIds</span></span>|<span data-ttu-id="5ebe3-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ebe3-134">String collection</span></span>|<span data-ttu-id="5ebe3-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ebe3-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-137">id</span><span class="sxs-lookup"><span data-stu-id="5ebe3-137">id</span></span>|<span data-ttu-id="5ebe3-138">String</span><span class="sxs-lookup"><span data-stu-id="5ebe3-138">String</span></span>|<span data-ttu-id="5ebe3-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-139">Key of the entity.</span></span> <span data-ttu-id="5ebe3-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebe3-141">createdDateTime</span></span>|<span data-ttu-id="5ebe3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebe3-142">DateTimeOffset</span></span>|<span data-ttu-id="5ebe3-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-143">DateTime the object was created.</span></span> <span data-ttu-id="5ebe3-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-145">descrição</span><span class="sxs-lookup"><span data-stu-id="5ebe3-145">description</span></span>|<span data-ttu-id="5ebe3-146">String</span><span class="sxs-lookup"><span data-stu-id="5ebe3-146">String</span></span>|<span data-ttu-id="5ebe3-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ebe3-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebe3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="5ebe3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebe3-150">DateTimeOffset</span></span>|<span data-ttu-id="5ebe3-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="5ebe3-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="5ebe3-153">displayName</span></span>|<span data-ttu-id="5ebe3-154">String</span><span class="sxs-lookup"><span data-stu-id="5ebe3-154">String</span></span>|<span data-ttu-id="5ebe3-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ebe3-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-157">version</span><span class="sxs-lookup"><span data-stu-id="5ebe3-157">version</span></span>|<span data-ttu-id="5ebe3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebe3-158">Int32</span></span>|<span data-ttu-id="5ebe3-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-159">Version of the device configuration.</span></span> <span data-ttu-id="5ebe3-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5ebe3-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5ebe3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5ebe3-161">passwordRequired</span></span>|<span data-ttu-id="5ebe3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-162">Boolean</span></span>|<span data-ttu-id="5ebe3-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="5ebe3-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5ebe3-164">passwordMinimumLength</span></span>|<span data-ttu-id="5ebe3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebe3-165">Int32</span></span>|<span data-ttu-id="5ebe3-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-166">Minimum password length.</span></span> <span data-ttu-id="5ebe3-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="5ebe3-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5ebe3-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5ebe3-168">passwordRequiredType</span></span>|[<span data-ttu-id="5ebe3-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5ebe3-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="5ebe3-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-170">Type of characters in password.</span></span> <span data-ttu-id="5ebe3-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="5ebe3-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5ebe3-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5ebe3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebe3-173">Int32</span></span>|<span data-ttu-id="5ebe3-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5ebe3-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5ebe3-175">passwordExpirationDays</span></span>|<span data-ttu-id="5ebe3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebe3-176">Int32</span></span>|<span data-ttu-id="5ebe3-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-177">Number of days before the password expires.</span></span> <span data-ttu-id="5ebe3-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="5ebe3-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5ebe3-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5ebe3-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5ebe3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebe3-180">Int32</span></span>|<span data-ttu-id="5ebe3-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-181">Number of previous passwords to block.</span></span> <span data-ttu-id="5ebe3-182">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="5ebe3-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5ebe3-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5ebe3-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5ebe3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebe3-184">Int32</span></span>|<span data-ttu-id="5ebe3-185">Número de falhas de login permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="5ebe3-186">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5ebe3-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5ebe3-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5ebe3-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="5ebe3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-188">Boolean</span></span>|<span data-ttu-id="5ebe3-189">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="5ebe3-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="5ebe3-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="5ebe3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-191">Boolean</span></span>|<span data-ttu-id="5ebe3-192">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="5ebe3-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5ebe3-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="5ebe3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-194">Boolean</span></span>|<span data-ttu-id="5ebe3-195">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="5ebe3-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5ebe3-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5ebe3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-197">Boolean</span></span>|<span data-ttu-id="5ebe3-198">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5ebe3-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5ebe3-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5ebe3-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="5ebe3-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5ebe3-201">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5ebe3-202">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5ebe3-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="5ebe3-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="5ebe3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-204">Boolean</span></span>|<span data-ttu-id="5ebe3-205">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="5ebe3-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5ebe3-206">osMinimumVersion</span></span>|<span data-ttu-id="5ebe3-207">String</span><span class="sxs-lookup"><span data-stu-id="5ebe3-207">String</span></span>|<span data-ttu-id="5ebe3-208">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-208">Minimum Android version.</span></span>|
|<span data-ttu-id="5ebe3-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5ebe3-209">osMaximumVersion</span></span>|<span data-ttu-id="5ebe3-210">String</span><span class="sxs-lookup"><span data-stu-id="5ebe3-210">String</span></span>|<span data-ttu-id="5ebe3-211">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-211">Maximum Android version.</span></span>|
|<span data-ttu-id="5ebe3-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5ebe3-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="5ebe3-213">String</span><span class="sxs-lookup"><span data-stu-id="5ebe3-213">String</span></span>|<span data-ttu-id="5ebe3-214">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="5ebe3-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5ebe3-215">storageRequireEncryption</span></span>|<span data-ttu-id="5ebe3-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-216">Boolean</span></span>|<span data-ttu-id="5ebe3-217">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="5ebe3-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="5ebe3-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="5ebe3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-219">Boolean</span></span>|<span data-ttu-id="5ebe3-220">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="5ebe3-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="5ebe3-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="5ebe3-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-222">Boolean</span></span>|<span data-ttu-id="5ebe3-223">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="5ebe3-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="5ebe3-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="5ebe3-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-225">Boolean</span></span>|<span data-ttu-id="5ebe3-226">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="5ebe3-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="5ebe3-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="5ebe3-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-228">Boolean</span></span>|<span data-ttu-id="5ebe3-229">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="5ebe3-230">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="5ebe3-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="5ebe3-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="5ebe3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebe3-232">Boolean</span></span>|<span data-ttu-id="5ebe3-233">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="5ebe3-234">securityRequiredAndroidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="5ebe3-234">securityRequiredAndroidSafetyNetEvaluationType</span></span>|[<span data-ttu-id="5ebe3-235">androidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="5ebe3-235">androidSafetyNetEvaluationType</span></span>](../resources/intune-deviceconfig-androidsafetynetevaluationtype.md)|<span data-ttu-id="5ebe3-236">Exigir um tipo de avaliação SafetyNet específico para conformidade.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-236">Require a specific SafetyNet evaluation type for compliance.</span></span> <span data-ttu-id="5ebe3-237">Os valores possíveis são: `basic` e `hardwareBacked`.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-237">Possible values are: `basic`, `hardwareBacked`.</span></span>|



## <a name="response"></a><span data-ttu-id="5ebe3-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebe3-238">Response</span></span>
<span data-ttu-id="5ebe3-239">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-239">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebe3-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ebe3-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ebe3-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebe3-241">Request</span></span>
<span data-ttu-id="5ebe3-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1354

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
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```

### <a name="response"></a><span data-ttu-id="5ebe3-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebe3-243">Response</span></span>
<span data-ttu-id="5ebe3-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebe3-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1526

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
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```




