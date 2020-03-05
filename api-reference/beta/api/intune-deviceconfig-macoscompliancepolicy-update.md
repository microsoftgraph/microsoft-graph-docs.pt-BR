---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5095f6750e347f3d2ff83cb72878c175098a93c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442443"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="cd46f-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cd46f-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="cd46f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cd46f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd46f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd46f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd46f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd46f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd46f-107">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd46f-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd46f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd46f-108">Prerequisites</span></span>
<span data-ttu-id="cd46f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd46f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd46f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd46f-111">Permission type</span></span>|<span data-ttu-id="cd46f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd46f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd46f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd46f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd46f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd46f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd46f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd46f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd46f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd46f-116">Not supported.</span></span>|
|<span data-ttu-id="cd46f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd46f-117">Application</span></span>|<span data-ttu-id="cd46f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd46f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd46f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd46f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="cd46f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd46f-120">Request headers</span></span>
|<span data-ttu-id="cd46f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd46f-121">Header</span></span>|<span data-ttu-id="cd46f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cd46f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd46f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd46f-123">Authorization</span></span>|<span data-ttu-id="cd46f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd46f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd46f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd46f-125">Accept</span></span>|<span data-ttu-id="cd46f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd46f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd46f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd46f-127">Request body</span></span>
<span data-ttu-id="cd46f-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd46f-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="cd46f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd46f-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="cd46f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd46f-130">Property</span></span>|<span data-ttu-id="cd46f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd46f-131">Type</span></span>|<span data-ttu-id="cd46f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd46f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd46f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd46f-133">roleScopeTagIds</span></span>|<span data-ttu-id="cd46f-134">String collection</span><span class="sxs-lookup"><span data-stu-id="cd46f-134">String collection</span></span>|<span data-ttu-id="cd46f-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="cd46f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd46f-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-137">id</span><span class="sxs-lookup"><span data-stu-id="cd46f-137">id</span></span>|<span data-ttu-id="cd46f-138">String</span><span class="sxs-lookup"><span data-stu-id="cd46f-138">String</span></span>|<span data-ttu-id="cd46f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd46f-139">Key of the entity.</span></span> <span data-ttu-id="cd46f-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd46f-141">createdDateTime</span></span>|<span data-ttu-id="cd46f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd46f-142">DateTimeOffset</span></span>|<span data-ttu-id="cd46f-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cd46f-143">DateTime the object was created.</span></span> <span data-ttu-id="cd46f-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-145">description</span><span class="sxs-lookup"><span data-stu-id="cd46f-145">description</span></span>|<span data-ttu-id="cd46f-146">String</span><span class="sxs-lookup"><span data-stu-id="cd46f-146">String</span></span>|<span data-ttu-id="cd46f-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd46f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd46f-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd46f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="cd46f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd46f-150">DateTimeOffset</span></span>|<span data-ttu-id="cd46f-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cd46f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="cd46f-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="cd46f-153">displayName</span></span>|<span data-ttu-id="cd46f-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd46f-154">String</span></span>|<span data-ttu-id="cd46f-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd46f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd46f-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-157">version</span><span class="sxs-lookup"><span data-stu-id="cd46f-157">version</span></span>|<span data-ttu-id="cd46f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="cd46f-158">Int32</span></span>|<span data-ttu-id="cd46f-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd46f-159">Version of the device configuration.</span></span> <span data-ttu-id="cd46f-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd46f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cd46f-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cd46f-161">passwordRequired</span></span>|<span data-ttu-id="cd46f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd46f-162">Boolean</span></span>|<span data-ttu-id="cd46f-163">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="cd46f-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="cd46f-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cd46f-164">passwordBlockSimple</span></span>|<span data-ttu-id="cd46f-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd46f-165">Boolean</span></span>|<span data-ttu-id="cd46f-166">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="cd46f-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="cd46f-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cd46f-167">passwordExpirationDays</span></span>|<span data-ttu-id="cd46f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="cd46f-168">Int32</span></span>|<span data-ttu-id="cd46f-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="cd46f-169">Number of days before the password expires.</span></span> <span data-ttu-id="cd46f-170">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="cd46f-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="cd46f-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cd46f-171">passwordMinimumLength</span></span>|<span data-ttu-id="cd46f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="cd46f-172">Int32</span></span>|<span data-ttu-id="cd46f-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="cd46f-173">Minimum length of password.</span></span> <span data-ttu-id="cd46f-174">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="cd46f-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="cd46f-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cd46f-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cd46f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="cd46f-176">Int32</span></span>|<span data-ttu-id="cd46f-177">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="cd46f-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="cd46f-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cd46f-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cd46f-179">Int32</span><span class="sxs-lookup"><span data-stu-id="cd46f-179">Int32</span></span>|<span data-ttu-id="cd46f-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="cd46f-180">Number of previous passwords to block.</span></span> <span data-ttu-id="cd46f-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="cd46f-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cd46f-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cd46f-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cd46f-183">Int32</span><span class="sxs-lookup"><span data-stu-id="cd46f-183">Int32</span></span>|<span data-ttu-id="cd46f-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="cd46f-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="cd46f-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cd46f-185">passwordRequiredType</span></span>|[<span data-ttu-id="cd46f-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cd46f-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cd46f-187">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="cd46f-187">The required password type.</span></span> <span data-ttu-id="cd46f-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="cd46f-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cd46f-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cd46f-189">osMinimumVersion</span></span>|<span data-ttu-id="cd46f-190">String</span><span class="sxs-lookup"><span data-stu-id="cd46f-190">String</span></span>|<span data-ttu-id="cd46f-191">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="cd46f-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="cd46f-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cd46f-192">osMaximumVersion</span></span>|<span data-ttu-id="cd46f-193">String</span><span class="sxs-lookup"><span data-stu-id="cd46f-193">String</span></span>|<span data-ttu-id="cd46f-194">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="cd46f-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="cd46f-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="cd46f-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="cd46f-196">String</span><span class="sxs-lookup"><span data-stu-id="cd46f-196">String</span></span>|<span data-ttu-id="cd46f-197">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="cd46f-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="cd46f-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="cd46f-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="cd46f-199">String</span><span class="sxs-lookup"><span data-stu-id="cd46f-199">String</span></span>|<span data-ttu-id="cd46f-200">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="cd46f-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="cd46f-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cd46f-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="cd46f-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="cd46f-202">Boolean</span></span>|<span data-ttu-id="cd46f-203">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="cd46f-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="cd46f-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cd46f-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cd46f-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd46f-205">Boolean</span></span>|<span data-ttu-id="cd46f-206">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="cd46f-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="cd46f-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cd46f-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cd46f-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="cd46f-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cd46f-209">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="cd46f-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cd46f-210">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="cd46f-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cd46f-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="cd46f-211">storageRequireEncryption</span></span>|<span data-ttu-id="cd46f-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="cd46f-212">Boolean</span></span>|<span data-ttu-id="cd46f-213">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="cd46f-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="cd46f-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="cd46f-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="cd46f-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="cd46f-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="cd46f-216">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="cd46f-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="cd46f-217">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="cd46f-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="cd46f-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="cd46f-218">firewallEnabled</span></span>|<span data-ttu-id="cd46f-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd46f-219">Boolean</span></span>|<span data-ttu-id="cd46f-220">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="cd46f-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="cd46f-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="cd46f-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="cd46f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd46f-222">Boolean</span></span>|<span data-ttu-id="cd46f-223">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="cd46f-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="cd46f-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="cd46f-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="cd46f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd46f-225">Boolean</span></span>|<span data-ttu-id="cd46f-226">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="cd46f-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="cd46f-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd46f-227">Response</span></span>
<span data-ttu-id="cd46f-228">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd46f-228">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd46f-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd46f-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd46f-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd46f-230">Request</span></span>
<span data-ttu-id="cd46f-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd46f-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="cd46f-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd46f-232">Response</span></span>
<span data-ttu-id="cd46f-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd46f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





