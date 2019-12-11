---
title: Criar windows10MobileCompliancePolicy
description: Cria um novo objeto windows10MobileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c7eda4ce05ded43e79ca20affe30425603aef01e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947376"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="43e24-103">Criar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="43e24-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="43e24-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43e24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43e24-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43e24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43e24-106">Cria um novo objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43e24-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43e24-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43e24-107">Prerequisites</span></span>
<span data-ttu-id="43e24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43e24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43e24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43e24-110">Permission type</span></span>|<span data-ttu-id="43e24-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43e24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43e24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43e24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43e24-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e24-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43e24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43e24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43e24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43e24-115">Not supported.</span></span>|
|<span data-ttu-id="43e24-116">Application</span><span class="sxs-lookup"><span data-stu-id="43e24-116">Application</span></span>|<span data-ttu-id="43e24-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e24-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43e24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43e24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="43e24-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43e24-119">Request headers</span></span>
|<span data-ttu-id="43e24-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43e24-120">Header</span></span>|<span data-ttu-id="43e24-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43e24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43e24-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43e24-122">Authorization</span></span>|<span data-ttu-id="43e24-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43e24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43e24-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43e24-124">Accept</span></span>|<span data-ttu-id="43e24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43e24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43e24-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43e24-126">Request body</span></span>
<span data-ttu-id="43e24-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="43e24-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="43e24-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="43e24-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="43e24-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43e24-129">Property</span></span>|<span data-ttu-id="43e24-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="43e24-130">Type</span></span>|<span data-ttu-id="43e24-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="43e24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43e24-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43e24-132">roleScopeTagIds</span></span>|<span data-ttu-id="43e24-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43e24-133">String collection</span></span>|<span data-ttu-id="43e24-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="43e24-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="43e24-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-136">id</span><span class="sxs-lookup"><span data-stu-id="43e24-136">id</span></span>|<span data-ttu-id="43e24-137">String</span><span class="sxs-lookup"><span data-stu-id="43e24-137">String</span></span>|<span data-ttu-id="43e24-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="43e24-138">Key of the entity.</span></span> <span data-ttu-id="43e24-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43e24-140">createdDateTime</span></span>|<span data-ttu-id="43e24-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43e24-141">DateTimeOffset</span></span>|<span data-ttu-id="43e24-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="43e24-142">DateTime the object was created.</span></span> <span data-ttu-id="43e24-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-144">description</span><span class="sxs-lookup"><span data-stu-id="43e24-144">description</span></span>|<span data-ttu-id="43e24-145">String</span><span class="sxs-lookup"><span data-stu-id="43e24-145">String</span></span>|<span data-ttu-id="43e24-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43e24-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43e24-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43e24-148">lastModifiedDateTime</span></span>|<span data-ttu-id="43e24-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43e24-149">DateTimeOffset</span></span>|<span data-ttu-id="43e24-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="43e24-150">DateTime the object was last modified.</span></span> <span data-ttu-id="43e24-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-152">displayName</span><span class="sxs-lookup"><span data-stu-id="43e24-152">displayName</span></span>|<span data-ttu-id="43e24-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43e24-153">String</span></span>|<span data-ttu-id="43e24-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43e24-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43e24-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-156">version</span><span class="sxs-lookup"><span data-stu-id="43e24-156">version</span></span>|<span data-ttu-id="43e24-157">Int32</span><span class="sxs-lookup"><span data-stu-id="43e24-157">Int32</span></span>|<span data-ttu-id="43e24-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43e24-158">Version of the device configuration.</span></span> <span data-ttu-id="43e24-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43e24-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="43e24-160">passwordRequired</span></span>|<span data-ttu-id="43e24-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-161">Boolean</span></span>|<span data-ttu-id="43e24-162">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="43e24-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="43e24-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="43e24-163">passwordBlockSimple</span></span>|<span data-ttu-id="43e24-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="43e24-164">Boolean</span></span>|<span data-ttu-id="43e24-165">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="43e24-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="43e24-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="43e24-166">passwordMinimumLength</span></span>|<span data-ttu-id="43e24-167">Int32</span><span class="sxs-lookup"><span data-stu-id="43e24-167">Int32</span></span>|<span data-ttu-id="43e24-168">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="43e24-168">Minimum password length.</span></span> <span data-ttu-id="43e24-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="43e24-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="43e24-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="43e24-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="43e24-171">Int32</span><span class="sxs-lookup"><span data-stu-id="43e24-171">Int32</span></span>|<span data-ttu-id="43e24-172">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="43e24-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="43e24-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="43e24-173">passwordRequiredType</span></span>|[<span data-ttu-id="43e24-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="43e24-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="43e24-175">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="43e24-175">The required password type.</span></span> <span data-ttu-id="43e24-176">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="43e24-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="43e24-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="43e24-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="43e24-178">Int32</span><span class="sxs-lookup"><span data-stu-id="43e24-178">Int32</span></span>|<span data-ttu-id="43e24-179">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="43e24-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="43e24-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="43e24-180">passwordExpirationDays</span></span>|<span data-ttu-id="43e24-181">Int32</span><span class="sxs-lookup"><span data-stu-id="43e24-181">Int32</span></span>|<span data-ttu-id="43e24-182">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="43e24-182">Number of days before password expiration.</span></span> <span data-ttu-id="43e24-183">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="43e24-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="43e24-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="43e24-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="43e24-185">Int32</span><span class="sxs-lookup"><span data-stu-id="43e24-185">Int32</span></span>|<span data-ttu-id="43e24-186">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="43e24-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="43e24-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="43e24-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="43e24-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="43e24-188">Boolean</span></span>|<span data-ttu-id="43e24-189">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="43e24-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="43e24-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="43e24-190">osMinimumVersion</span></span>|<span data-ttu-id="43e24-191">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="43e24-191">String</span></span>|<span data-ttu-id="43e24-192">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="43e24-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="43e24-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="43e24-193">osMaximumVersion</span></span>|<span data-ttu-id="43e24-194">String</span><span class="sxs-lookup"><span data-stu-id="43e24-194">String</span></span>|<span data-ttu-id="43e24-195">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="43e24-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="43e24-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="43e24-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="43e24-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-197">Boolean</span></span>|<span data-ttu-id="43e24-198">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="43e24-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="43e24-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="43e24-199">bitLockerEnabled</span></span>|<span data-ttu-id="43e24-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-200">Boolean</span></span>|<span data-ttu-id="43e24-201">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="43e24-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="43e24-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="43e24-202">secureBootEnabled</span></span>|<span data-ttu-id="43e24-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-203">Boolean</span></span>|<span data-ttu-id="43e24-204">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="43e24-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="43e24-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="43e24-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="43e24-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-206">Boolean</span></span>|<span data-ttu-id="43e24-207">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="43e24-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="43e24-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="43e24-208">storageRequireEncryption</span></span>|<span data-ttu-id="43e24-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-209">Boolean</span></span>|<span data-ttu-id="43e24-210">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="43e24-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="43e24-211">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="43e24-211">activeFirewallRequired</span></span>|<span data-ttu-id="43e24-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="43e24-212">Boolean</span></span>|<span data-ttu-id="43e24-213">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="43e24-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="43e24-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="43e24-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="43e24-215">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="43e24-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="43e24-216">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="43e24-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="43e24-217">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="43e24-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="43e24-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="43e24-218">Response</span></span>
<span data-ttu-id="43e24-219">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43e24-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43e24-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43e24-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="43e24-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43e24-221">Request</span></span>
<span data-ttu-id="43e24-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43e24-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="43e24-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="43e24-223">Response</span></span>
<span data-ttu-id="43e24-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43e24-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





