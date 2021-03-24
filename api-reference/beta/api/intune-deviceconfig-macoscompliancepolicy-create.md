---
title: Criar macOSCompliancePolicy
description: Cria um novo objeto macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd41f34c4f2386ee48cb73361a53e5eed8a3beb1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129836"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="a59e0-103">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a59e0-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="a59e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a59e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a59e0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a59e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a59e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a59e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a59e0-107">Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a59e0-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a59e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a59e0-108">Prerequisites</span></span>
<span data-ttu-id="a59e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a59e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a59e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a59e0-111">Permission type</span></span>|<span data-ttu-id="a59e0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a59e0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a59e0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a59e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a59e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a59e0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a59e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a59e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a59e0-116">Not supported.</span></span>|
|<span data-ttu-id="a59e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a59e0-117">Application</span></span>|<span data-ttu-id="a59e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a59e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a59e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a59e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a59e0-120">Request headers</span></span>
|<span data-ttu-id="a59e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a59e0-121">Header</span></span>|<span data-ttu-id="a59e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a59e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a59e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a59e0-123">Authorization</span></span>|<span data-ttu-id="a59e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a59e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a59e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a59e0-125">Accept</span></span>|<span data-ttu-id="a59e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a59e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a59e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a59e0-127">Request body</span></span>
<span data-ttu-id="a59e0-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="a59e0-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="a59e0-129">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="a59e0-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="a59e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a59e0-130">Property</span></span>|<span data-ttu-id="a59e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a59e0-131">Type</span></span>|<span data-ttu-id="a59e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a59e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59e0-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a59e0-133">roleScopeTagIds</span></span>|<span data-ttu-id="a59e0-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59e0-134">String collection</span></span>|<span data-ttu-id="a59e0-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="a59e0-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a59e0-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-137">id</span><span class="sxs-lookup"><span data-stu-id="a59e0-137">id</span></span>|<span data-ttu-id="a59e0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59e0-138">String</span></span>|<span data-ttu-id="a59e0-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a59e0-139">Key of the entity.</span></span> <span data-ttu-id="a59e0-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a59e0-141">createdDateTime</span></span>|<span data-ttu-id="a59e0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59e0-142">DateTimeOffset</span></span>|<span data-ttu-id="a59e0-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a59e0-143">DateTime the object was created.</span></span> <span data-ttu-id="a59e0-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-145">descrição</span><span class="sxs-lookup"><span data-stu-id="a59e0-145">description</span></span>|<span data-ttu-id="a59e0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59e0-146">String</span></span>|<span data-ttu-id="a59e0-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a59e0-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a59e0-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a59e0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a59e0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59e0-150">DateTimeOffset</span></span>|<span data-ttu-id="a59e0-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a59e0-151">DateTime the object was last modified.</span></span> <span data-ttu-id="a59e0-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="a59e0-153">displayName</span></span>|<span data-ttu-id="a59e0-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59e0-154">String</span></span>|<span data-ttu-id="a59e0-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a59e0-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a59e0-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-157">version</span><span class="sxs-lookup"><span data-stu-id="a59e0-157">version</span></span>|<span data-ttu-id="a59e0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a59e0-158">Int32</span></span>|<span data-ttu-id="a59e0-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a59e0-159">Version of the device configuration.</span></span> <span data-ttu-id="a59e0-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a59e0-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a59e0-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a59e0-161">passwordRequired</span></span>|<span data-ttu-id="a59e0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a59e0-162">Boolean</span></span>|<span data-ttu-id="a59e0-163">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="a59e0-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="a59e0-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a59e0-164">passwordBlockSimple</span></span>|<span data-ttu-id="a59e0-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="a59e0-165">Boolean</span></span>|<span data-ttu-id="a59e0-166">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="a59e0-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="a59e0-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a59e0-167">passwordExpirationDays</span></span>|<span data-ttu-id="a59e0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a59e0-168">Int32</span></span>|<span data-ttu-id="a59e0-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="a59e0-169">Number of days before the password expires.</span></span> <span data-ttu-id="a59e0-170">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="a59e0-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a59e0-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a59e0-171">passwordMinimumLength</span></span>|<span data-ttu-id="a59e0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="a59e0-172">Int32</span></span>|<span data-ttu-id="a59e0-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="a59e0-173">Minimum length of password.</span></span> <span data-ttu-id="a59e0-174">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="a59e0-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="a59e0-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a59e0-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a59e0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a59e0-176">Int32</span></span>|<span data-ttu-id="a59e0-177">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="a59e0-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a59e0-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a59e0-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a59e0-179">Int32</span><span class="sxs-lookup"><span data-stu-id="a59e0-179">Int32</span></span>|<span data-ttu-id="a59e0-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="a59e0-180">Number of previous passwords to block.</span></span> <span data-ttu-id="a59e0-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="a59e0-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a59e0-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a59e0-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a59e0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a59e0-183">Int32</span></span>|<span data-ttu-id="a59e0-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="a59e0-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a59e0-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a59e0-185">passwordRequiredType</span></span>|[<span data-ttu-id="a59e0-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a59e0-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a59e0-187">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="a59e0-187">The required password type.</span></span> <span data-ttu-id="a59e0-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a59e0-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a59e0-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a59e0-189">osMinimumVersion</span></span>|<span data-ttu-id="a59e0-190">String</span><span class="sxs-lookup"><span data-stu-id="a59e0-190">String</span></span>|<span data-ttu-id="a59e0-191">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="a59e0-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="a59e0-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a59e0-192">osMaximumVersion</span></span>|<span data-ttu-id="a59e0-193">String</span><span class="sxs-lookup"><span data-stu-id="a59e0-193">String</span></span>|<span data-ttu-id="a59e0-194">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="a59e0-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="a59e0-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="a59e0-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="a59e0-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59e0-196">String</span></span>|<span data-ttu-id="a59e0-197">Versão mínima de com build do MacOS.</span><span class="sxs-lookup"><span data-stu-id="a59e0-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="a59e0-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="a59e0-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="a59e0-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59e0-199">String</span></span>|<span data-ttu-id="a59e0-200">Versão de composição máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="a59e0-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="a59e0-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a59e0-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="a59e0-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="a59e0-202">Boolean</span></span>|<span data-ttu-id="a59e0-203">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="a59e0-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="a59e0-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a59e0-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="a59e0-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="a59e0-205">Boolean</span></span>|<span data-ttu-id="a59e0-206">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="a59e0-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="a59e0-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a59e0-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="a59e0-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="a59e0-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="a59e0-209">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="a59e0-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="a59e0-210">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="a59e0-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="a59e0-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a59e0-211">storageRequireEncryption</span></span>|<span data-ttu-id="a59e0-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="a59e0-212">Boolean</span></span>|<span data-ttu-id="a59e0-213">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="a59e0-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="a59e0-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="a59e0-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="a59e0-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="a59e0-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="a59e0-216">Configuração de Sistema e Privacidade que determina de quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="a59e0-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="a59e0-217">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="a59e0-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="a59e0-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="a59e0-218">firewallEnabled</span></span>|<span data-ttu-id="a59e0-219">Booleano</span><span class="sxs-lookup"><span data-stu-id="a59e0-219">Boolean</span></span>|<span data-ttu-id="a59e0-220">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="a59e0-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="a59e0-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="a59e0-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="a59e0-222">Booleano</span><span class="sxs-lookup"><span data-stu-id="a59e0-222">Boolean</span></span>|<span data-ttu-id="a59e0-223">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="a59e0-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="a59e0-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="a59e0-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="a59e0-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="a59e0-225">Boolean</span></span>|<span data-ttu-id="a59e0-226">Corresponde a "Habilitar o modo de furtividade".</span><span class="sxs-lookup"><span data-stu-id="a59e0-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="a59e0-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59e0-227">Response</span></span>
<span data-ttu-id="a59e0-228">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a59e0-228">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a59e0-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a59e0-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="a59e0-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a59e0-230">Request</span></span>
<span data-ttu-id="a59e0-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a59e0-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1083

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
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="a59e0-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59e0-232">Response</span></span>
<span data-ttu-id="a59e0-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a59e0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1255

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
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```




