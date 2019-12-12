---
title: Criar androidCompliancePolicy
description: Cria um novo objeto androidCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97b16113f9b963e39814eec405471a8884c2c334
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954255"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="3147d-103">Criar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3147d-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="3147d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3147d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3147d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3147d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3147d-106">Cria um novo objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3147d-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3147d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3147d-107">Prerequisites</span></span>
<span data-ttu-id="3147d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3147d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3147d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3147d-110">Permission type</span></span>|<span data-ttu-id="3147d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3147d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3147d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3147d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3147d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3147d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3147d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3147d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3147d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3147d-115">Not supported.</span></span>|
|<span data-ttu-id="3147d-116">Application</span><span class="sxs-lookup"><span data-stu-id="3147d-116">Application</span></span>|<span data-ttu-id="3147d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3147d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3147d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3147d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3147d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3147d-119">Request headers</span></span>
|<span data-ttu-id="3147d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3147d-120">Header</span></span>|<span data-ttu-id="3147d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3147d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3147d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3147d-122">Authorization</span></span>|<span data-ttu-id="3147d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3147d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3147d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3147d-124">Accept</span></span>|<span data-ttu-id="3147d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3147d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3147d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3147d-126">Request body</span></span>
<span data-ttu-id="3147d-127">No corpo da solicitação, forneça uma representação JSON do objeto androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3147d-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="3147d-128">A tabela a seguir mostra as propriedades obrigatórias ao criar androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3147d-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="3147d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3147d-129">Property</span></span>|<span data-ttu-id="3147d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3147d-130">Type</span></span>|<span data-ttu-id="3147d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3147d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3147d-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3147d-132">roleScopeTagIds</span></span>|<span data-ttu-id="3147d-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3147d-133">String collection</span></span>|<span data-ttu-id="3147d-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3147d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3147d-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-136">id</span><span class="sxs-lookup"><span data-stu-id="3147d-136">id</span></span>|<span data-ttu-id="3147d-137">String</span><span class="sxs-lookup"><span data-stu-id="3147d-137">String</span></span>|<span data-ttu-id="3147d-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3147d-138">Key of the entity.</span></span> <span data-ttu-id="3147d-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3147d-140">createdDateTime</span></span>|<span data-ttu-id="3147d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3147d-141">DateTimeOffset</span></span>|<span data-ttu-id="3147d-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3147d-142">DateTime the object was created.</span></span> <span data-ttu-id="3147d-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-144">description</span><span class="sxs-lookup"><span data-stu-id="3147d-144">description</span></span>|<span data-ttu-id="3147d-145">String</span><span class="sxs-lookup"><span data-stu-id="3147d-145">String</span></span>|<span data-ttu-id="3147d-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3147d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3147d-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3147d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3147d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3147d-149">DateTimeOffset</span></span>|<span data-ttu-id="3147d-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3147d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="3147d-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="3147d-152">displayName</span></span>|<span data-ttu-id="3147d-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3147d-153">String</span></span>|<span data-ttu-id="3147d-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3147d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3147d-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-156">version</span><span class="sxs-lookup"><span data-stu-id="3147d-156">version</span></span>|<span data-ttu-id="3147d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3147d-157">Int32</span></span>|<span data-ttu-id="3147d-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3147d-158">Version of the device configuration.</span></span> <span data-ttu-id="3147d-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3147d-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3147d-160">passwordRequired</span></span>|<span data-ttu-id="3147d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-161">Boolean</span></span>|<span data-ttu-id="3147d-162">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3147d-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="3147d-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3147d-163">passwordMinimumLength</span></span>|<span data-ttu-id="3147d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3147d-164">Int32</span></span>|<span data-ttu-id="3147d-165">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="3147d-165">Minimum password length.</span></span> <span data-ttu-id="3147d-166">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="3147d-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3147d-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3147d-167">passwordRequiredType</span></span>|[<span data-ttu-id="3147d-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3147d-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="3147d-169">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="3147d-169">Type of characters in password.</span></span> <span data-ttu-id="3147d-170">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="3147d-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="3147d-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3147d-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3147d-172">Int32</span><span class="sxs-lookup"><span data-stu-id="3147d-172">Int32</span></span>|<span data-ttu-id="3147d-173">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="3147d-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3147d-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3147d-174">passwordExpirationDays</span></span>|<span data-ttu-id="3147d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="3147d-175">Int32</span></span>|<span data-ttu-id="3147d-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="3147d-176">Number of days before the password expires.</span></span> <span data-ttu-id="3147d-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="3147d-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3147d-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3147d-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3147d-179">Int32</span><span class="sxs-lookup"><span data-stu-id="3147d-179">Int32</span></span>|<span data-ttu-id="3147d-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="3147d-180">Number of previous passwords to block.</span></span> <span data-ttu-id="3147d-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="3147d-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3147d-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3147d-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3147d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="3147d-183">Int32</span></span>|<span data-ttu-id="3147d-184">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="3147d-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="3147d-185">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="3147d-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3147d-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="3147d-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="3147d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-187">Boolean</span></span>|<span data-ttu-id="3147d-188">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="3147d-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="3147d-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="3147d-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="3147d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-190">Boolean</span></span>|<span data-ttu-id="3147d-191">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="3147d-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="3147d-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3147d-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="3147d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-193">Boolean</span></span>|<span data-ttu-id="3147d-194">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="3147d-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="3147d-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3147d-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3147d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-196">Boolean</span></span>|<span data-ttu-id="3147d-197">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="3147d-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="3147d-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3147d-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3147d-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3147d-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3147d-200">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="3147d-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3147d-201">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3147d-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3147d-202">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3147d-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3147d-203">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3147d-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3147d-204">MDATP requer nível mínimo de risco de proteção contra ameaças móveis para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="3147d-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3147d-205">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3147d-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3147d-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="3147d-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="3147d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-207">Boolean</span></span>|<span data-ttu-id="3147d-208">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="3147d-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="3147d-209">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="3147d-209">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="3147d-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-210">Boolean</span></span>|<span data-ttu-id="3147d-211">Bloquear dispositivos gerenciados pelo administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3147d-211">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="3147d-212">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3147d-212">osMinimumVersion</span></span>|<span data-ttu-id="3147d-213">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3147d-213">String</span></span>|<span data-ttu-id="3147d-214">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="3147d-214">Minimum Android version.</span></span>|
|<span data-ttu-id="3147d-215">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3147d-215">osMaximumVersion</span></span>|<span data-ttu-id="3147d-216">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3147d-216">String</span></span>|<span data-ttu-id="3147d-217">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="3147d-217">Maximum Android version.</span></span>|
|<span data-ttu-id="3147d-218">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3147d-218">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="3147d-219">String</span><span class="sxs-lookup"><span data-stu-id="3147d-219">String</span></span>|<span data-ttu-id="3147d-220">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="3147d-220">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="3147d-221">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3147d-221">storageRequireEncryption</span></span>|<span data-ttu-id="3147d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-222">Boolean</span></span>|<span data-ttu-id="3147d-223">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="3147d-223">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="3147d-224">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="3147d-224">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="3147d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-225">Boolean</span></span>|<span data-ttu-id="3147d-226">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="3147d-226">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="3147d-227">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="3147d-227">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="3147d-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-228">Boolean</span></span>|<span data-ttu-id="3147d-229">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="3147d-229">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="3147d-230">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="3147d-230">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="3147d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-231">Boolean</span></span>|<span data-ttu-id="3147d-232">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3147d-232">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="3147d-233">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="3147d-233">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="3147d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-234">Boolean</span></span>|<span data-ttu-id="3147d-235">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="3147d-235">Require the device to have up to date security providers.</span></span> <span data-ttu-id="3147d-236">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="3147d-236">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="3147d-237">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="3147d-237">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="3147d-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="3147d-238">Boolean</span></span>|<span data-ttu-id="3147d-239">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="3147d-239">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="3147d-240">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="3147d-240">conditionStatementId</span></span>|<span data-ttu-id="3147d-241">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3147d-241">String</span></span>|<span data-ttu-id="3147d-242">ID da instrução de condição.</span><span class="sxs-lookup"><span data-stu-id="3147d-242">Condition statement id.</span></span>|
|<span data-ttu-id="3147d-243">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="3147d-243">restrictedApps</span></span>|<span data-ttu-id="3147d-244">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3147d-244">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3147d-245">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="3147d-245">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="3147d-246">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="3147d-246">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3147d-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="3147d-247">Response</span></span>
<span data-ttu-id="3147d-248">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3147d-248">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3147d-249">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3147d-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="3147d-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3147d-250">Request</span></span>
<span data-ttu-id="3147d-251">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3147d-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1710

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

### <a name="response"></a><span data-ttu-id="3147d-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="3147d-252">Response</span></span>
<span data-ttu-id="3147d-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3147d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1882

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





