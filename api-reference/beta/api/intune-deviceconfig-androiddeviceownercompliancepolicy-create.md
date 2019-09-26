---
title: Criar androidDeviceOwnerCompliancePolicy
description: Criar um novo objeto androidDeviceOwnerCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c6df95e12c0837cfcb70cbaae1e59731b484a63
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170053"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="49a22-103">Criar androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="49a22-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="49a22-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49a22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49a22-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49a22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49a22-106">Criar um novo objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="49a22-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49a22-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49a22-107">Prerequisites</span></span>
<span data-ttu-id="49a22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49a22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49a22-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49a22-110">Permission type</span></span>|<span data-ttu-id="49a22-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49a22-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49a22-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49a22-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49a22-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49a22-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49a22-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49a22-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49a22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49a22-115">Not supported.</span></span>|
|<span data-ttu-id="49a22-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49a22-116">Application</span></span>|<span data-ttu-id="49a22-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49a22-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49a22-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49a22-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="49a22-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49a22-119">Request headers</span></span>
|<span data-ttu-id="49a22-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49a22-120">Header</span></span>|<span data-ttu-id="49a22-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49a22-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49a22-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49a22-122">Authorization</span></span>|<span data-ttu-id="49a22-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49a22-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49a22-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49a22-124">Accept</span></span>|<span data-ttu-id="49a22-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49a22-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49a22-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49a22-126">Request body</span></span>
<span data-ttu-id="49a22-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="49a22-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="49a22-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="49a22-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="49a22-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49a22-129">Property</span></span>|<span data-ttu-id="49a22-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49a22-130">Type</span></span>|<span data-ttu-id="49a22-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49a22-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49a22-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49a22-132">roleScopeTagIds</span></span>|<span data-ttu-id="49a22-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49a22-133">String collection</span></span>|<span data-ttu-id="49a22-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="49a22-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49a22-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-136">id</span><span class="sxs-lookup"><span data-stu-id="49a22-136">id</span></span>|<span data-ttu-id="49a22-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49a22-137">String</span></span>|<span data-ttu-id="49a22-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="49a22-138">Key of the entity.</span></span> <span data-ttu-id="49a22-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49a22-140">createdDateTime</span></span>|<span data-ttu-id="49a22-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49a22-141">DateTimeOffset</span></span>|<span data-ttu-id="49a22-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="49a22-142">DateTime the object was created.</span></span> <span data-ttu-id="49a22-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-144">descrição</span><span class="sxs-lookup"><span data-stu-id="49a22-144">description</span></span>|<span data-ttu-id="49a22-145">String</span><span class="sxs-lookup"><span data-stu-id="49a22-145">String</span></span>|<span data-ttu-id="49a22-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49a22-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49a22-148">lastModifiedDateTime</span></span>|<span data-ttu-id="49a22-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49a22-149">DateTimeOffset</span></span>|<span data-ttu-id="49a22-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="49a22-150">DateTime the object was last modified.</span></span> <span data-ttu-id="49a22-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-152">displayName</span><span class="sxs-lookup"><span data-stu-id="49a22-152">displayName</span></span>|<span data-ttu-id="49a22-153">String</span><span class="sxs-lookup"><span data-stu-id="49a22-153">String</span></span>|<span data-ttu-id="49a22-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49a22-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-156">version</span><span class="sxs-lookup"><span data-stu-id="49a22-156">version</span></span>|<span data-ttu-id="49a22-157">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-157">Int32</span></span>|<span data-ttu-id="49a22-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-158">Version of the device configuration.</span></span> <span data-ttu-id="49a22-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49a22-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49a22-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="49a22-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="49a22-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="49a22-161">Boolean</span></span>|<span data-ttu-id="49a22-162">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="49a22-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="49a22-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="49a22-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="49a22-164">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="49a22-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="49a22-165">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="49a22-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="49a22-166">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="49a22-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="49a22-167">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="49a22-167">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="49a22-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="49a22-168">Boolean</span></span>|<span data-ttu-id="49a22-169">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="49a22-169">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="49a22-170">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="49a22-170">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="49a22-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="49a22-171">Boolean</span></span>|<span data-ttu-id="49a22-172">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="49a22-172">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="49a22-173">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="49a22-173">osMinimumVersion</span></span>|<span data-ttu-id="49a22-174">String</span><span class="sxs-lookup"><span data-stu-id="49a22-174">String</span></span>|<span data-ttu-id="49a22-175">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="49a22-175">Minimum Android version.</span></span>|
|<span data-ttu-id="49a22-176">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="49a22-176">osMaximumVersion</span></span>|<span data-ttu-id="49a22-177">String</span><span class="sxs-lookup"><span data-stu-id="49a22-177">String</span></span>|<span data-ttu-id="49a22-178">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="49a22-178">Maximum Android version.</span></span>|
|<span data-ttu-id="49a22-179">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="49a22-179">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="49a22-180">String</span><span class="sxs-lookup"><span data-stu-id="49a22-180">String</span></span>|<span data-ttu-id="49a22-181">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="49a22-181">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="49a22-182">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="49a22-182">passwordRequired</span></span>|<span data-ttu-id="49a22-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="49a22-183">Boolean</span></span>|<span data-ttu-id="49a22-184">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-184">Require a password to unlock device.</span></span>|
|<span data-ttu-id="49a22-185">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="49a22-185">passwordMinimumLength</span></span>|<span data-ttu-id="49a22-186">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-186">Int32</span></span>|<span data-ttu-id="49a22-187">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="49a22-187">Minimum password length.</span></span> <span data-ttu-id="49a22-188">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-188">Valid values 4 to 16</span></span>|
|<span data-ttu-id="49a22-189">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="49a22-189">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="49a22-190">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-190">Int32</span></span>|<span data-ttu-id="49a22-191">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-191">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="49a22-192">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="49a22-193">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="49a22-193">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="49a22-194">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-194">Int32</span></span>|<span data-ttu-id="49a22-195">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-195">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="49a22-196">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="49a22-197">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="49a22-197">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="49a22-198">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-198">Int32</span></span>|<span data-ttu-id="49a22-199">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-199">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="49a22-200">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="49a22-201">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="49a22-201">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="49a22-202">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-202">Int32</span></span>|<span data-ttu-id="49a22-203">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-203">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="49a22-204">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="49a22-205">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="49a22-205">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="49a22-206">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-206">Int32</span></span>|<span data-ttu-id="49a22-207">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-207">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="49a22-208">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="49a22-209">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="49a22-209">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="49a22-210">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-210">Int32</span></span>|<span data-ttu-id="49a22-211">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49a22-211">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="49a22-212">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="49a22-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="49a22-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="49a22-213">passwordRequiredType</span></span>|[<span data-ttu-id="49a22-214">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="49a22-214">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="49a22-215">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="49a22-215">Type of characters in password.</span></span> <span data-ttu-id="49a22-216">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="49a22-216">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="49a22-217">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="49a22-217">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="49a22-218">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-218">Int32</span></span>|<span data-ttu-id="49a22-219">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="49a22-219">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="49a22-220">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="49a22-220">passwordExpirationDays</span></span>|<span data-ttu-id="49a22-221">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-221">Int32</span></span>|<span data-ttu-id="49a22-222">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="49a22-222">Number of days before the password expires.</span></span> <span data-ttu-id="49a22-223">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="49a22-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="49a22-224">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="49a22-224">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="49a22-225">Int32</span><span class="sxs-lookup"><span data-stu-id="49a22-225">Int32</span></span>|<span data-ttu-id="49a22-226">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="49a22-226">Number of previous passwords to block.</span></span> <span data-ttu-id="49a22-227">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="49a22-227">Valid values 1 to 24</span></span>|
|<span data-ttu-id="49a22-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="49a22-228">storageRequireEncryption</span></span>|<span data-ttu-id="49a22-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="49a22-229">Boolean</span></span>|<span data-ttu-id="49a22-230">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="49a22-230">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="49a22-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="49a22-231">Response</span></span>
<span data-ttu-id="49a22-232">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49a22-232">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49a22-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49a22-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="49a22-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49a22-234">Request</span></span>
<span data-ttu-id="49a22-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49a22-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1160

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="49a22-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="49a22-236">Response</span></span>
<span data-ttu-id="49a22-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49a22-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1332

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```




