---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
ms.openlocfilehash: 73e6d4d3fb0d24699e22b87dc3489a17e1287bd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037952"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="ef124-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ef124-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="ef124-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef124-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef124-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef124-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef124-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef124-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef124-107">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef124-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef124-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef124-108">Prerequisites</span></span>
<span data-ttu-id="ef124-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef124-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef124-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef124-111">Permission type</span></span>|<span data-ttu-id="ef124-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef124-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef124-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef124-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef124-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef124-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef124-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef124-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef124-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef124-116">Not supported.</span></span>|
|<span data-ttu-id="ef124-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef124-117">Application</span></span>|<span data-ttu-id="ef124-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef124-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef124-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef124-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ef124-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef124-120">Request headers</span></span>
|<span data-ttu-id="ef124-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef124-121">Header</span></span>|<span data-ttu-id="ef124-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef124-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef124-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef124-123">Authorization</span></span>|<span data-ttu-id="ef124-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef124-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef124-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef124-125">Accept</span></span>|<span data-ttu-id="ef124-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef124-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef124-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef124-127">Request body</span></span>
<span data-ttu-id="ef124-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef124-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="ef124-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ef124-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="ef124-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef124-130">Property</span></span>|<span data-ttu-id="ef124-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef124-131">Type</span></span>|<span data-ttu-id="ef124-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef124-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef124-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef124-133">roleScopeTagIds</span></span>|<span data-ttu-id="ef124-134">String collection</span><span class="sxs-lookup"><span data-stu-id="ef124-134">String collection</span></span>|<span data-ttu-id="ef124-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef124-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef124-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-137">id</span><span class="sxs-lookup"><span data-stu-id="ef124-137">id</span></span>|<span data-ttu-id="ef124-138">String</span><span class="sxs-lookup"><span data-stu-id="ef124-138">String</span></span>|<span data-ttu-id="ef124-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef124-139">Key of the entity.</span></span> <span data-ttu-id="ef124-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef124-141">createdDateTime</span></span>|<span data-ttu-id="ef124-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef124-142">DateTimeOffset</span></span>|<span data-ttu-id="ef124-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ef124-143">DateTime the object was created.</span></span> <span data-ttu-id="ef124-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-145">description</span><span class="sxs-lookup"><span data-stu-id="ef124-145">description</span></span>|<span data-ttu-id="ef124-146">String</span><span class="sxs-lookup"><span data-stu-id="ef124-146">String</span></span>|<span data-ttu-id="ef124-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef124-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef124-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef124-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ef124-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef124-150">DateTimeOffset</span></span>|<span data-ttu-id="ef124-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef124-151">DateTime the object was last modified.</span></span> <span data-ttu-id="ef124-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ef124-153">displayName</span></span>|<span data-ttu-id="ef124-154">String</span><span class="sxs-lookup"><span data-stu-id="ef124-154">String</span></span>|<span data-ttu-id="ef124-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef124-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef124-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-157">version</span><span class="sxs-lookup"><span data-stu-id="ef124-157">version</span></span>|<span data-ttu-id="ef124-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ef124-158">Int32</span></span>|<span data-ttu-id="ef124-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef124-159">Version of the device configuration.</span></span> <span data-ttu-id="ef124-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ef124-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ef124-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ef124-161">passwordRequired</span></span>|<span data-ttu-id="ef124-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-162">Boolean</span></span>|<span data-ttu-id="ef124-163">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="ef124-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="ef124-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ef124-164">passwordBlockSimple</span></span>|<span data-ttu-id="ef124-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-165">Boolean</span></span>|<span data-ttu-id="ef124-166">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="ef124-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="ef124-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ef124-167">passwordExpirationDays</span></span>|<span data-ttu-id="ef124-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ef124-168">Int32</span></span>|<span data-ttu-id="ef124-169">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="ef124-169">Number of days before the password expires.</span></span> <span data-ttu-id="ef124-170">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="ef124-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ef124-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ef124-171">passwordMinimumLength</span></span>|<span data-ttu-id="ef124-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ef124-172">Int32</span></span>|<span data-ttu-id="ef124-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="ef124-173">Minimum length of password.</span></span> <span data-ttu-id="ef124-174">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="ef124-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ef124-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ef124-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ef124-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ef124-176">Int32</span></span>|<span data-ttu-id="ef124-177">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="ef124-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ef124-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ef124-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ef124-179">Int32</span><span class="sxs-lookup"><span data-stu-id="ef124-179">Int32</span></span>|<span data-ttu-id="ef124-180">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ef124-180">Number of previous passwords to block.</span></span> <span data-ttu-id="ef124-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="ef124-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ef124-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ef124-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ef124-183">Int32</span><span class="sxs-lookup"><span data-stu-id="ef124-183">Int32</span></span>|<span data-ttu-id="ef124-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="ef124-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ef124-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ef124-185">passwordRequiredType</span></span>|[<span data-ttu-id="ef124-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ef124-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ef124-187">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="ef124-187">The required password type.</span></span> <span data-ttu-id="ef124-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ef124-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ef124-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ef124-189">osMinimumVersion</span></span>|<span data-ttu-id="ef124-190">String</span><span class="sxs-lookup"><span data-stu-id="ef124-190">String</span></span>|<span data-ttu-id="ef124-191">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="ef124-191">Minimum IOS version.</span></span>|
|<span data-ttu-id="ef124-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ef124-192">osMaximumVersion</span></span>|<span data-ttu-id="ef124-193">String</span><span class="sxs-lookup"><span data-stu-id="ef124-193">String</span></span>|<span data-ttu-id="ef124-194">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="ef124-194">Maximum IOS version.</span></span>|
|<span data-ttu-id="ef124-195">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ef124-195">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="ef124-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-196">Boolean</span></span>|<span data-ttu-id="ef124-197">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="ef124-197">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="ef124-198">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ef124-198">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ef124-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-199">Boolean</span></span>|<span data-ttu-id="ef124-200">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="ef124-200">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="ef124-201">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ef124-201">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ef124-202">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ef124-202">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ef124-203">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="ef124-203">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ef124-204">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ef124-204">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ef124-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ef124-205">storageRequireEncryption</span></span>|<span data-ttu-id="ef124-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-206">Boolean</span></span>|<span data-ttu-id="ef124-207">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="ef124-207">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="ef124-208">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="ef124-208">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="ef124-209">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="ef124-209">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="ef124-210">Sistema e configuração de privacidade que determina quais aplicativos de locais de download podem ser executados de em um dispositivo macOS.</span><span class="sxs-lookup"><span data-stu-id="ef124-210">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="ef124-211">Os valores possíveis são: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="ef124-211">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="ef124-212">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="ef124-212">firewallEnabled</span></span>|<span data-ttu-id="ef124-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-213">Boolean</span></span>|<span data-ttu-id="ef124-214">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="ef124-214">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="ef124-215">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="ef124-215">firewallBlockAllIncoming</span></span>|<span data-ttu-id="ef124-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-216">Boolean</span></span>|<span data-ttu-id="ef124-217">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="ef124-217">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="ef124-218">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="ef124-218">firewallEnableStealthMode</span></span>|<span data-ttu-id="ef124-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef124-219">Boolean</span></span>|<span data-ttu-id="ef124-220">Corresponde ao "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="ef124-220">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="ef124-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef124-221">Response</span></span>
<span data-ttu-id="ef124-222">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef124-222">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef124-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef124-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef124-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef124-224">Request</span></span>
<span data-ttu-id="ef124-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef124-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 963

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="ef124-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef124-226">Response</span></span>
<span data-ttu-id="ef124-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef124-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1131

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





