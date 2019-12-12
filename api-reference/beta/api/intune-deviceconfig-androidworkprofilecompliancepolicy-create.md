---
title: Criar na entidadeandroidworkprofilecompliancepolicy
description: Criar um novo objeto na entidadeandroidworkprofilecompliancepolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1c545afa13d241e3dcd9c3d54de77d8736ad7ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954654"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="7d984-103">Criar na entidadeandroidworkprofilecompliancepolicy</span><span class="sxs-lookup"><span data-stu-id="7d984-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="7d984-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d984-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d984-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d984-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d984-106">Criar um novo objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7d984-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d984-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d984-107">Prerequisites</span></span>
<span data-ttu-id="7d984-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d984-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d984-110">Permission type</span></span>|<span data-ttu-id="7d984-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d984-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d984-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d984-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d984-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d984-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d984-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d984-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d984-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d984-115">Not supported.</span></span>|
|<span data-ttu-id="7d984-116">Application</span><span class="sxs-lookup"><span data-stu-id="7d984-116">Application</span></span>|<span data-ttu-id="7d984-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d984-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d984-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d984-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7d984-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d984-119">Request headers</span></span>
|<span data-ttu-id="7d984-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d984-120">Header</span></span>|<span data-ttu-id="7d984-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d984-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d984-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d984-122">Authorization</span></span>|<span data-ttu-id="7d984-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d984-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d984-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d984-124">Accept</span></span>|<span data-ttu-id="7d984-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d984-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d984-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d984-126">Request body</span></span>
<span data-ttu-id="7d984-127">No corpo da solicitação, forneça uma representação JSON do objeto na entidadeandroidworkprofilecompliancepolicy.</span><span class="sxs-lookup"><span data-stu-id="7d984-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="7d984-128">A tabela a seguir mostra as propriedades que são necessárias ao criar na entidadeandroidworkprofilecompliancepolicy.</span><span class="sxs-lookup"><span data-stu-id="7d984-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="7d984-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d984-129">Property</span></span>|<span data-ttu-id="7d984-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d984-130">Type</span></span>|<span data-ttu-id="7d984-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d984-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d984-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d984-132">roleScopeTagIds</span></span>|<span data-ttu-id="7d984-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d984-133">String collection</span></span>|<span data-ttu-id="7d984-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7d984-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d984-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-136">id</span><span class="sxs-lookup"><span data-stu-id="7d984-136">id</span></span>|<span data-ttu-id="7d984-137">String</span><span class="sxs-lookup"><span data-stu-id="7d984-137">String</span></span>|<span data-ttu-id="7d984-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d984-138">Key of the entity.</span></span> <span data-ttu-id="7d984-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d984-140">createdDateTime</span></span>|<span data-ttu-id="7d984-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d984-141">DateTimeOffset</span></span>|<span data-ttu-id="7d984-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7d984-142">DateTime the object was created.</span></span> <span data-ttu-id="7d984-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-144">description</span><span class="sxs-lookup"><span data-stu-id="7d984-144">description</span></span>|<span data-ttu-id="7d984-145">String</span><span class="sxs-lookup"><span data-stu-id="7d984-145">String</span></span>|<span data-ttu-id="7d984-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d984-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d984-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d984-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7d984-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d984-149">DateTimeOffset</span></span>|<span data-ttu-id="7d984-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7d984-150">DateTime the object was last modified.</span></span> <span data-ttu-id="7d984-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-152">displayName</span><span class="sxs-lookup"><span data-stu-id="7d984-152">displayName</span></span>|<span data-ttu-id="7d984-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d984-153">String</span></span>|<span data-ttu-id="7d984-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d984-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d984-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-156">version</span><span class="sxs-lookup"><span data-stu-id="7d984-156">version</span></span>|<span data-ttu-id="7d984-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7d984-157">Int32</span></span>|<span data-ttu-id="7d984-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d984-158">Version of the device configuration.</span></span> <span data-ttu-id="7d984-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d984-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d984-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7d984-160">passwordRequired</span></span>|<span data-ttu-id="7d984-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-161">Boolean</span></span>|<span data-ttu-id="7d984-162">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d984-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="7d984-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7d984-163">passwordMinimumLength</span></span>|<span data-ttu-id="7d984-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7d984-164">Int32</span></span>|<span data-ttu-id="7d984-165">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="7d984-165">Minimum password length.</span></span> <span data-ttu-id="7d984-166">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="7d984-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7d984-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7d984-167">passwordRequiredType</span></span>|[<span data-ttu-id="7d984-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7d984-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="7d984-169">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="7d984-169">Type of characters in password.</span></span> <span data-ttu-id="7d984-170">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="7d984-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="7d984-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7d984-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7d984-172">Int32</span><span class="sxs-lookup"><span data-stu-id="7d984-172">Int32</span></span>|<span data-ttu-id="7d984-173">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="7d984-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7d984-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7d984-174">passwordExpirationDays</span></span>|<span data-ttu-id="7d984-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7d984-175">Int32</span></span>|<span data-ttu-id="7d984-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="7d984-176">Number of days before the password expires.</span></span> <span data-ttu-id="7d984-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="7d984-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7d984-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7d984-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7d984-179">Int32</span><span class="sxs-lookup"><span data-stu-id="7d984-179">Int32</span></span>|<span data-ttu-id="7d984-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="7d984-180">Number of previous passwords to block.</span></span> <span data-ttu-id="7d984-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="7d984-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7d984-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7d984-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7d984-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7d984-183">Int32</span></span>|<span data-ttu-id="7d984-184">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="7d984-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="7d984-185">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="7d984-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7d984-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="7d984-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="7d984-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-187">Boolean</span></span>|<span data-ttu-id="7d984-188">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="7d984-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="7d984-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="7d984-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="7d984-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-190">Boolean</span></span>|<span data-ttu-id="7d984-191">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="7d984-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="7d984-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7d984-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="7d984-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-193">Boolean</span></span>|<span data-ttu-id="7d984-194">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="7d984-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="7d984-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7d984-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="7d984-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-196">Boolean</span></span>|<span data-ttu-id="7d984-197">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="7d984-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="7d984-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7d984-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7d984-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="7d984-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7d984-200">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="7d984-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7d984-201">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7d984-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7d984-202">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7d984-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7d984-203">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="7d984-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7d984-204">MDATP requer nível mínimo de risco de proteção contra ameaças móveis para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="7d984-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7d984-205">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7d984-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7d984-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="7d984-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="7d984-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-207">Boolean</span></span>|<span data-ttu-id="7d984-208">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="7d984-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="7d984-209">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7d984-209">osMinimumVersion</span></span>|<span data-ttu-id="7d984-210">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d984-210">String</span></span>|<span data-ttu-id="7d984-211">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="7d984-211">Minimum Android version.</span></span>|
|<span data-ttu-id="7d984-212">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7d984-212">osMaximumVersion</span></span>|<span data-ttu-id="7d984-213">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d984-213">String</span></span>|<span data-ttu-id="7d984-214">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="7d984-214">Maximum Android version.</span></span>|
|<span data-ttu-id="7d984-215">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="7d984-215">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="7d984-216">String</span><span class="sxs-lookup"><span data-stu-id="7d984-216">String</span></span>|<span data-ttu-id="7d984-217">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="7d984-217">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="7d984-218">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7d984-218">storageRequireEncryption</span></span>|<span data-ttu-id="7d984-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-219">Boolean</span></span>|<span data-ttu-id="7d984-220">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="7d984-220">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="7d984-221">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="7d984-221">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="7d984-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-222">Boolean</span></span>|<span data-ttu-id="7d984-223">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="7d984-223">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="7d984-224">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="7d984-224">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="7d984-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-225">Boolean</span></span>|<span data-ttu-id="7d984-226">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="7d984-226">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="7d984-227">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="7d984-227">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="7d984-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-228">Boolean</span></span>|<span data-ttu-id="7d984-229">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d984-229">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="7d984-230">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="7d984-230">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="7d984-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-231">Boolean</span></span>|<span data-ttu-id="7d984-232">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="7d984-232">Require the device to have up to date security providers.</span></span> <span data-ttu-id="7d984-233">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="7d984-233">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="7d984-234">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="7d984-234">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="7d984-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d984-235">Boolean</span></span>|<span data-ttu-id="7d984-236">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="7d984-236">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="7d984-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d984-237">Response</span></span>
<span data-ttu-id="7d984-238">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [na entidadeandroidworkprofilecompliancepolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d984-238">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d984-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d984-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d984-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d984-240">Request</span></span>
<span data-ttu-id="7d984-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d984-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1350

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
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="7d984-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d984-242">Response</span></span>
<span data-ttu-id="7d984-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d984-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1522

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
  "securityRequireCompanyPortalAppIntegrity": true
}
```





