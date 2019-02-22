---
title: Criar androidForWorkCompliancePolicy
description: Criar um novo objeto androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e3f644236c6c76c46481acfcb4a6a4ba778eefa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144916"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="0d86a-103">Criar androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0d86a-103">Create androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="0d86a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d86a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d86a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d86a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d86a-106">Criar um novo objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0d86a-106">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d86a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d86a-107">Prerequisites</span></span>
<span data-ttu-id="0d86a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d86a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d86a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d86a-110">Permission type</span></span>|<span data-ttu-id="0d86a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d86a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d86a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d86a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d86a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d86a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d86a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d86a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d86a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d86a-115">Not supported.</span></span>|
|<span data-ttu-id="0d86a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d86a-116">Application</span></span>|<span data-ttu-id="0d86a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d86a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d86a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d86a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0d86a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d86a-119">Request headers</span></span>
|<span data-ttu-id="0d86a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d86a-120">Header</span></span>|<span data-ttu-id="0d86a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0d86a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d86a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d86a-122">Authorization</span></span>|<span data-ttu-id="0d86a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d86a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d86a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d86a-124">Accept</span></span>|<span data-ttu-id="0d86a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d86a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d86a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d86a-126">Request body</span></span>
<span data-ttu-id="0d86a-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0d86a-127">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="0d86a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="0d86a-128">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="0d86a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d86a-129">Property</span></span>|<span data-ttu-id="0d86a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d86a-130">Type</span></span>|<span data-ttu-id="0d86a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d86a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d86a-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d86a-132">roleScopeTagIds</span></span>|<span data-ttu-id="0d86a-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d86a-133">String collection</span></span>|<span data-ttu-id="0d86a-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0d86a-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0d86a-135">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-136">id</span><span class="sxs-lookup"><span data-stu-id="0d86a-136">id</span></span>|<span data-ttu-id="0d86a-137">String</span><span class="sxs-lookup"><span data-stu-id="0d86a-137">String</span></span>|<span data-ttu-id="0d86a-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d86a-138">Key of the entity.</span></span> <span data-ttu-id="0d86a-139">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d86a-140">createdDateTime</span></span>|<span data-ttu-id="0d86a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d86a-141">DateTimeOffset</span></span>|<span data-ttu-id="0d86a-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0d86a-142">DateTime the object was created.</span></span> <span data-ttu-id="0d86a-143">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-144">description</span><span class="sxs-lookup"><span data-stu-id="0d86a-144">description</span></span>|<span data-ttu-id="0d86a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d86a-145">String</span></span>|<span data-ttu-id="0d86a-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d86a-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d86a-147">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d86a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0d86a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d86a-149">DateTimeOffset</span></span>|<span data-ttu-id="0d86a-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0d86a-150">DateTime the object was last modified.</span></span> <span data-ttu-id="0d86a-151">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-152">displayName</span><span class="sxs-lookup"><span data-stu-id="0d86a-152">displayName</span></span>|<span data-ttu-id="0d86a-153">String</span><span class="sxs-lookup"><span data-stu-id="0d86a-153">String</span></span>|<span data-ttu-id="0d86a-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d86a-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d86a-155">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-156">version</span><span class="sxs-lookup"><span data-stu-id="0d86a-156">version</span></span>|<span data-ttu-id="0d86a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0d86a-157">Int32</span></span>|<span data-ttu-id="0d86a-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d86a-158">Version of the device configuration.</span></span> <span data-ttu-id="0d86a-159">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0d86a-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d86a-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0d86a-160">passwordRequired</span></span>|<span data-ttu-id="0d86a-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-161">Boolean</span></span>|<span data-ttu-id="0d86a-162">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d86a-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="0d86a-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0d86a-163">passwordMinimumLength</span></span>|<span data-ttu-id="0d86a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0d86a-164">Int32</span></span>|<span data-ttu-id="0d86a-165">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0d86a-165">Minimum password length.</span></span> <span data-ttu-id="0d86a-166">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="0d86a-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0d86a-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0d86a-167">passwordRequiredType</span></span>|[<span data-ttu-id="0d86a-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0d86a-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="0d86a-169">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="0d86a-169">Type of characters in password.</span></span> <span data-ttu-id="0d86a-170">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="0d86a-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="0d86a-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0d86a-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0d86a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="0d86a-172">Int32</span></span>|<span data-ttu-id="0d86a-173">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0d86a-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0d86a-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0d86a-174">passwordExpirationDays</span></span>|<span data-ttu-id="0d86a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0d86a-175">Int32</span></span>|<span data-ttu-id="0d86a-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="0d86a-176">Number of days before the password expires.</span></span> <span data-ttu-id="0d86a-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="0d86a-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="0d86a-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0d86a-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0d86a-179">Int32</span><span class="sxs-lookup"><span data-stu-id="0d86a-179">Int32</span></span>|<span data-ttu-id="0d86a-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="0d86a-180">Number of previous passwords to block.</span></span> <span data-ttu-id="0d86a-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="0d86a-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0d86a-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="0d86a-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="0d86a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0d86a-183">Int32</span></span>|<span data-ttu-id="0d86a-184">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="0d86a-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="0d86a-185">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="0d86a-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="0d86a-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="0d86a-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="0d86a-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-187">Boolean</span></span>|<span data-ttu-id="0d86a-188">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="0d86a-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="0d86a-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="0d86a-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="0d86a-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-190">Boolean</span></span>|<span data-ttu-id="0d86a-191">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="0d86a-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="0d86a-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="0d86a-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="0d86a-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-193">Boolean</span></span>|<span data-ttu-id="0d86a-194">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="0d86a-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="0d86a-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0d86a-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0d86a-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-196">Boolean</span></span>|<span data-ttu-id="0d86a-197">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="0d86a-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0d86a-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0d86a-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0d86a-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0d86a-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0d86a-200">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="0d86a-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0d86a-201">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0d86a-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0d86a-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="0d86a-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="0d86a-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-203">Boolean</span></span>|<span data-ttu-id="0d86a-204">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="0d86a-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="0d86a-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0d86a-205">osMinimumVersion</span></span>|<span data-ttu-id="0d86a-206">String</span><span class="sxs-lookup"><span data-stu-id="0d86a-206">String</span></span>|<span data-ttu-id="0d86a-207">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="0d86a-207">Minimum Android version.</span></span>|
|<span data-ttu-id="0d86a-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0d86a-208">osMaximumVersion</span></span>|<span data-ttu-id="0d86a-209">String</span><span class="sxs-lookup"><span data-stu-id="0d86a-209">String</span></span>|<span data-ttu-id="0d86a-210">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="0d86a-210">Maximum Android version.</span></span>|
|<span data-ttu-id="0d86a-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0d86a-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="0d86a-212">String</span><span class="sxs-lookup"><span data-stu-id="0d86a-212">String</span></span>|<span data-ttu-id="0d86a-213">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="0d86a-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="0d86a-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0d86a-214">storageRequireEncryption</span></span>|<span data-ttu-id="0d86a-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-215">Boolean</span></span>|<span data-ttu-id="0d86a-216">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="0d86a-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="0d86a-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="0d86a-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="0d86a-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-218">Boolean</span></span>|<span data-ttu-id="0d86a-219">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="0d86a-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="0d86a-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="0d86a-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="0d86a-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-221">Boolean</span></span>|<span data-ttu-id="0d86a-222">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="0d86a-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="0d86a-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="0d86a-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="0d86a-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-224">Boolean</span></span>|<span data-ttu-id="0d86a-225">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0d86a-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="0d86a-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="0d86a-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="0d86a-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-227">Boolean</span></span>|<span data-ttu-id="0d86a-228">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="0d86a-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="0d86a-229">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="0d86a-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="0d86a-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="0d86a-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="0d86a-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d86a-231">Boolean</span></span>|<span data-ttu-id="0d86a-232">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="0d86a-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="0d86a-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d86a-233">Response</span></span>
<span data-ttu-id="0d86a-234">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d86a-234">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d86a-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d86a-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d86a-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d86a-236">Request</span></span>
<span data-ttu-id="0d86a-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d86a-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d86a-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d86a-238">Response</span></span>
<span data-ttu-id="0d86a-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d86a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




