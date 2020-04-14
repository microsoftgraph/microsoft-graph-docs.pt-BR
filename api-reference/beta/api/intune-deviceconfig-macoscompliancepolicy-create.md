---
title: Criar macOSCompliancePolicy
description: Cria um novo objeto macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 337ed25504a45c9fd9d9248154862231c6963716
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438335"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="2fc01-103">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2fc01-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="2fc01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fc01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fc01-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2fc01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fc01-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fc01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fc01-107">Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2fc01-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fc01-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fc01-108">Prerequisites</span></span>
<span data-ttu-id="2fc01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fc01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fc01-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fc01-111">Permission type</span></span>|<span data-ttu-id="2fc01-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2fc01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fc01-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fc01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fc01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fc01-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fc01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fc01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fc01-116">Not supported.</span></span>|
|<span data-ttu-id="2fc01-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fc01-117">Application</span></span>|<span data-ttu-id="2fc01-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fc01-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fc01-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fc01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2fc01-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc01-120">Request headers</span></span>
|<span data-ttu-id="2fc01-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fc01-121">Header</span></span>|<span data-ttu-id="2fc01-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2fc01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fc01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fc01-123">Authorization</span></span>|<span data-ttu-id="2fc01-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fc01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fc01-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2fc01-125">Accept</span></span>|<span data-ttu-id="2fc01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fc01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fc01-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc01-127">Request body</span></span>
<span data-ttu-id="2fc01-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2fc01-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="2fc01-129">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2fc01-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="2fc01-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fc01-130">Property</span></span>|<span data-ttu-id="2fc01-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fc01-131">Type</span></span>|<span data-ttu-id="2fc01-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fc01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc01-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2fc01-133">roleScopeTagIds</span></span>|<span data-ttu-id="2fc01-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="2fc01-134">String collection</span></span>|<span data-ttu-id="2fc01-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2fc01-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2fc01-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-137">id</span><span class="sxs-lookup"><span data-stu-id="2fc01-137">id</span></span>|<span data-ttu-id="2fc01-138">String</span><span class="sxs-lookup"><span data-stu-id="2fc01-138">String</span></span>|<span data-ttu-id="2fc01-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2fc01-139">Key of the entity.</span></span> <span data-ttu-id="2fc01-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc01-141">createdDateTime</span></span>|<span data-ttu-id="2fc01-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc01-142">DateTimeOffset</span></span>|<span data-ttu-id="2fc01-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2fc01-143">DateTime the object was created.</span></span> <span data-ttu-id="2fc01-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-145">description</span><span class="sxs-lookup"><span data-stu-id="2fc01-145">description</span></span>|<span data-ttu-id="2fc01-146">String</span><span class="sxs-lookup"><span data-stu-id="2fc01-146">String</span></span>|<span data-ttu-id="2fc01-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2fc01-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2fc01-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fc01-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2fc01-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fc01-150">DateTimeOffset</span></span>|<span data-ttu-id="2fc01-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2fc01-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2fc01-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2fc01-153">displayName</span></span>|<span data-ttu-id="2fc01-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fc01-154">String</span></span>|<span data-ttu-id="2fc01-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2fc01-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2fc01-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-157">version</span><span class="sxs-lookup"><span data-stu-id="2fc01-157">version</span></span>|<span data-ttu-id="2fc01-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc01-158">Int32</span></span>|<span data-ttu-id="2fc01-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2fc01-159">Version of the device configuration.</span></span> <span data-ttu-id="2fc01-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fc01-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2fc01-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2fc01-161">passwordRequired</span></span>|<span data-ttu-id="2fc01-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc01-162">Boolean</span></span>|<span data-ttu-id="2fc01-163">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="2fc01-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="2fc01-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2fc01-164">passwordBlockSimple</span></span>|<span data-ttu-id="2fc01-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc01-165">Boolean</span></span>|<span data-ttu-id="2fc01-166">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="2fc01-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="2fc01-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2fc01-167">passwordExpirationDays</span></span>|<span data-ttu-id="2fc01-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc01-168">Int32</span></span>|<span data-ttu-id="2fc01-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="2fc01-169">Number of days before the password expires.</span></span> <span data-ttu-id="2fc01-170">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="2fc01-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="2fc01-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2fc01-171">passwordMinimumLength</span></span>|<span data-ttu-id="2fc01-172">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc01-172">Int32</span></span>|<span data-ttu-id="2fc01-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="2fc01-173">Minimum length of password.</span></span> <span data-ttu-id="2fc01-174">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="2fc01-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="2fc01-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2fc01-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2fc01-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc01-176">Int32</span></span>|<span data-ttu-id="2fc01-177">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="2fc01-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2fc01-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2fc01-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2fc01-179">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc01-179">Int32</span></span>|<span data-ttu-id="2fc01-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="2fc01-180">Number of previous passwords to block.</span></span> <span data-ttu-id="2fc01-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="2fc01-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="2fc01-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2fc01-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2fc01-183">Int32</span><span class="sxs-lookup"><span data-stu-id="2fc01-183">Int32</span></span>|<span data-ttu-id="2fc01-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="2fc01-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2fc01-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2fc01-185">passwordRequiredType</span></span>|[<span data-ttu-id="2fc01-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2fc01-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2fc01-187">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="2fc01-187">The required password type.</span></span> <span data-ttu-id="2fc01-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2fc01-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2fc01-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2fc01-189">osMinimumVersion</span></span>|<span data-ttu-id="2fc01-190">String</span><span class="sxs-lookup"><span data-stu-id="2fc01-190">String</span></span>|<span data-ttu-id="2fc01-191">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="2fc01-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="2fc01-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2fc01-192">osMaximumVersion</span></span>|<span data-ttu-id="2fc01-193">String</span><span class="sxs-lookup"><span data-stu-id="2fc01-193">String</span></span>|<span data-ttu-id="2fc01-194">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="2fc01-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="2fc01-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="2fc01-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="2fc01-196">String</span><span class="sxs-lookup"><span data-stu-id="2fc01-196">String</span></span>|<span data-ttu-id="2fc01-197">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="2fc01-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="2fc01-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="2fc01-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="2fc01-199">String</span><span class="sxs-lookup"><span data-stu-id="2fc01-199">String</span></span>|<span data-ttu-id="2fc01-200">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="2fc01-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="2fc01-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2fc01-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="2fc01-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="2fc01-202">Boolean</span></span>|<span data-ttu-id="2fc01-203">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="2fc01-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="2fc01-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2fc01-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2fc01-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc01-205">Boolean</span></span>|<span data-ttu-id="2fc01-206">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="2fc01-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="2fc01-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2fc01-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2fc01-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2fc01-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2fc01-209">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2fc01-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2fc01-210">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="2fc01-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2fc01-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2fc01-211">storageRequireEncryption</span></span>|<span data-ttu-id="2fc01-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="2fc01-212">Boolean</span></span>|<span data-ttu-id="2fc01-213">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2fc01-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="2fc01-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="2fc01-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="2fc01-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="2fc01-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="2fc01-216">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="2fc01-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="2fc01-217">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="2fc01-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="2fc01-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="2fc01-218">firewallEnabled</span></span>|<span data-ttu-id="2fc01-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc01-219">Boolean</span></span>|<span data-ttu-id="2fc01-220">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="2fc01-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="2fc01-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="2fc01-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="2fc01-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc01-222">Boolean</span></span>|<span data-ttu-id="2fc01-223">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="2fc01-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="2fc01-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="2fc01-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="2fc01-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc01-225">Boolean</span></span>|<span data-ttu-id="2fc01-226">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="2fc01-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="2fc01-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fc01-227">Response</span></span>
<span data-ttu-id="2fc01-228">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fc01-228">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fc01-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fc01-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fc01-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fc01-230">Request</span></span>
<span data-ttu-id="2fc01-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fc01-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fc01-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fc01-232">Response</span></span>
<span data-ttu-id="2fc01-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fc01-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



