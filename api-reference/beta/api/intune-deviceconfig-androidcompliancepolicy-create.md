---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00090c3628bc419da35815a32d8bc3def6a2c62d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028116"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="083ad-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="083ad-103">Create androidCompliancePolicy</span></span>

<span data-ttu-id="083ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="083ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="083ad-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="083ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="083ad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="083ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="083ad-107">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="083ad-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="083ad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="083ad-108">Prerequisites</span></span>
<span data-ttu-id="083ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="083ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="083ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="083ad-111">Permission type</span></span>|<span data-ttu-id="083ad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="083ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="083ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="083ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="083ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="083ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="083ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="083ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="083ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="083ad-116">Not supported.</span></span>|
|<span data-ttu-id="083ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="083ad-117">Application</span></span>|<span data-ttu-id="083ad-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="083ad-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="083ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="083ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="083ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="083ad-120">Request headers</span></span>
|<span data-ttu-id="083ad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="083ad-121">Header</span></span>|<span data-ttu-id="083ad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="083ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="083ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="083ad-123">Authorization</span></span>|<span data-ttu-id="083ad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="083ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="083ad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="083ad-125">Accept</span></span>|<span data-ttu-id="083ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="083ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="083ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="083ad-127">Request body</span></span>
<span data-ttu-id="083ad-128">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="083ad-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="083ad-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="083ad-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="083ad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="083ad-130">Property</span></span>|<span data-ttu-id="083ad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="083ad-131">Type</span></span>|<span data-ttu-id="083ad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="083ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="083ad-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="083ad-133">roleScopeTagIds</span></span>|<span data-ttu-id="083ad-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="083ad-134">String collection</span></span>|<span data-ttu-id="083ad-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="083ad-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="083ad-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-137">id</span><span class="sxs-lookup"><span data-stu-id="083ad-137">id</span></span>|<span data-ttu-id="083ad-138">String</span><span class="sxs-lookup"><span data-stu-id="083ad-138">String</span></span>|<span data-ttu-id="083ad-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="083ad-139">Key of the entity.</span></span> <span data-ttu-id="083ad-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="083ad-141">createdDateTime</span></span>|<span data-ttu-id="083ad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="083ad-142">DateTimeOffset</span></span>|<span data-ttu-id="083ad-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="083ad-143">DateTime the object was created.</span></span> <span data-ttu-id="083ad-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-145">description</span><span class="sxs-lookup"><span data-stu-id="083ad-145">description</span></span>|<span data-ttu-id="083ad-146">String</span><span class="sxs-lookup"><span data-stu-id="083ad-146">String</span></span>|<span data-ttu-id="083ad-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="083ad-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="083ad-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="083ad-149">lastModifiedDateTime</span></span>|<span data-ttu-id="083ad-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="083ad-150">DateTimeOffset</span></span>|<span data-ttu-id="083ad-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="083ad-151">DateTime the object was last modified.</span></span> <span data-ttu-id="083ad-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-153">displayName</span><span class="sxs-lookup"><span data-stu-id="083ad-153">displayName</span></span>|<span data-ttu-id="083ad-154">String</span><span class="sxs-lookup"><span data-stu-id="083ad-154">String</span></span>|<span data-ttu-id="083ad-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="083ad-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="083ad-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-157">version</span><span class="sxs-lookup"><span data-stu-id="083ad-157">version</span></span>|<span data-ttu-id="083ad-158">Int32</span><span class="sxs-lookup"><span data-stu-id="083ad-158">Int32</span></span>|<span data-ttu-id="083ad-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="083ad-159">Version of the device configuration.</span></span> <span data-ttu-id="083ad-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="083ad-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="083ad-161">passwordRequired</span></span>|<span data-ttu-id="083ad-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-162">Boolean</span></span>|<span data-ttu-id="083ad-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="083ad-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="083ad-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="083ad-164">passwordMinimumLength</span></span>|<span data-ttu-id="083ad-165">Int32</span><span class="sxs-lookup"><span data-stu-id="083ad-165">Int32</span></span>|<span data-ttu-id="083ad-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="083ad-166">Minimum password length.</span></span> <span data-ttu-id="083ad-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="083ad-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="083ad-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="083ad-168">passwordRequiredType</span></span>|[<span data-ttu-id="083ad-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="083ad-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="083ad-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="083ad-170">Type of characters in password.</span></span> <span data-ttu-id="083ad-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="083ad-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="083ad-172">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="083ad-172">requiredPasswordComplexity</span></span>|[<span data-ttu-id="083ad-173">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="083ad-173">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="083ad-174">Indica a complexidade da senha necessária no Android.</span><span class="sxs-lookup"><span data-stu-id="083ad-174">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="083ad-175">Um de: nenhum, baixo, médio, alto.</span><span class="sxs-lookup"><span data-stu-id="083ad-175">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="083ad-176">Esta é uma nova API voltada para o Android 11 +.</span><span class="sxs-lookup"><span data-stu-id="083ad-176">This is a new API targeted to Android 11+.</span></span> <span data-ttu-id="083ad-177">Os valores possíveis são: `none`, `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="083ad-177">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="083ad-178">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="083ad-178">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="083ad-179">Int32</span><span class="sxs-lookup"><span data-stu-id="083ad-179">Int32</span></span>|<span data-ttu-id="083ad-180">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="083ad-180">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="083ad-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="083ad-181">passwordExpirationDays</span></span>|<span data-ttu-id="083ad-182">Int32</span><span class="sxs-lookup"><span data-stu-id="083ad-182">Int32</span></span>|<span data-ttu-id="083ad-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="083ad-183">Number of days before the password expires.</span></span> <span data-ttu-id="083ad-184">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="083ad-184">Valid values 1 to 365</span></span>|
|<span data-ttu-id="083ad-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="083ad-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="083ad-186">Int32</span><span class="sxs-lookup"><span data-stu-id="083ad-186">Int32</span></span>|<span data-ttu-id="083ad-187">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="083ad-187">Number of previous passwords to block.</span></span> <span data-ttu-id="083ad-188">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="083ad-188">Valid values 1 to 24</span></span>|
|<span data-ttu-id="083ad-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="083ad-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="083ad-190">Int32</span><span class="sxs-lookup"><span data-stu-id="083ad-190">Int32</span></span>|<span data-ttu-id="083ad-191">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="083ad-191">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="083ad-192">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="083ad-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="083ad-193">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="083ad-193">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="083ad-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-194">Boolean</span></span>|<span data-ttu-id="083ad-195">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="083ad-195">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="083ad-196">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="083ad-196">securityDisableUsbDebugging</span></span>|<span data-ttu-id="083ad-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-197">Boolean</span></span>|<span data-ttu-id="083ad-198">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="083ad-198">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="083ad-199">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="083ad-199">securityRequireVerifyApps</span></span>|<span data-ttu-id="083ad-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-200">Boolean</span></span>|<span data-ttu-id="083ad-201">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="083ad-201">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="083ad-202">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="083ad-202">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="083ad-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-203">Boolean</span></span>|<span data-ttu-id="083ad-204">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="083ad-204">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="083ad-205">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="083ad-205">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="083ad-206">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="083ad-206">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="083ad-207">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="083ad-207">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="083ad-208">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="083ad-208">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="083ad-209">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="083ad-209">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="083ad-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="083ad-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="083ad-211">MDATP requer nível mínimo de risco de proteção contra ameaças móveis para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="083ad-211">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="083ad-212">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="083ad-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="083ad-213">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="083ad-213">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="083ad-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-214">Boolean</span></span>|<span data-ttu-id="083ad-215">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="083ad-215">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="083ad-216">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="083ad-216">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="083ad-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="083ad-217">Boolean</span></span>|<span data-ttu-id="083ad-218">Bloquear dispositivos gerenciados pelo administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="083ad-218">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="083ad-219">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="083ad-219">osMinimumVersion</span></span>|<span data-ttu-id="083ad-220">String</span><span class="sxs-lookup"><span data-stu-id="083ad-220">String</span></span>|<span data-ttu-id="083ad-221">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="083ad-221">Minimum Android version.</span></span>|
|<span data-ttu-id="083ad-222">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="083ad-222">osMaximumVersion</span></span>|<span data-ttu-id="083ad-223">String</span><span class="sxs-lookup"><span data-stu-id="083ad-223">String</span></span>|<span data-ttu-id="083ad-224">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="083ad-224">Maximum Android version.</span></span>|
|<span data-ttu-id="083ad-225">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="083ad-225">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="083ad-226">String</span><span class="sxs-lookup"><span data-stu-id="083ad-226">String</span></span>|<span data-ttu-id="083ad-227">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="083ad-227">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="083ad-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="083ad-228">storageRequireEncryption</span></span>|<span data-ttu-id="083ad-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-229">Boolean</span></span>|<span data-ttu-id="083ad-230">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="083ad-230">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="083ad-231">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="083ad-231">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="083ad-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-232">Boolean</span></span>|<span data-ttu-id="083ad-233">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="083ad-233">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="083ad-234">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="083ad-234">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="083ad-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-235">Boolean</span></span>|<span data-ttu-id="083ad-236">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="083ad-236">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="083ad-237">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="083ad-237">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="083ad-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-238">Boolean</span></span>|<span data-ttu-id="083ad-239">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="083ad-239">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="083ad-240">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="083ad-240">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="083ad-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-241">Boolean</span></span>|<span data-ttu-id="083ad-242">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="083ad-242">Require the device to have up to date security providers.</span></span> <span data-ttu-id="083ad-243">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="083ad-243">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="083ad-244">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="083ad-244">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="083ad-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="083ad-245">Boolean</span></span>|<span data-ttu-id="083ad-246">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="083ad-246">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="083ad-247">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="083ad-247">conditionStatementId</span></span>|<span data-ttu-id="083ad-248">String</span><span class="sxs-lookup"><span data-stu-id="083ad-248">String</span></span>|<span data-ttu-id="083ad-249">ID da instrução de condição.</span><span class="sxs-lookup"><span data-stu-id="083ad-249">Condition statement id.</span></span>|
|<span data-ttu-id="083ad-250">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="083ad-250">restrictedApps</span></span>|<span data-ttu-id="083ad-251">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="083ad-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="083ad-252">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="083ad-252">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="083ad-253">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="083ad-253">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="083ad-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="083ad-254">Response</span></span>
<span data-ttu-id="083ad-255">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="083ad-255">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="083ad-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="083ad-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="083ad-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="083ad-257">Request</span></span>
<span data-ttu-id="083ad-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="083ad-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="083ad-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="083ad-259">Response</span></span>
<span data-ttu-id="083ad-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="083ad-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






