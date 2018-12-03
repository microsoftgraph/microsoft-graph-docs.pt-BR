---
title: Atualizar windows10MobileCompliancePolicy
description: Atualiza as propriedades de um objeto windows10MobileCompliancePolicy.
ms.openlocfilehash: d98fb9497a59db3e6ef051142df0dd6444679918
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038992"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="23876-103">Atualizar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="23876-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="23876-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="23876-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23876-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="23876-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23876-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23876-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23876-107">Atualiza as propriedades de um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="23876-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23876-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23876-108">Prerequisites</span></span>
<span data-ttu-id="23876-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23876-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23876-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23876-111">Permission type</span></span>|<span data-ttu-id="23876-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23876-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23876-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23876-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23876-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23876-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23876-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23876-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23876-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23876-116">Not supported.</span></span>|
|<span data-ttu-id="23876-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23876-117">Application</span></span>|<span data-ttu-id="23876-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23876-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23876-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23876-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="23876-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23876-120">Request headers</span></span>
|<span data-ttu-id="23876-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23876-121">Header</span></span>|<span data-ttu-id="23876-122">Valor</span><span class="sxs-lookup"><span data-stu-id="23876-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23876-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23876-123">Authorization</span></span>|<span data-ttu-id="23876-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23876-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23876-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23876-125">Accept</span></span>|<span data-ttu-id="23876-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23876-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23876-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23876-127">Request body</span></span>
<span data-ttu-id="23876-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="23876-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="23876-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="23876-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="23876-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23876-130">Property</span></span>|<span data-ttu-id="23876-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="23876-131">Type</span></span>|<span data-ttu-id="23876-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="23876-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23876-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23876-133">roleScopeTagIds</span></span>|<span data-ttu-id="23876-134">String collection</span><span class="sxs-lookup"><span data-stu-id="23876-134">String collection</span></span>|<span data-ttu-id="23876-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="23876-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23876-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-137">id</span><span class="sxs-lookup"><span data-stu-id="23876-137">id</span></span>|<span data-ttu-id="23876-138">String</span><span class="sxs-lookup"><span data-stu-id="23876-138">String</span></span>|<span data-ttu-id="23876-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23876-139">Key of the entity.</span></span> <span data-ttu-id="23876-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23876-141">createdDateTime</span></span>|<span data-ttu-id="23876-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23876-142">DateTimeOffset</span></span>|<span data-ttu-id="23876-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="23876-143">DateTime the object was created.</span></span> <span data-ttu-id="23876-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-145">description</span><span class="sxs-lookup"><span data-stu-id="23876-145">description</span></span>|<span data-ttu-id="23876-146">String</span><span class="sxs-lookup"><span data-stu-id="23876-146">String</span></span>|<span data-ttu-id="23876-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23876-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23876-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23876-149">lastModifiedDateTime</span></span>|<span data-ttu-id="23876-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23876-150">DateTimeOffset</span></span>|<span data-ttu-id="23876-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="23876-151">DateTime the object was last modified.</span></span> <span data-ttu-id="23876-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-153">displayName</span><span class="sxs-lookup"><span data-stu-id="23876-153">displayName</span></span>|<span data-ttu-id="23876-154">String</span><span class="sxs-lookup"><span data-stu-id="23876-154">String</span></span>|<span data-ttu-id="23876-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23876-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23876-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-157">version</span><span class="sxs-lookup"><span data-stu-id="23876-157">version</span></span>|<span data-ttu-id="23876-158">Int32</span><span class="sxs-lookup"><span data-stu-id="23876-158">Int32</span></span>|<span data-ttu-id="23876-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23876-159">Version of the device configuration.</span></span> <span data-ttu-id="23876-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23876-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="23876-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="23876-161">passwordRequired</span></span>|<span data-ttu-id="23876-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-162">Boolean</span></span>|<span data-ttu-id="23876-163">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="23876-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="23876-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="23876-164">passwordBlockSimple</span></span>|<span data-ttu-id="23876-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-165">Boolean</span></span>|<span data-ttu-id="23876-166">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="23876-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="23876-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="23876-167">passwordMinimumLength</span></span>|<span data-ttu-id="23876-168">Int32</span><span class="sxs-lookup"><span data-stu-id="23876-168">Int32</span></span>|<span data-ttu-id="23876-169">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="23876-169">Minimum password length.</span></span> <span data-ttu-id="23876-170">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="23876-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="23876-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="23876-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="23876-172">Int32</span><span class="sxs-lookup"><span data-stu-id="23876-172">Int32</span></span>|<span data-ttu-id="23876-173">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="23876-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="23876-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="23876-174">passwordRequiredType</span></span>|[<span data-ttu-id="23876-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="23876-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="23876-176">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="23876-176">The required password type.</span></span> <span data-ttu-id="23876-177">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="23876-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="23876-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="23876-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="23876-179">Int32</span><span class="sxs-lookup"><span data-stu-id="23876-179">Int32</span></span>|<span data-ttu-id="23876-180">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="23876-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="23876-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="23876-181">passwordExpirationDays</span></span>|<span data-ttu-id="23876-182">Int32</span><span class="sxs-lookup"><span data-stu-id="23876-182">Int32</span></span>|<span data-ttu-id="23876-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="23876-183">Number of days before password expiration.</span></span> <span data-ttu-id="23876-184">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="23876-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="23876-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="23876-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="23876-186">Int32</span><span class="sxs-lookup"><span data-stu-id="23876-186">Int32</span></span>|<span data-ttu-id="23876-187">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="23876-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="23876-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="23876-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="23876-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-189">Boolean</span></span>|<span data-ttu-id="23876-190">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="23876-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="23876-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="23876-191">osMinimumVersion</span></span>|<span data-ttu-id="23876-192">String</span><span class="sxs-lookup"><span data-stu-id="23876-192">String</span></span>|<span data-ttu-id="23876-193">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="23876-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="23876-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="23876-194">osMaximumVersion</span></span>|<span data-ttu-id="23876-195">String</span><span class="sxs-lookup"><span data-stu-id="23876-195">String</span></span>|<span data-ttu-id="23876-196">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="23876-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="23876-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="23876-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-198">Boolean</span></span>|<span data-ttu-id="23876-199">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="23876-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="23876-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-200">bitLockerEnabled</span></span>|<span data-ttu-id="23876-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-201">Boolean</span></span>|<span data-ttu-id="23876-202">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="23876-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="23876-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-203">secureBootEnabled</span></span>|<span data-ttu-id="23876-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-204">Boolean</span></span>|<span data-ttu-id="23876-205">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="23876-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="23876-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="23876-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-207">Boolean</span></span>|<span data-ttu-id="23876-208">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="23876-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="23876-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="23876-209">storageRequireEncryption</span></span>|<span data-ttu-id="23876-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-210">Boolean</span></span>|<span data-ttu-id="23876-211">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="23876-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="23876-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="23876-212">activeFirewallRequired</span></span>|<span data-ttu-id="23876-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-213">Boolean</span></span>|<span data-ttu-id="23876-214">Exigir um firewall ativas em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="23876-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="23876-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="23876-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="23876-216">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="23876-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="23876-217">O sistema operacional válido criar intervalos em dispositivos do Windows.</span><span class="sxs-lookup"><span data-stu-id="23876-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="23876-218">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="23876-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="23876-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="23876-219">Response</span></span>
<span data-ttu-id="23876-220">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23876-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23876-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23876-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="23876-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23876-222">Request</span></span>
<span data-ttu-id="23876-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23876-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1152

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
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="23876-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="23876-224">Response</span></span>
<span data-ttu-id="23876-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23876-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```





