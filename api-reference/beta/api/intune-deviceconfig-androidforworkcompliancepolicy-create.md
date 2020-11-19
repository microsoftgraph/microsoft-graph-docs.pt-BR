---
title: Criar androidForWorkCompliancePolicy
description: Criar um novo objeto androidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52e1f91df305ca5c3a5cf7ac8439a18345120d57
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49239687"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="d80f5-103">Criar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d80f5-103">Create androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="d80f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d80f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d80f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d80f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d80f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d80f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d80f5-107">Criar um novo objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d80f5-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d80f5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d80f5-108">Prerequisites</span></span>
<span data-ttu-id="d80f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d80f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d80f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d80f5-111">Permission type</span></span>|<span data-ttu-id="d80f5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d80f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d80f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d80f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d80f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d80f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d80f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d80f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d80f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d80f5-116">Not supported.</span></span>|
|<span data-ttu-id="d80f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d80f5-117">Application</span></span>|<span data-ttu-id="d80f5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d80f5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d80f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d80f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d80f5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d80f5-120">Request headers</span></span>
|<span data-ttu-id="d80f5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d80f5-121">Header</span></span>|<span data-ttu-id="d80f5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d80f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d80f5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d80f5-123">Authorization</span></span>|<span data-ttu-id="d80f5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d80f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d80f5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d80f5-125">Accept</span></span>|<span data-ttu-id="d80f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d80f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d80f5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d80f5-127">Request body</span></span>
<span data-ttu-id="d80f5-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d80f5-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="d80f5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d80f5-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="d80f5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d80f5-130">Property</span></span>|<span data-ttu-id="d80f5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d80f5-131">Type</span></span>|<span data-ttu-id="d80f5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d80f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d80f5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d80f5-133">roleScopeTagIds</span></span>|<span data-ttu-id="d80f5-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d80f5-134">String collection</span></span>|<span data-ttu-id="d80f5-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d80f5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d80f5-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-137">id</span><span class="sxs-lookup"><span data-stu-id="d80f5-137">id</span></span>|<span data-ttu-id="d80f5-138">String</span><span class="sxs-lookup"><span data-stu-id="d80f5-138">String</span></span>|<span data-ttu-id="d80f5-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d80f5-139">Key of the entity.</span></span> <span data-ttu-id="d80f5-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d80f5-141">createdDateTime</span></span>|<span data-ttu-id="d80f5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d80f5-142">DateTimeOffset</span></span>|<span data-ttu-id="d80f5-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d80f5-143">DateTime the object was created.</span></span> <span data-ttu-id="d80f5-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-145">description</span><span class="sxs-lookup"><span data-stu-id="d80f5-145">description</span></span>|<span data-ttu-id="d80f5-146">String</span><span class="sxs-lookup"><span data-stu-id="d80f5-146">String</span></span>|<span data-ttu-id="d80f5-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d80f5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d80f5-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d80f5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d80f5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d80f5-150">DateTimeOffset</span></span>|<span data-ttu-id="d80f5-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d80f5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="d80f5-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d80f5-153">displayName</span></span>|<span data-ttu-id="d80f5-154">String</span><span class="sxs-lookup"><span data-stu-id="d80f5-154">String</span></span>|<span data-ttu-id="d80f5-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d80f5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d80f5-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-157">version</span><span class="sxs-lookup"><span data-stu-id="d80f5-157">version</span></span>|<span data-ttu-id="d80f5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d80f5-158">Int32</span></span>|<span data-ttu-id="d80f5-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d80f5-159">Version of the device configuration.</span></span> <span data-ttu-id="d80f5-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d80f5-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d80f5-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d80f5-161">passwordRequired</span></span>|<span data-ttu-id="d80f5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-162">Boolean</span></span>|<span data-ttu-id="d80f5-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d80f5-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="d80f5-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d80f5-164">passwordMinimumLength</span></span>|<span data-ttu-id="d80f5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d80f5-165">Int32</span></span>|<span data-ttu-id="d80f5-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="d80f5-166">Minimum password length.</span></span> <span data-ttu-id="d80f5-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="d80f5-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d80f5-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d80f5-168">passwordRequiredType</span></span>|[<span data-ttu-id="d80f5-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d80f5-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="d80f5-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="d80f5-170">Type of characters in password.</span></span> <span data-ttu-id="d80f5-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="d80f5-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="d80f5-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d80f5-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d80f5-173">Int32</span><span class="sxs-lookup"><span data-stu-id="d80f5-173">Int32</span></span>|<span data-ttu-id="d80f5-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="d80f5-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d80f5-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d80f5-175">passwordExpirationDays</span></span>|<span data-ttu-id="d80f5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d80f5-176">Int32</span></span>|<span data-ttu-id="d80f5-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="d80f5-177">Number of days before the password expires.</span></span> <span data-ttu-id="d80f5-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="d80f5-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d80f5-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d80f5-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d80f5-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d80f5-180">Int32</span></span>|<span data-ttu-id="d80f5-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d80f5-181">Number of previous passwords to block.</span></span> <span data-ttu-id="d80f5-182">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="d80f5-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d80f5-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d80f5-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d80f5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d80f5-184">Int32</span></span>|<span data-ttu-id="d80f5-185">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="d80f5-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="d80f5-186">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="d80f5-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="d80f5-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="d80f5-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="d80f5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-188">Boolean</span></span>|<span data-ttu-id="d80f5-189">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="d80f5-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="d80f5-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="d80f5-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="d80f5-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-191">Boolean</span></span>|<span data-ttu-id="d80f5-192">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="d80f5-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="d80f5-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="d80f5-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="d80f5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-194">Boolean</span></span>|<span data-ttu-id="d80f5-195">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="d80f5-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="d80f5-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d80f5-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="d80f5-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-197">Boolean</span></span>|<span data-ttu-id="d80f5-198">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="d80f5-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="d80f5-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="d80f5-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="d80f5-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="d80f5-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="d80f5-201">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="d80f5-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="d80f5-202">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="d80f5-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="d80f5-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="d80f5-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="d80f5-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-204">Boolean</span></span>|<span data-ttu-id="d80f5-205">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="d80f5-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="d80f5-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d80f5-206">osMinimumVersion</span></span>|<span data-ttu-id="d80f5-207">String</span><span class="sxs-lookup"><span data-stu-id="d80f5-207">String</span></span>|<span data-ttu-id="d80f5-208">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="d80f5-208">Minimum Android version.</span></span>|
|<span data-ttu-id="d80f5-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d80f5-209">osMaximumVersion</span></span>|<span data-ttu-id="d80f5-210">String</span><span class="sxs-lookup"><span data-stu-id="d80f5-210">String</span></span>|<span data-ttu-id="d80f5-211">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="d80f5-211">Maximum Android version.</span></span>|
|<span data-ttu-id="d80f5-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d80f5-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="d80f5-213">String</span><span class="sxs-lookup"><span data-stu-id="d80f5-213">String</span></span>|<span data-ttu-id="d80f5-214">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="d80f5-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="d80f5-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d80f5-215">storageRequireEncryption</span></span>|<span data-ttu-id="d80f5-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-216">Boolean</span></span>|<span data-ttu-id="d80f5-217">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="d80f5-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="d80f5-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="d80f5-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="d80f5-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-219">Boolean</span></span>|<span data-ttu-id="d80f5-220">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="d80f5-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="d80f5-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="d80f5-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="d80f5-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-222">Boolean</span></span>|<span data-ttu-id="d80f5-223">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="d80f5-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="d80f5-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="d80f5-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="d80f5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-225">Boolean</span></span>|<span data-ttu-id="d80f5-226">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d80f5-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="d80f5-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="d80f5-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="d80f5-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-228">Boolean</span></span>|<span data-ttu-id="d80f5-229">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="d80f5-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="d80f5-230">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="d80f5-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="d80f5-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="d80f5-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="d80f5-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80f5-232">Boolean</span></span>|<span data-ttu-id="d80f5-233">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="d80f5-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="d80f5-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="d80f5-234">Response</span></span>
<span data-ttu-id="d80f5-235">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d80f5-235">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d80f5-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d80f5-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="d80f5-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d80f5-237">Request</span></span>
<span data-ttu-id="d80f5-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d80f5-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="d80f5-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="d80f5-239">Response</span></span>
<span data-ttu-id="d80f5-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d80f5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




