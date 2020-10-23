---
title: Atualizar androidDeviceOwnerCompliancePolicy
description: Atualiza as propriedades de um objeto androidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4574c8bf63d429a0be8b13af791821770299ea74
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733941"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="eadcb-103">Atualizar androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="eadcb-103">Update androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="eadcb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eadcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eadcb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eadcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eadcb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eadcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eadcb-107">Atualiza as propriedades de um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="eadcb-107">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eadcb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eadcb-108">Prerequisites</span></span>
<span data-ttu-id="eadcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eadcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eadcb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eadcb-111">Permission type</span></span>|<span data-ttu-id="eadcb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eadcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eadcb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eadcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eadcb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eadcb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eadcb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eadcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eadcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eadcb-116">Not supported.</span></span>|
|<span data-ttu-id="eadcb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eadcb-117">Application</span></span>|<span data-ttu-id="eadcb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eadcb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eadcb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eadcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="eadcb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eadcb-120">Request headers</span></span>
|<span data-ttu-id="eadcb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eadcb-121">Header</span></span>|<span data-ttu-id="eadcb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eadcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eadcb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eadcb-123">Authorization</span></span>|<span data-ttu-id="eadcb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eadcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eadcb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eadcb-125">Accept</span></span>|<span data-ttu-id="eadcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eadcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eadcb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eadcb-127">Request body</span></span>
<span data-ttu-id="eadcb-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="eadcb-128">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="eadcb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="eadcb-129">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="eadcb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eadcb-130">Property</span></span>|<span data-ttu-id="eadcb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eadcb-131">Type</span></span>|<span data-ttu-id="eadcb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eadcb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eadcb-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eadcb-133">roleScopeTagIds</span></span>|<span data-ttu-id="eadcb-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eadcb-134">String collection</span></span>|<span data-ttu-id="eadcb-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="eadcb-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eadcb-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-137">id</span><span class="sxs-lookup"><span data-stu-id="eadcb-137">id</span></span>|<span data-ttu-id="eadcb-138">String</span><span class="sxs-lookup"><span data-stu-id="eadcb-138">String</span></span>|<span data-ttu-id="eadcb-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eadcb-139">Key of the entity.</span></span> <span data-ttu-id="eadcb-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eadcb-141">createdDateTime</span></span>|<span data-ttu-id="eadcb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eadcb-142">DateTimeOffset</span></span>|<span data-ttu-id="eadcb-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="eadcb-143">DateTime the object was created.</span></span> <span data-ttu-id="eadcb-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-145">description</span><span class="sxs-lookup"><span data-stu-id="eadcb-145">description</span></span>|<span data-ttu-id="eadcb-146">String</span><span class="sxs-lookup"><span data-stu-id="eadcb-146">String</span></span>|<span data-ttu-id="eadcb-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eadcb-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eadcb-149">lastModifiedDateTime</span></span>|<span data-ttu-id="eadcb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eadcb-150">DateTimeOffset</span></span>|<span data-ttu-id="eadcb-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="eadcb-151">DateTime the object was last modified.</span></span> <span data-ttu-id="eadcb-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-153">displayName</span><span class="sxs-lookup"><span data-stu-id="eadcb-153">displayName</span></span>|<span data-ttu-id="eadcb-154">String</span><span class="sxs-lookup"><span data-stu-id="eadcb-154">String</span></span>|<span data-ttu-id="eadcb-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eadcb-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-157">version</span><span class="sxs-lookup"><span data-stu-id="eadcb-157">version</span></span>|<span data-ttu-id="eadcb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-158">Int32</span></span>|<span data-ttu-id="eadcb-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-159">Version of the device configuration.</span></span> <span data-ttu-id="eadcb-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eadcb-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eadcb-161">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="eadcb-161">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="eadcb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eadcb-162">Boolean</span></span>|<span data-ttu-id="eadcb-163">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="eadcb-163">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="eadcb-164">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="eadcb-164">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="eadcb-165">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="eadcb-165">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="eadcb-166">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="eadcb-166">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="eadcb-167">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="eadcb-167">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="eadcb-168">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="eadcb-168">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="eadcb-169">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="eadcb-169">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="eadcb-170">MDATP requer nível mínimo de risco de proteção contra ameaças móveis para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="eadcb-170">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="eadcb-171">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="eadcb-171">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="eadcb-172">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="eadcb-172">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="eadcb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="eadcb-173">Boolean</span></span>|<span data-ttu-id="eadcb-174">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="eadcb-174">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="eadcb-175">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="eadcb-175">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="eadcb-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="eadcb-176">Boolean</span></span>|<span data-ttu-id="eadcb-177">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="eadcb-177">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="eadcb-178">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="eadcb-178">osMinimumVersion</span></span>|<span data-ttu-id="eadcb-179">String</span><span class="sxs-lookup"><span data-stu-id="eadcb-179">String</span></span>|<span data-ttu-id="eadcb-180">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="eadcb-180">Minimum Android version.</span></span>|
|<span data-ttu-id="eadcb-181">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="eadcb-181">osMaximumVersion</span></span>|<span data-ttu-id="eadcb-182">String</span><span class="sxs-lookup"><span data-stu-id="eadcb-182">String</span></span>|<span data-ttu-id="eadcb-183">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="eadcb-183">Maximum Android version.</span></span>|
|<span data-ttu-id="eadcb-184">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="eadcb-184">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="eadcb-185">String</span><span class="sxs-lookup"><span data-stu-id="eadcb-185">String</span></span>|<span data-ttu-id="eadcb-186">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="eadcb-186">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="eadcb-187">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="eadcb-187">passwordRequired</span></span>|<span data-ttu-id="eadcb-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="eadcb-188">Boolean</span></span>|<span data-ttu-id="eadcb-189">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-189">Require a password to unlock device.</span></span>|
|<span data-ttu-id="eadcb-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="eadcb-190">passwordMinimumLength</span></span>|<span data-ttu-id="eadcb-191">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-191">Int32</span></span>|<span data-ttu-id="eadcb-192">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="eadcb-192">Minimum password length.</span></span> <span data-ttu-id="eadcb-193">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="eadcb-194">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="eadcb-194">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="eadcb-195">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-195">Int32</span></span>|<span data-ttu-id="eadcb-196">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-196">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="eadcb-197">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-197">Valid values 1 to 16</span></span>|
|<span data-ttu-id="eadcb-198">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="eadcb-198">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="eadcb-199">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-199">Int32</span></span>|<span data-ttu-id="eadcb-200">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-200">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="eadcb-201">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-201">Valid values 1 to 16</span></span>|
|<span data-ttu-id="eadcb-202">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="eadcb-202">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="eadcb-203">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-203">Int32</span></span>|<span data-ttu-id="eadcb-204">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-204">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="eadcb-205">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-205">Valid values 1 to 16</span></span>|
|<span data-ttu-id="eadcb-206">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="eadcb-206">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="eadcb-207">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-207">Int32</span></span>|<span data-ttu-id="eadcb-208">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-208">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="eadcb-209">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-209">Valid values 1 to 16</span></span>|
|<span data-ttu-id="eadcb-210">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="eadcb-210">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="eadcb-211">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-211">Int32</span></span>|<span data-ttu-id="eadcb-212">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-212">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="eadcb-213">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-213">Valid values 1 to 16</span></span>|
|<span data-ttu-id="eadcb-214">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="eadcb-214">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="eadcb-215">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-215">Int32</span></span>|<span data-ttu-id="eadcb-216">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eadcb-216">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="eadcb-217">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="eadcb-217">Valid values 1 to 16</span></span>|
|<span data-ttu-id="eadcb-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="eadcb-218">passwordRequiredType</span></span>|[<span data-ttu-id="eadcb-219">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="eadcb-219">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="eadcb-220">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="eadcb-220">Type of characters in password.</span></span> <span data-ttu-id="eadcb-221">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="eadcb-221">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="eadcb-222">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="eadcb-222">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="eadcb-223">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-223">Int32</span></span>|<span data-ttu-id="eadcb-224">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="eadcb-224">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="eadcb-225">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="eadcb-225">passwordExpirationDays</span></span>|<span data-ttu-id="eadcb-226">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-226">Int32</span></span>|<span data-ttu-id="eadcb-227">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="eadcb-227">Number of days before the password expires.</span></span> <span data-ttu-id="eadcb-228">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="eadcb-228">Valid values 1 to 365</span></span>|
|<span data-ttu-id="eadcb-229">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="eadcb-229">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="eadcb-230">Int32</span><span class="sxs-lookup"><span data-stu-id="eadcb-230">Int32</span></span>|<span data-ttu-id="eadcb-231">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="eadcb-231">Number of previous passwords to block.</span></span> <span data-ttu-id="eadcb-232">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="eadcb-232">Valid values 1 to 24</span></span>|
|<span data-ttu-id="eadcb-233">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="eadcb-233">storageRequireEncryption</span></span>|<span data-ttu-id="eadcb-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="eadcb-234">Boolean</span></span>|<span data-ttu-id="eadcb-235">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="eadcb-235">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="eadcb-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="eadcb-236">Response</span></span>
<span data-ttu-id="eadcb-237">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eadcb-237">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eadcb-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eadcb-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="eadcb-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eadcb-239">Request</span></span>
<span data-ttu-id="eadcb-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eadcb-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eadcb-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="eadcb-241">Response</span></span>
<span data-ttu-id="eadcb-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eadcb-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





