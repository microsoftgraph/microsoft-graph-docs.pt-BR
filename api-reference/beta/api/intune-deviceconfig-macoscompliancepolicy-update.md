---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4eae08b154553b78b987ca65dc22a8e8fff12eb8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864057"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="0f5d2-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0f5d2-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="0f5d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f5d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f5d2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f5d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f5d2-107">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f5d2-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f5d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f5d2-108">Prerequisites</span></span>
<span data-ttu-id="0f5d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f5d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f5d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f5d2-111">Permission type</span></span>|<span data-ttu-id="0f5d2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f5d2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f5d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f5d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f5d2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f5d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-116">Not supported.</span></span>|
|<span data-ttu-id="0f5d2-117">Application</span><span class="sxs-lookup"><span data-stu-id="0f5d2-117">Application</span></span>|<span data-ttu-id="0f5d2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f5d2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f5d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f5d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0f5d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f5d2-120">Request headers</span></span>
|<span data-ttu-id="0f5d2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f5d2-121">Header</span></span>|<span data-ttu-id="0f5d2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f5d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f5d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f5d2-123">Authorization</span></span>|<span data-ttu-id="0f5d2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f5d2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f5d2-125">Accept</span></span>|<span data-ttu-id="0f5d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f5d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f5d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f5d2-127">Request body</span></span>
<span data-ttu-id="0f5d2-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f5d2-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="0f5d2-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f5d2-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="0f5d2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f5d2-130">Property</span></span>|<span data-ttu-id="0f5d2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f5d2-131">Type</span></span>|<span data-ttu-id="0f5d2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f5d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f5d2-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f5d2-133">roleScopeTagIds</span></span>|<span data-ttu-id="0f5d2-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0f5d2-134">String collection</span></span>|<span data-ttu-id="0f5d2-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f5d2-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-137">id</span><span class="sxs-lookup"><span data-stu-id="0f5d2-137">id</span></span>|<span data-ttu-id="0f5d2-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f5d2-138">String</span></span>|<span data-ttu-id="0f5d2-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-139">Key of the entity.</span></span> <span data-ttu-id="0f5d2-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f5d2-141">createdDateTime</span></span>|<span data-ttu-id="0f5d2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f5d2-142">DateTimeOffset</span></span>|<span data-ttu-id="0f5d2-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-143">DateTime the object was created.</span></span> <span data-ttu-id="0f5d2-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-145">description</span><span class="sxs-lookup"><span data-stu-id="0f5d2-145">description</span></span>|<span data-ttu-id="0f5d2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f5d2-146">String</span></span>|<span data-ttu-id="0f5d2-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f5d2-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f5d2-149">lastModifiedDateTime</span></span>|<span data-ttu-id="0f5d2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f5d2-150">DateTimeOffset</span></span>|<span data-ttu-id="0f5d2-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-151">DateTime the object was last modified.</span></span> <span data-ttu-id="0f5d2-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0f5d2-153">displayName</span></span>|<span data-ttu-id="0f5d2-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f5d2-154">String</span></span>|<span data-ttu-id="0f5d2-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f5d2-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-157">version</span><span class="sxs-lookup"><span data-stu-id="0f5d2-157">version</span></span>|<span data-ttu-id="0f5d2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5d2-158">Int32</span></span>|<span data-ttu-id="0f5d2-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-159">Version of the device configuration.</span></span> <span data-ttu-id="0f5d2-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f5d2-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0f5d2-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0f5d2-161">passwordRequired</span></span>|<span data-ttu-id="0f5d2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5d2-162">Boolean</span></span>|<span data-ttu-id="0f5d2-163">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0f5d2-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0f5d2-164">passwordBlockSimple</span></span>|<span data-ttu-id="0f5d2-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f5d2-165">Boolean</span></span>|<span data-ttu-id="0f5d2-166">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="0f5d2-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0f5d2-167">passwordExpirationDays</span></span>|<span data-ttu-id="0f5d2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5d2-168">Int32</span></span>|<span data-ttu-id="0f5d2-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-169">Number of days before the password expires.</span></span> <span data-ttu-id="0f5d2-170">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="0f5d2-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0f5d2-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0f5d2-171">passwordMinimumLength</span></span>|<span data-ttu-id="0f5d2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5d2-172">Int32</span></span>|<span data-ttu-id="0f5d2-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-173">Minimum length of password.</span></span> <span data-ttu-id="0f5d2-174">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="0f5d2-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0f5d2-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0f5d2-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0f5d2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5d2-176">Int32</span></span>|<span data-ttu-id="0f5d2-177">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0f5d2-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0f5d2-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0f5d2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5d2-179">Int32</span></span>|<span data-ttu-id="0f5d2-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-180">Number of previous passwords to block.</span></span> <span data-ttu-id="0f5d2-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="0f5d2-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0f5d2-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0f5d2-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0f5d2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5d2-183">Int32</span></span>|<span data-ttu-id="0f5d2-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0f5d2-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0f5d2-185">passwordRequiredType</span></span>|[<span data-ttu-id="0f5d2-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0f5d2-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0f5d2-187">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-187">The required password type.</span></span> <span data-ttu-id="0f5d2-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0f5d2-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0f5d2-189">osMinimumVersion</span></span>|<span data-ttu-id="0f5d2-190">String</span><span class="sxs-lookup"><span data-stu-id="0f5d2-190">String</span></span>|<span data-ttu-id="0f5d2-191">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="0f5d2-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0f5d2-192">osMaximumVersion</span></span>|<span data-ttu-id="0f5d2-193">String</span><span class="sxs-lookup"><span data-stu-id="0f5d2-193">String</span></span>|<span data-ttu-id="0f5d2-194">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="0f5d2-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0f5d2-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="0f5d2-196">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0f5d2-196">String</span></span>|<span data-ttu-id="0f5d2-197">Versão mínima de com build do MacOS.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="0f5d2-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0f5d2-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="0f5d2-199">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0f5d2-199">String</span></span>|<span data-ttu-id="0f5d2-200">Versão de composição máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="0f5d2-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0f5d2-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="0f5d2-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f5d2-202">Boolean</span></span>|<span data-ttu-id="0f5d2-203">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="0f5d2-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0f5d2-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0f5d2-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5d2-205">Boolean</span></span>|<span data-ttu-id="0f5d2-206">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0f5d2-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0f5d2-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0f5d2-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0f5d2-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0f5d2-209">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0f5d2-210">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0f5d2-211">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0f5d2-211">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0f5d2-212">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0f5d2-212">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0f5d2-213">O MDATP exige nível mínimo de risco da Proteção Contra Ameaças Móveis para relatar o não-atendimento.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-213">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0f5d2-214">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-214">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0f5d2-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0f5d2-215">storageRequireEncryption</span></span>|<span data-ttu-id="0f5d2-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f5d2-216">Boolean</span></span>|<span data-ttu-id="0f5d2-217">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-217">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="0f5d2-218">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="0f5d2-218">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="0f5d2-219">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="0f5d2-219">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="0f5d2-220">Configuração de Sistema e Privacidade que determina de quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-220">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="0f5d2-221">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-221">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="0f5d2-222">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0f5d2-222">firewallEnabled</span></span>|<span data-ttu-id="0f5d2-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5d2-223">Boolean</span></span>|<span data-ttu-id="0f5d2-224">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-224">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0f5d2-225">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0f5d2-225">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0f5d2-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5d2-226">Boolean</span></span>|<span data-ttu-id="0f5d2-227">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="0f5d2-227">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0f5d2-228">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0f5d2-228">firewallEnableStealthMode</span></span>|<span data-ttu-id="0f5d2-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5d2-229">Boolean</span></span>|<span data-ttu-id="0f5d2-230">Corresponde a "Habilitar o modo de furtividade".</span><span class="sxs-lookup"><span data-stu-id="0f5d2-230">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="0f5d2-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f5d2-231">Response</span></span>
<span data-ttu-id="0f5d2-232">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-232">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f5d2-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f5d2-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f5d2-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f5d2-234">Request</span></span>
<span data-ttu-id="0f5d2-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1146

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="0f5d2-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f5d2-236">Response</span></span>
<span data-ttu-id="0f5d2-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f5d2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```




