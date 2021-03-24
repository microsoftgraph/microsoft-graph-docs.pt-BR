---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8affcd773474c025acf0371f96bb401b1dcad17f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126791"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="42d2a-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="42d2a-103">Create androidCompliancePolicy</span></span>

<span data-ttu-id="42d2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42d2a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42d2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42d2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42d2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d2a-107">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="42d2a-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42d2a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42d2a-108">Prerequisites</span></span>
<span data-ttu-id="42d2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42d2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42d2a-111">Permission type</span></span>|<span data-ttu-id="42d2a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42d2a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42d2a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42d2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42d2a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d2a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42d2a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42d2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42d2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d2a-116">Not supported.</span></span>|
|<span data-ttu-id="42d2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d2a-117">Application</span></span>|<span data-ttu-id="42d2a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d2a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42d2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42d2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="42d2a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42d2a-120">Request headers</span></span>
|<span data-ttu-id="42d2a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42d2a-121">Header</span></span>|<span data-ttu-id="42d2a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42d2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42d2a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42d2a-123">Authorization</span></span>|<span data-ttu-id="42d2a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42d2a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42d2a-125">Accept</span></span>|<span data-ttu-id="42d2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42d2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42d2a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42d2a-127">Request body</span></span>
<span data-ttu-id="42d2a-128">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="42d2a-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="42d2a-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="42d2a-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="42d2a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42d2a-130">Property</span></span>|<span data-ttu-id="42d2a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d2a-131">Type</span></span>|<span data-ttu-id="42d2a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d2a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42d2a-133">roleScopeTagIds</span></span>|<span data-ttu-id="42d2a-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d2a-134">String collection</span></span>|<span data-ttu-id="42d2a-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="42d2a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42d2a-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-137">id</span><span class="sxs-lookup"><span data-stu-id="42d2a-137">id</span></span>|<span data-ttu-id="42d2a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d2a-138">String</span></span>|<span data-ttu-id="42d2a-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42d2a-139">Key of the entity.</span></span> <span data-ttu-id="42d2a-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42d2a-141">createdDateTime</span></span>|<span data-ttu-id="42d2a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42d2a-142">DateTimeOffset</span></span>|<span data-ttu-id="42d2a-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="42d2a-143">DateTime the object was created.</span></span> <span data-ttu-id="42d2a-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-145">descrição</span><span class="sxs-lookup"><span data-stu-id="42d2a-145">description</span></span>|<span data-ttu-id="42d2a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d2a-146">String</span></span>|<span data-ttu-id="42d2a-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42d2a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42d2a-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42d2a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="42d2a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42d2a-150">DateTimeOffset</span></span>|<span data-ttu-id="42d2a-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="42d2a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="42d2a-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="42d2a-153">displayName</span></span>|<span data-ttu-id="42d2a-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d2a-154">String</span></span>|<span data-ttu-id="42d2a-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42d2a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42d2a-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-157">version</span><span class="sxs-lookup"><span data-stu-id="42d2a-157">version</span></span>|<span data-ttu-id="42d2a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="42d2a-158">Int32</span></span>|<span data-ttu-id="42d2a-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42d2a-159">Version of the device configuration.</span></span> <span data-ttu-id="42d2a-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42d2a-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="42d2a-161">passwordRequired</span></span>|<span data-ttu-id="42d2a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-162">Boolean</span></span>|<span data-ttu-id="42d2a-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42d2a-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="42d2a-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42d2a-164">passwordMinimumLength</span></span>|<span data-ttu-id="42d2a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="42d2a-165">Int32</span></span>|<span data-ttu-id="42d2a-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="42d2a-166">Minimum password length.</span></span> <span data-ttu-id="42d2a-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="42d2a-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="42d2a-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="42d2a-168">passwordRequiredType</span></span>|[<span data-ttu-id="42d2a-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="42d2a-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="42d2a-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="42d2a-170">Type of characters in password.</span></span> <span data-ttu-id="42d2a-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="42d2a-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="42d2a-172">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="42d2a-172">requiredPasswordComplexity</span></span>|[<span data-ttu-id="42d2a-173">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="42d2a-173">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="42d2a-174">Indica a complexidade de senha necessária no Android.</span><span class="sxs-lookup"><span data-stu-id="42d2a-174">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="42d2a-175">Um deles: NONE, LOW, MEDIUM, HIGH.</span><span class="sxs-lookup"><span data-stu-id="42d2a-175">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="42d2a-176">Esta é uma nova API direcionada ao Android 11+.</span><span class="sxs-lookup"><span data-stu-id="42d2a-176">This is a new API targeted to Android 11+.</span></span> <span data-ttu-id="42d2a-177">Os valores possíveis são: `none`, `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="42d2a-177">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="42d2a-178">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="42d2a-178">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="42d2a-179">Int32</span><span class="sxs-lookup"><span data-stu-id="42d2a-179">Int32</span></span>|<span data-ttu-id="42d2a-180">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="42d2a-180">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="42d2a-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="42d2a-181">passwordExpirationDays</span></span>|<span data-ttu-id="42d2a-182">Int32</span><span class="sxs-lookup"><span data-stu-id="42d2a-182">Int32</span></span>|<span data-ttu-id="42d2a-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="42d2a-183">Number of days before the password expires.</span></span> <span data-ttu-id="42d2a-184">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="42d2a-184">Valid values 1 to 365</span></span>|
|<span data-ttu-id="42d2a-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="42d2a-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="42d2a-186">Int32</span><span class="sxs-lookup"><span data-stu-id="42d2a-186">Int32</span></span>|<span data-ttu-id="42d2a-187">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="42d2a-187">Number of previous passwords to block.</span></span> <span data-ttu-id="42d2a-188">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="42d2a-188">Valid values 1 to 24</span></span>|
|<span data-ttu-id="42d2a-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="42d2a-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="42d2a-190">Int32</span><span class="sxs-lookup"><span data-stu-id="42d2a-190">Int32</span></span>|<span data-ttu-id="42d2a-191">Número de falhas de login permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="42d2a-191">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="42d2a-192">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="42d2a-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="42d2a-193">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="42d2a-193">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="42d2a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-194">Boolean</span></span>|<span data-ttu-id="42d2a-195">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="42d2a-195">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="42d2a-196">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="42d2a-196">securityDisableUsbDebugging</span></span>|<span data-ttu-id="42d2a-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-197">Boolean</span></span>|<span data-ttu-id="42d2a-198">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="42d2a-198">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="42d2a-199">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="42d2a-199">securityRequireVerifyApps</span></span>|<span data-ttu-id="42d2a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-200">Boolean</span></span>|<span data-ttu-id="42d2a-201">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="42d2a-201">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="42d2a-202">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="42d2a-202">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="42d2a-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-203">Boolean</span></span>|<span data-ttu-id="42d2a-204">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="42d2a-204">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="42d2a-205">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="42d2a-205">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="42d2a-206">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="42d2a-206">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="42d2a-207">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="42d2a-207">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="42d2a-208">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="42d2a-208">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="42d2a-209">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="42d2a-209">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="42d2a-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="42d2a-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="42d2a-211">O MDATP exige nível mínimo de risco da Proteção Contra Ameaças Móveis para relatar o não-atendimento.</span><span class="sxs-lookup"><span data-stu-id="42d2a-211">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="42d2a-212">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="42d2a-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="42d2a-213">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="42d2a-213">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="42d2a-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-214">Boolean</span></span>|<span data-ttu-id="42d2a-215">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="42d2a-215">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="42d2a-216">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="42d2a-216">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="42d2a-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="42d2a-217">Boolean</span></span>|<span data-ttu-id="42d2a-218">Bloquear dispositivos gerenciados pelo administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="42d2a-218">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="42d2a-219">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="42d2a-219">osMinimumVersion</span></span>|<span data-ttu-id="42d2a-220">String</span><span class="sxs-lookup"><span data-stu-id="42d2a-220">String</span></span>|<span data-ttu-id="42d2a-221">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="42d2a-221">Minimum Android version.</span></span>|
|<span data-ttu-id="42d2a-222">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="42d2a-222">osMaximumVersion</span></span>|<span data-ttu-id="42d2a-223">String</span><span class="sxs-lookup"><span data-stu-id="42d2a-223">String</span></span>|<span data-ttu-id="42d2a-224">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="42d2a-224">Maximum Android version.</span></span>|
|<span data-ttu-id="42d2a-225">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="42d2a-225">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="42d2a-226">String</span><span class="sxs-lookup"><span data-stu-id="42d2a-226">String</span></span>|<span data-ttu-id="42d2a-227">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="42d2a-227">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="42d2a-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="42d2a-228">storageRequireEncryption</span></span>|<span data-ttu-id="42d2a-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-229">Boolean</span></span>|<span data-ttu-id="42d2a-230">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="42d2a-230">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="42d2a-231">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="42d2a-231">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="42d2a-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-232">Boolean</span></span>|<span data-ttu-id="42d2a-233">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="42d2a-233">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="42d2a-234">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="42d2a-234">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="42d2a-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-235">Boolean</span></span>|<span data-ttu-id="42d2a-236">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="42d2a-236">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="42d2a-237">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="42d2a-237">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="42d2a-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-238">Boolean</span></span>|<span data-ttu-id="42d2a-239">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42d2a-239">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="42d2a-240">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="42d2a-240">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="42d2a-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-241">Boolean</span></span>|<span data-ttu-id="42d2a-242">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="42d2a-242">Require the device to have up to date security providers.</span></span> <span data-ttu-id="42d2a-243">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="42d2a-243">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="42d2a-244">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="42d2a-244">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="42d2a-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2a-245">Boolean</span></span>|<span data-ttu-id="42d2a-246">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="42d2a-246">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="42d2a-247">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="42d2a-247">conditionStatementId</span></span>|<span data-ttu-id="42d2a-248">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d2a-248">String</span></span>|<span data-ttu-id="42d2a-249">ID da instrução Condition.</span><span class="sxs-lookup"><span data-stu-id="42d2a-249">Condition statement id.</span></span>|
|<span data-ttu-id="42d2a-250">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="42d2a-250">restrictedApps</span></span>|<span data-ttu-id="42d2a-251">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="42d2a-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="42d2a-252">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="42d2a-252">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="42d2a-253">Essa coleção pode conter no máximo 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="42d2a-253">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="42d2a-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d2a-254">Response</span></span>
<span data-ttu-id="42d2a-255">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42d2a-255">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42d2a-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42d2a-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="42d2a-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42d2a-257">Request</span></span>
<span data-ttu-id="42d2a-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d2a-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1750

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
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
  "securityBlockDeviceAdministratorManagedDevices": true,
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

### <a name="response"></a><span data-ttu-id="42d2a-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d2a-259">Response</span></span>
<span data-ttu-id="42d2a-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42d2a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1922

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
  "requiredPasswordComplexity": "low",
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
  "securityBlockDeviceAdministratorManagedDevices": true,
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




