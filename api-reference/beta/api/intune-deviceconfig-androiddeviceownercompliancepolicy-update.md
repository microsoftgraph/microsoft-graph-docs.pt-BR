---
title: Atualizar androidDeviceOwnerCompliancePolicy
description: Atualiza as propriedades de um objeto androidDeviceOwnerCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 818e7a1717c079c1dbc0f45da898d2494098d83a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759861"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="fee96-103">Atualizar androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fee96-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="fee96-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fee96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fee96-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fee96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fee96-106">Atualiza as propriedades de um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fee96-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fee96-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fee96-107">Prerequisites</span></span>
<span data-ttu-id="fee96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fee96-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fee96-110">Permission type</span></span>|<span data-ttu-id="fee96-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fee96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fee96-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fee96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fee96-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fee96-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fee96-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fee96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fee96-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee96-115">Not supported.</span></span>|
|<span data-ttu-id="fee96-116">Application</span><span class="sxs-lookup"><span data-stu-id="fee96-116">Application</span></span>|<span data-ttu-id="fee96-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fee96-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fee96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fee96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fee96-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fee96-119">Request headers</span></span>
|<span data-ttu-id="fee96-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fee96-120">Header</span></span>|<span data-ttu-id="fee96-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fee96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fee96-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fee96-122">Authorization</span></span>|<span data-ttu-id="fee96-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fee96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fee96-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fee96-124">Accept</span></span>|<span data-ttu-id="fee96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fee96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fee96-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fee96-126">Request body</span></span>
<span data-ttu-id="fee96-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fee96-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="fee96-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fee96-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="fee96-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fee96-129">Property</span></span>|<span data-ttu-id="fee96-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee96-130">Type</span></span>|<span data-ttu-id="fee96-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fee96-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fee96-132">roleScopeTagIds</span></span>|<span data-ttu-id="fee96-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fee96-133">String collection</span></span>|<span data-ttu-id="fee96-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fee96-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fee96-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-136">id</span><span class="sxs-lookup"><span data-stu-id="fee96-136">id</span></span>|<span data-ttu-id="fee96-137">String</span><span class="sxs-lookup"><span data-stu-id="fee96-137">String</span></span>|<span data-ttu-id="fee96-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fee96-138">Key of the entity.</span></span> <span data-ttu-id="fee96-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fee96-140">createdDateTime</span></span>|<span data-ttu-id="fee96-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee96-141">DateTimeOffset</span></span>|<span data-ttu-id="fee96-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fee96-142">DateTime the object was created.</span></span> <span data-ttu-id="fee96-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-144">description</span><span class="sxs-lookup"><span data-stu-id="fee96-144">description</span></span>|<span data-ttu-id="fee96-145">String</span><span class="sxs-lookup"><span data-stu-id="fee96-145">String</span></span>|<span data-ttu-id="fee96-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fee96-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fee96-148">lastModifiedDateTime</span></span>|<span data-ttu-id="fee96-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee96-149">DateTimeOffset</span></span>|<span data-ttu-id="fee96-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fee96-150">DateTime the object was last modified.</span></span> <span data-ttu-id="fee96-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-152">displayName</span><span class="sxs-lookup"><span data-stu-id="fee96-152">displayName</span></span>|<span data-ttu-id="fee96-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fee96-153">String</span></span>|<span data-ttu-id="fee96-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fee96-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-156">version</span><span class="sxs-lookup"><span data-stu-id="fee96-156">version</span></span>|<span data-ttu-id="fee96-157">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-157">Int32</span></span>|<span data-ttu-id="fee96-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-158">Version of the device configuration.</span></span> <span data-ttu-id="fee96-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fee96-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fee96-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="fee96-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="fee96-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="fee96-161">Boolean</span></span>|<span data-ttu-id="fee96-162">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="fee96-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="fee96-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="fee96-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="fee96-164">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="fee96-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="fee96-165">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="fee96-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="fee96-166">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="fee96-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="fee96-167">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="fee96-167">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="fee96-168">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="fee96-168">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="fee96-169">MDATP requer nível mínimo de risco de proteção contra ameaças móveis para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="fee96-169">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="fee96-170">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="fee96-170">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="fee96-171">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="fee96-171">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="fee96-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="fee96-172">Boolean</span></span>|<span data-ttu-id="fee96-173">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="fee96-173">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="fee96-174">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="fee96-174">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="fee96-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="fee96-175">Boolean</span></span>|<span data-ttu-id="fee96-176">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="fee96-176">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="fee96-177">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fee96-177">osMinimumVersion</span></span>|<span data-ttu-id="fee96-178">String</span><span class="sxs-lookup"><span data-stu-id="fee96-178">String</span></span>|<span data-ttu-id="fee96-179">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="fee96-179">Minimum Android version.</span></span>|
|<span data-ttu-id="fee96-180">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fee96-180">osMaximumVersion</span></span>|<span data-ttu-id="fee96-181">String</span><span class="sxs-lookup"><span data-stu-id="fee96-181">String</span></span>|<span data-ttu-id="fee96-182">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="fee96-182">Maximum Android version.</span></span>|
|<span data-ttu-id="fee96-183">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="fee96-183">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="fee96-184">String</span><span class="sxs-lookup"><span data-stu-id="fee96-184">String</span></span>|<span data-ttu-id="fee96-185">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="fee96-185">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="fee96-186">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fee96-186">passwordRequired</span></span>|<span data-ttu-id="fee96-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="fee96-187">Boolean</span></span>|<span data-ttu-id="fee96-188">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-188">Require a password to unlock device.</span></span>|
|<span data-ttu-id="fee96-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fee96-189">passwordMinimumLength</span></span>|<span data-ttu-id="fee96-190">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-190">Int32</span></span>|<span data-ttu-id="fee96-191">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="fee96-191">Minimum password length.</span></span> <span data-ttu-id="fee96-192">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="fee96-193">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="fee96-193">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="fee96-194">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-194">Int32</span></span>|<span data-ttu-id="fee96-195">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-195">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="fee96-196">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fee96-197">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="fee96-197">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="fee96-198">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-198">Int32</span></span>|<span data-ttu-id="fee96-199">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-199">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="fee96-200">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fee96-201">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="fee96-201">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="fee96-202">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-202">Int32</span></span>|<span data-ttu-id="fee96-203">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-203">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="fee96-204">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fee96-205">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="fee96-205">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="fee96-206">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-206">Int32</span></span>|<span data-ttu-id="fee96-207">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-207">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="fee96-208">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fee96-209">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="fee96-209">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="fee96-210">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-210">Int32</span></span>|<span data-ttu-id="fee96-211">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-211">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="fee96-212">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fee96-213">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="fee96-213">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="fee96-214">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-214">Int32</span></span>|<span data-ttu-id="fee96-215">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fee96-215">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="fee96-216">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="fee96-216">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fee96-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fee96-217">passwordRequiredType</span></span>|[<span data-ttu-id="fee96-218">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="fee96-218">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="fee96-219">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="fee96-219">Type of characters in password.</span></span> <span data-ttu-id="fee96-220">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="fee96-220">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="fee96-221">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fee96-221">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fee96-222">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-222">Int32</span></span>|<span data-ttu-id="fee96-223">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="fee96-223">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="fee96-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fee96-224">passwordExpirationDays</span></span>|<span data-ttu-id="fee96-225">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-225">Int32</span></span>|<span data-ttu-id="fee96-226">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="fee96-226">Number of days before the password expires.</span></span> <span data-ttu-id="fee96-227">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="fee96-227">Valid values 1 to 365</span></span>|
|<span data-ttu-id="fee96-228">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="fee96-228">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="fee96-229">Int32</span><span class="sxs-lookup"><span data-stu-id="fee96-229">Int32</span></span>|<span data-ttu-id="fee96-230">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="fee96-230">Number of previous passwords to block.</span></span> <span data-ttu-id="fee96-231">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="fee96-231">Valid values 1 to 24</span></span>|
|<span data-ttu-id="fee96-232">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="fee96-232">storageRequireEncryption</span></span>|<span data-ttu-id="fee96-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="fee96-233">Boolean</span></span>|<span data-ttu-id="fee96-234">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="fee96-234">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="fee96-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee96-235">Response</span></span>
<span data-ttu-id="fee96-236">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fee96-236">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fee96-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fee96-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="fee96-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fee96-238">Request</span></span>
<span data-ttu-id="fee96-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fee96-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1223

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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

### <a name="response"></a><span data-ttu-id="fee96-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee96-240">Response</span></span>
<span data-ttu-id="fee96-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fee96-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1395

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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




