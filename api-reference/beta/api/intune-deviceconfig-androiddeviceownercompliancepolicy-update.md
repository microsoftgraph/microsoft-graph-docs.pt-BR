---
title: Atualizar androidDeviceOwnerCompliancePolicy
description: Atualize as propriedades de um objeto androidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3dd359839127b16ac9ebb7ae74478a287530694a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133539"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="6528b-103">Atualizar androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6528b-103">Update androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="6528b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6528b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6528b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6528b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6528b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6528b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6528b-107">Atualize as propriedades de [um objeto androidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-107">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6528b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6528b-108">Prerequisites</span></span>
<span data-ttu-id="6528b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6528b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6528b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6528b-111">Permission type</span></span>|<span data-ttu-id="6528b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6528b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6528b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6528b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6528b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6528b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6528b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6528b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6528b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6528b-116">Not supported.</span></span>|
|<span data-ttu-id="6528b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6528b-117">Application</span></span>|<span data-ttu-id="6528b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6528b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6528b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6528b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6528b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6528b-120">Request headers</span></span>
|<span data-ttu-id="6528b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6528b-121">Header</span></span>|<span data-ttu-id="6528b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6528b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6528b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6528b-123">Authorization</span></span>|<span data-ttu-id="6528b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6528b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6528b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6528b-125">Accept</span></span>|<span data-ttu-id="6528b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6528b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6528b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6528b-127">Request body</span></span>
<span data-ttu-id="6528b-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-128">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="6528b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6528b-129">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="6528b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6528b-130">Property</span></span>|<span data-ttu-id="6528b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6528b-131">Type</span></span>|<span data-ttu-id="6528b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6528b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6528b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6528b-133">roleScopeTagIds</span></span>|<span data-ttu-id="6528b-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6528b-134">String collection</span></span>|<span data-ttu-id="6528b-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="6528b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6528b-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-137">id</span><span class="sxs-lookup"><span data-stu-id="6528b-137">id</span></span>|<span data-ttu-id="6528b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6528b-138">String</span></span>|<span data-ttu-id="6528b-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6528b-139">Key of the entity.</span></span> <span data-ttu-id="6528b-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6528b-141">createdDateTime</span></span>|<span data-ttu-id="6528b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6528b-142">DateTimeOffset</span></span>|<span data-ttu-id="6528b-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6528b-143">DateTime the object was created.</span></span> <span data-ttu-id="6528b-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-145">descrição</span><span class="sxs-lookup"><span data-stu-id="6528b-145">description</span></span>|<span data-ttu-id="6528b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6528b-146">String</span></span>|<span data-ttu-id="6528b-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6528b-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6528b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6528b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6528b-150">DateTimeOffset</span></span>|<span data-ttu-id="6528b-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6528b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="6528b-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6528b-153">displayName</span></span>|<span data-ttu-id="6528b-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6528b-154">String</span></span>|<span data-ttu-id="6528b-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6528b-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-157">version</span><span class="sxs-lookup"><span data-stu-id="6528b-157">version</span></span>|<span data-ttu-id="6528b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-158">Int32</span></span>|<span data-ttu-id="6528b-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-159">Version of the device configuration.</span></span> <span data-ttu-id="6528b-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6528b-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6528b-161">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6528b-161">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6528b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6528b-162">Boolean</span></span>|<span data-ttu-id="6528b-163">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="6528b-163">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6528b-164">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6528b-164">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6528b-165">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6528b-165">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6528b-166">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="6528b-166">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6528b-167">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6528b-167">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6528b-168">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6528b-168">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6528b-169">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6528b-169">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6528b-170">O MDATP exige nível mínimo de risco da Proteção Contra Ameaças Móveis para relatar o não-atendimento.</span><span class="sxs-lookup"><span data-stu-id="6528b-170">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6528b-171">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6528b-171">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6528b-172">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="6528b-172">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="6528b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6528b-173">Boolean</span></span>|<span data-ttu-id="6528b-174">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6528b-174">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="6528b-175">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="6528b-175">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="6528b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="6528b-176">Boolean</span></span>|<span data-ttu-id="6528b-177">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6528b-177">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="6528b-178">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6528b-178">osMinimumVersion</span></span>|<span data-ttu-id="6528b-179">String</span><span class="sxs-lookup"><span data-stu-id="6528b-179">String</span></span>|<span data-ttu-id="6528b-180">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="6528b-180">Minimum Android version.</span></span>|
|<span data-ttu-id="6528b-181">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6528b-181">osMaximumVersion</span></span>|<span data-ttu-id="6528b-182">String</span><span class="sxs-lookup"><span data-stu-id="6528b-182">String</span></span>|<span data-ttu-id="6528b-183">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="6528b-183">Maximum Android version.</span></span>|
|<span data-ttu-id="6528b-184">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6528b-184">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="6528b-185">String</span><span class="sxs-lookup"><span data-stu-id="6528b-185">String</span></span>|<span data-ttu-id="6528b-186">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="6528b-186">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="6528b-187">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6528b-187">passwordRequired</span></span>|<span data-ttu-id="6528b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6528b-188">Boolean</span></span>|<span data-ttu-id="6528b-189">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-189">Require a password to unlock device.</span></span>|
|<span data-ttu-id="6528b-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6528b-190">passwordMinimumLength</span></span>|<span data-ttu-id="6528b-191">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-191">Int32</span></span>|<span data-ttu-id="6528b-192">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="6528b-192">Minimum password length.</span></span> <span data-ttu-id="6528b-193">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6528b-194">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6528b-194">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="6528b-195">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-195">Int32</span></span>|<span data-ttu-id="6528b-196">Indica o número mínimo de caracteres de letra necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-196">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="6528b-197">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-197">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6528b-198">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6528b-198">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="6528b-199">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-199">Int32</span></span>|<span data-ttu-id="6528b-200">Indica o número mínimo de caracteres de caixa inferiores necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-200">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="6528b-201">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-201">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6528b-202">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6528b-202">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="6528b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-203">Int32</span></span>|<span data-ttu-id="6528b-204">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-204">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="6528b-205">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-205">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6528b-206">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6528b-206">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="6528b-207">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-207">Int32</span></span>|<span data-ttu-id="6528b-208">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-208">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="6528b-209">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-209">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6528b-210">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6528b-210">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="6528b-211">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-211">Int32</span></span>|<span data-ttu-id="6528b-212">Indica o número mínimo de caracteres de símbolo necessário para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-212">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="6528b-213">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-213">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6528b-214">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6528b-214">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="6528b-215">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-215">Int32</span></span>|<span data-ttu-id="6528b-216">Indica o número mínimo de caracteres de letras maiúsculas de maiúsculas e médios necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6528b-216">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="6528b-217">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="6528b-217">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6528b-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6528b-218">passwordRequiredType</span></span>|[<span data-ttu-id="6528b-219">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6528b-219">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="6528b-220">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="6528b-220">Type of characters in password.</span></span> <span data-ttu-id="6528b-221">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="6528b-221">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="6528b-222">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6528b-222">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6528b-223">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-223">Int32</span></span>|<span data-ttu-id="6528b-224">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6528b-224">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6528b-225">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6528b-225">passwordExpirationDays</span></span>|<span data-ttu-id="6528b-226">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-226">Int32</span></span>|<span data-ttu-id="6528b-227">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="6528b-227">Number of days before the password expires.</span></span> <span data-ttu-id="6528b-228">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="6528b-228">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6528b-229">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="6528b-229">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="6528b-230">Int32</span><span class="sxs-lookup"><span data-stu-id="6528b-230">Int32</span></span>|<span data-ttu-id="6528b-231">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6528b-231">Number of previous passwords to block.</span></span> <span data-ttu-id="6528b-232">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="6528b-232">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6528b-233">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6528b-233">storageRequireEncryption</span></span>|<span data-ttu-id="6528b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="6528b-234">Boolean</span></span>|<span data-ttu-id="6528b-235">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="6528b-235">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6528b-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="6528b-236">Response</span></span>
<span data-ttu-id="6528b-237">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6528b-237">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6528b-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6528b-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="6528b-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6528b-239">Request</span></span>
<span data-ttu-id="6528b-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6528b-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6528b-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="6528b-241">Response</span></span>
<span data-ttu-id="6528b-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6528b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




