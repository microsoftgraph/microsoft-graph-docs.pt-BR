---
title: Criar macOSCompliancePolicy
description: Cria um novo objeto macOSCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6d3762f4e8334789aaa6a4958f90c4c710f8f08
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178904"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="416b0-103">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="416b0-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="416b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="416b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="416b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="416b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="416b0-106">Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="416b0-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="416b0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="416b0-107">Prerequisites</span></span>
<span data-ttu-id="416b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="416b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="416b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="416b0-110">Permission type</span></span>|<span data-ttu-id="416b0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="416b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="416b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="416b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="416b0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="416b0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="416b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="416b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="416b0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="416b0-115">Not supported.</span></span>|
|<span data-ttu-id="416b0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="416b0-116">Application</span></span>|<span data-ttu-id="416b0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="416b0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="416b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="416b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="416b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="416b0-119">Request headers</span></span>
|<span data-ttu-id="416b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="416b0-120">Header</span></span>|<span data-ttu-id="416b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="416b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="416b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="416b0-122">Authorization</span></span>|<span data-ttu-id="416b0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="416b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="416b0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="416b0-124">Accept</span></span>|<span data-ttu-id="416b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="416b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="416b0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="416b0-126">Request body</span></span>
<span data-ttu-id="416b0-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="416b0-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="416b0-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="416b0-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="416b0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="416b0-129">Property</span></span>|<span data-ttu-id="416b0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="416b0-130">Type</span></span>|<span data-ttu-id="416b0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="416b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="416b0-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="416b0-132">roleScopeTagIds</span></span>|<span data-ttu-id="416b0-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="416b0-133">String collection</span></span>|<span data-ttu-id="416b0-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="416b0-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="416b0-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-136">id</span><span class="sxs-lookup"><span data-stu-id="416b0-136">id</span></span>|<span data-ttu-id="416b0-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="416b0-137">String</span></span>|<span data-ttu-id="416b0-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="416b0-138">Key of the entity.</span></span> <span data-ttu-id="416b0-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="416b0-140">createdDateTime</span></span>|<span data-ttu-id="416b0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="416b0-141">DateTimeOffset</span></span>|<span data-ttu-id="416b0-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="416b0-142">DateTime the object was created.</span></span> <span data-ttu-id="416b0-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-144">descrição</span><span class="sxs-lookup"><span data-stu-id="416b0-144">description</span></span>|<span data-ttu-id="416b0-145">String</span><span class="sxs-lookup"><span data-stu-id="416b0-145">String</span></span>|<span data-ttu-id="416b0-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="416b0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="416b0-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="416b0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="416b0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="416b0-149">DateTimeOffset</span></span>|<span data-ttu-id="416b0-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="416b0-150">DateTime the object was last modified.</span></span> <span data-ttu-id="416b0-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-152">displayName</span><span class="sxs-lookup"><span data-stu-id="416b0-152">displayName</span></span>|<span data-ttu-id="416b0-153">String</span><span class="sxs-lookup"><span data-stu-id="416b0-153">String</span></span>|<span data-ttu-id="416b0-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="416b0-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="416b0-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-156">version</span><span class="sxs-lookup"><span data-stu-id="416b0-156">version</span></span>|<span data-ttu-id="416b0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="416b0-157">Int32</span></span>|<span data-ttu-id="416b0-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="416b0-158">Version of the device configuration.</span></span> <span data-ttu-id="416b0-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="416b0-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="416b0-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="416b0-160">passwordRequired</span></span>|<span data-ttu-id="416b0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="416b0-161">Boolean</span></span>|<span data-ttu-id="416b0-162">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="416b0-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="416b0-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="416b0-163">passwordBlockSimple</span></span>|<span data-ttu-id="416b0-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="416b0-164">Boolean</span></span>|<span data-ttu-id="416b0-165">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="416b0-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="416b0-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="416b0-166">passwordExpirationDays</span></span>|<span data-ttu-id="416b0-167">Int32</span><span class="sxs-lookup"><span data-stu-id="416b0-167">Int32</span></span>|<span data-ttu-id="416b0-168">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="416b0-168">Number of days before the password expires.</span></span> <span data-ttu-id="416b0-169">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="416b0-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="416b0-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="416b0-170">passwordMinimumLength</span></span>|<span data-ttu-id="416b0-171">Int32</span><span class="sxs-lookup"><span data-stu-id="416b0-171">Int32</span></span>|<span data-ttu-id="416b0-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="416b0-172">Minimum length of password.</span></span> <span data-ttu-id="416b0-173">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="416b0-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="416b0-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="416b0-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="416b0-175">Int32</span><span class="sxs-lookup"><span data-stu-id="416b0-175">Int32</span></span>|<span data-ttu-id="416b0-176">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="416b0-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="416b0-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="416b0-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="416b0-178">Int32</span><span class="sxs-lookup"><span data-stu-id="416b0-178">Int32</span></span>|<span data-ttu-id="416b0-179">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="416b0-179">Number of previous passwords to block.</span></span> <span data-ttu-id="416b0-180">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="416b0-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="416b0-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="416b0-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="416b0-182">Int32</span><span class="sxs-lookup"><span data-stu-id="416b0-182">Int32</span></span>|<span data-ttu-id="416b0-183">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="416b0-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="416b0-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="416b0-184">passwordRequiredType</span></span>|[<span data-ttu-id="416b0-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="416b0-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="416b0-186">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="416b0-186">The required password type.</span></span> <span data-ttu-id="416b0-187">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="416b0-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="416b0-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="416b0-188">osMinimumVersion</span></span>|<span data-ttu-id="416b0-189">String</span><span class="sxs-lookup"><span data-stu-id="416b0-189">String</span></span>|<span data-ttu-id="416b0-190">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="416b0-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="416b0-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="416b0-191">osMaximumVersion</span></span>|<span data-ttu-id="416b0-192">String</span><span class="sxs-lookup"><span data-stu-id="416b0-192">String</span></span>|<span data-ttu-id="416b0-193">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="416b0-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="416b0-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="416b0-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="416b0-195">String</span><span class="sxs-lookup"><span data-stu-id="416b0-195">String</span></span>|<span data-ttu-id="416b0-196">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="416b0-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="416b0-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="416b0-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="416b0-198">String</span><span class="sxs-lookup"><span data-stu-id="416b0-198">String</span></span>|<span data-ttu-id="416b0-199">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="416b0-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="416b0-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="416b0-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="416b0-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="416b0-201">Boolean</span></span>|<span data-ttu-id="416b0-202">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="416b0-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="416b0-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="416b0-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="416b0-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="416b0-204">Boolean</span></span>|<span data-ttu-id="416b0-205">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="416b0-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="416b0-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="416b0-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="416b0-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="416b0-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="416b0-208">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="416b0-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="416b0-209">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="416b0-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="416b0-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="416b0-210">storageRequireEncryption</span></span>|<span data-ttu-id="416b0-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="416b0-211">Boolean</span></span>|<span data-ttu-id="416b0-212">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="416b0-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="416b0-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="416b0-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="416b0-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="416b0-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="416b0-215">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="416b0-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="416b0-216">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="416b0-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="416b0-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="416b0-217">firewallEnabled</span></span>|<span data-ttu-id="416b0-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="416b0-218">Boolean</span></span>|<span data-ttu-id="416b0-219">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="416b0-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="416b0-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="416b0-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="416b0-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="416b0-221">Boolean</span></span>|<span data-ttu-id="416b0-222">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="416b0-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="416b0-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="416b0-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="416b0-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="416b0-224">Boolean</span></span>|<span data-ttu-id="416b0-225">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="416b0-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="416b0-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="416b0-226">Response</span></span>
<span data-ttu-id="416b0-227">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="416b0-227">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="416b0-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="416b0-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="416b0-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="416b0-229">Request</span></span>
<span data-ttu-id="416b0-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="416b0-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="416b0-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="416b0-231">Response</span></span>
<span data-ttu-id="416b0-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="416b0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




