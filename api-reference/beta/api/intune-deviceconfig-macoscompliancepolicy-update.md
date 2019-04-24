---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2eb1e7835d0febcd608f8019557d6955065fab1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518979"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="21076-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="21076-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="21076-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21076-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21076-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21076-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21076-106">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="21076-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21076-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21076-107">Prerequisites</span></span>
<span data-ttu-id="21076-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21076-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21076-110">Permission type</span></span>|<span data-ttu-id="21076-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21076-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21076-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21076-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21076-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21076-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21076-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21076-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21076-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21076-115">Not supported.</span></span>|
|<span data-ttu-id="21076-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21076-116">Application</span></span>|<span data-ttu-id="21076-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21076-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21076-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21076-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="21076-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21076-119">Request headers</span></span>
|<span data-ttu-id="21076-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21076-120">Header</span></span>|<span data-ttu-id="21076-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21076-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21076-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21076-122">Authorization</span></span>|<span data-ttu-id="21076-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21076-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21076-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21076-124">Accept</span></span>|<span data-ttu-id="21076-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21076-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21076-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21076-126">Request body</span></span>
<span data-ttu-id="21076-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="21076-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="21076-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="21076-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="21076-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21076-129">Property</span></span>|<span data-ttu-id="21076-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="21076-130">Type</span></span>|<span data-ttu-id="21076-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="21076-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21076-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21076-132">roleScopeTagIds</span></span>|<span data-ttu-id="21076-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="21076-133">String collection</span></span>|<span data-ttu-id="21076-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="21076-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="21076-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-136">id</span><span class="sxs-lookup"><span data-stu-id="21076-136">id</span></span>|<span data-ttu-id="21076-137">String</span><span class="sxs-lookup"><span data-stu-id="21076-137">String</span></span>|<span data-ttu-id="21076-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21076-138">Key of the entity.</span></span> <span data-ttu-id="21076-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21076-140">createdDateTime</span></span>|<span data-ttu-id="21076-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21076-141">DateTimeOffset</span></span>|<span data-ttu-id="21076-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="21076-142">DateTime the object was created.</span></span> <span data-ttu-id="21076-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-144">description</span><span class="sxs-lookup"><span data-stu-id="21076-144">description</span></span>|<span data-ttu-id="21076-145">String</span><span class="sxs-lookup"><span data-stu-id="21076-145">String</span></span>|<span data-ttu-id="21076-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21076-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21076-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21076-148">lastModifiedDateTime</span></span>|<span data-ttu-id="21076-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21076-149">DateTimeOffset</span></span>|<span data-ttu-id="21076-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="21076-150">DateTime the object was last modified.</span></span> <span data-ttu-id="21076-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-152">displayName</span><span class="sxs-lookup"><span data-stu-id="21076-152">displayName</span></span>|<span data-ttu-id="21076-153">String</span><span class="sxs-lookup"><span data-stu-id="21076-153">String</span></span>|<span data-ttu-id="21076-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21076-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21076-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-156">version</span><span class="sxs-lookup"><span data-stu-id="21076-156">version</span></span>|<span data-ttu-id="21076-157">Int32</span><span class="sxs-lookup"><span data-stu-id="21076-157">Int32</span></span>|<span data-ttu-id="21076-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21076-158">Version of the device configuration.</span></span> <span data-ttu-id="21076-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="21076-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="21076-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="21076-160">passwordRequired</span></span>|<span data-ttu-id="21076-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="21076-161">Boolean</span></span>|<span data-ttu-id="21076-162">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="21076-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="21076-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="21076-163">passwordBlockSimple</span></span>|<span data-ttu-id="21076-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="21076-164">Boolean</span></span>|<span data-ttu-id="21076-165">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="21076-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="21076-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="21076-166">passwordExpirationDays</span></span>|<span data-ttu-id="21076-167">Int32</span><span class="sxs-lookup"><span data-stu-id="21076-167">Int32</span></span>|<span data-ttu-id="21076-168">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="21076-168">Number of days before the password expires.</span></span> <span data-ttu-id="21076-169">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="21076-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="21076-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="21076-170">passwordMinimumLength</span></span>|<span data-ttu-id="21076-171">Int32</span><span class="sxs-lookup"><span data-stu-id="21076-171">Int32</span></span>|<span data-ttu-id="21076-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="21076-172">Minimum length of password.</span></span> <span data-ttu-id="21076-173">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="21076-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="21076-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="21076-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="21076-175">Int32</span><span class="sxs-lookup"><span data-stu-id="21076-175">Int32</span></span>|<span data-ttu-id="21076-176">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="21076-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="21076-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="21076-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="21076-178">Int32</span><span class="sxs-lookup"><span data-stu-id="21076-178">Int32</span></span>|<span data-ttu-id="21076-179">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="21076-179">Number of previous passwords to block.</span></span> <span data-ttu-id="21076-180">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="21076-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="21076-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="21076-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="21076-182">Int32</span><span class="sxs-lookup"><span data-stu-id="21076-182">Int32</span></span>|<span data-ttu-id="21076-183">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="21076-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="21076-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="21076-184">passwordRequiredType</span></span>|[<span data-ttu-id="21076-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="21076-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="21076-186">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="21076-186">The required password type.</span></span> <span data-ttu-id="21076-187">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="21076-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="21076-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="21076-188">osMinimumVersion</span></span>|<span data-ttu-id="21076-189">String</span><span class="sxs-lookup"><span data-stu-id="21076-189">String</span></span>|<span data-ttu-id="21076-190">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="21076-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="21076-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="21076-191">osMaximumVersion</span></span>|<span data-ttu-id="21076-192">String</span><span class="sxs-lookup"><span data-stu-id="21076-192">String</span></span>|<span data-ttu-id="21076-193">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="21076-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="21076-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="21076-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="21076-195">String</span><span class="sxs-lookup"><span data-stu-id="21076-195">String</span></span>|<span data-ttu-id="21076-196">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="21076-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="21076-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="21076-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="21076-198">String</span><span class="sxs-lookup"><span data-stu-id="21076-198">String</span></span>|<span data-ttu-id="21076-199">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="21076-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="21076-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="21076-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="21076-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="21076-201">Boolean</span></span>|<span data-ttu-id="21076-202">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="21076-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="21076-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="21076-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="21076-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="21076-204">Boolean</span></span>|<span data-ttu-id="21076-205">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="21076-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="21076-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="21076-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="21076-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="21076-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="21076-208">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="21076-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="21076-209">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="21076-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="21076-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="21076-210">storageRequireEncryption</span></span>|<span data-ttu-id="21076-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="21076-211">Boolean</span></span>|<span data-ttu-id="21076-212">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="21076-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="21076-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="21076-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="21076-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="21076-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="21076-215">Configuração de sistema e privacidade que determina quais locais de download os aplicativos podem ser executados em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="21076-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="21076-216">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="21076-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="21076-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="21076-217">firewallEnabled</span></span>|<span data-ttu-id="21076-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="21076-218">Boolean</span></span>|<span data-ttu-id="21076-219">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="21076-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="21076-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="21076-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="21076-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="21076-221">Boolean</span></span>|<span data-ttu-id="21076-222">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="21076-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="21076-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="21076-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="21076-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="21076-224">Boolean</span></span>|<span data-ttu-id="21076-225">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="21076-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="21076-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="21076-226">Response</span></span>
<span data-ttu-id="21076-227">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21076-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21076-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21076-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="21076-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21076-229">Request</span></span>
<span data-ttu-id="21076-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21076-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21076-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="21076-231">Response</span></span>
<span data-ttu-id="21076-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21076-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





