---
title: Criar windows10MobileCompliancePolicy
description: Cria um novo objeto windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c252ece92661c2b57c8d8c7ea6c1b714a9bb9594
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516564"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="42b6f-103">Criar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="42b6f-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="42b6f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42b6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42b6f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42b6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42b6f-106">Cria um novo objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="42b6f-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42b6f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42b6f-107">Prerequisites</span></span>
<span data-ttu-id="42b6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42b6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42b6f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42b6f-110">Permission type</span></span>|<span data-ttu-id="42b6f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42b6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42b6f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42b6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42b6f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42b6f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42b6f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42b6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42b6f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42b6f-115">Not supported.</span></span>|
|<span data-ttu-id="42b6f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42b6f-116">Application</span></span>|<span data-ttu-id="42b6f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42b6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42b6f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42b6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="42b6f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42b6f-119">Request headers</span></span>
|<span data-ttu-id="42b6f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42b6f-120">Header</span></span>|<span data-ttu-id="42b6f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="42b6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42b6f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42b6f-122">Authorization</span></span>|<span data-ttu-id="42b6f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42b6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42b6f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42b6f-124">Accept</span></span>|<span data-ttu-id="42b6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42b6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42b6f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42b6f-126">Request body</span></span>
<span data-ttu-id="42b6f-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="42b6f-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="42b6f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="42b6f-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="42b6f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42b6f-129">Property</span></span>|<span data-ttu-id="42b6f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="42b6f-130">Type</span></span>|<span data-ttu-id="42b6f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="42b6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42b6f-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42b6f-132">roleScopeTagIds</span></span>|<span data-ttu-id="42b6f-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42b6f-133">String collection</span></span>|<span data-ttu-id="42b6f-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="42b6f-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42b6f-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-136">id</span><span class="sxs-lookup"><span data-stu-id="42b6f-136">id</span></span>|<span data-ttu-id="42b6f-137">String</span><span class="sxs-lookup"><span data-stu-id="42b6f-137">String</span></span>|<span data-ttu-id="42b6f-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42b6f-138">Key of the entity.</span></span> <span data-ttu-id="42b6f-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42b6f-140">createdDateTime</span></span>|<span data-ttu-id="42b6f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b6f-141">DateTimeOffset</span></span>|<span data-ttu-id="42b6f-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="42b6f-142">DateTime the object was created.</span></span> <span data-ttu-id="42b6f-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-144">description</span><span class="sxs-lookup"><span data-stu-id="42b6f-144">description</span></span>|<span data-ttu-id="42b6f-145">String</span><span class="sxs-lookup"><span data-stu-id="42b6f-145">String</span></span>|<span data-ttu-id="42b6f-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b6f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42b6f-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42b6f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="42b6f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b6f-149">DateTimeOffset</span></span>|<span data-ttu-id="42b6f-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="42b6f-150">DateTime the object was last modified.</span></span> <span data-ttu-id="42b6f-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="42b6f-152">displayName</span></span>|<span data-ttu-id="42b6f-153">String</span><span class="sxs-lookup"><span data-stu-id="42b6f-153">String</span></span>|<span data-ttu-id="42b6f-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b6f-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42b6f-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-156">version</span><span class="sxs-lookup"><span data-stu-id="42b6f-156">version</span></span>|<span data-ttu-id="42b6f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="42b6f-157">Int32</span></span>|<span data-ttu-id="42b6f-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42b6f-158">Version of the device configuration.</span></span> <span data-ttu-id="42b6f-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42b6f-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="42b6f-160">passwordRequired</span></span>|<span data-ttu-id="42b6f-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-161">Boolean</span></span>|<span data-ttu-id="42b6f-162">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="42b6f-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="42b6f-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="42b6f-163">passwordBlockSimple</span></span>|<span data-ttu-id="42b6f-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-164">Boolean</span></span>|<span data-ttu-id="42b6f-165">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="42b6f-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="42b6f-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42b6f-166">passwordMinimumLength</span></span>|<span data-ttu-id="42b6f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="42b6f-167">Int32</span></span>|<span data-ttu-id="42b6f-168">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="42b6f-168">Minimum password length.</span></span> <span data-ttu-id="42b6f-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="42b6f-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="42b6f-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="42b6f-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="42b6f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="42b6f-171">Int32</span></span>|<span data-ttu-id="42b6f-172">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="42b6f-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="42b6f-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="42b6f-173">passwordRequiredType</span></span>|[<span data-ttu-id="42b6f-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="42b6f-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="42b6f-175">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="42b6f-175">The required password type.</span></span> <span data-ttu-id="42b6f-176">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="42b6f-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="42b6f-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="42b6f-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="42b6f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="42b6f-178">Int32</span></span>|<span data-ttu-id="42b6f-179">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="42b6f-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="42b6f-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="42b6f-180">passwordExpirationDays</span></span>|<span data-ttu-id="42b6f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="42b6f-181">Int32</span></span>|<span data-ttu-id="42b6f-182">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="42b6f-182">Number of days before password expiration.</span></span> <span data-ttu-id="42b6f-183">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="42b6f-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="42b6f-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="42b6f-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="42b6f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="42b6f-185">Int32</span></span>|<span data-ttu-id="42b6f-186">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="42b6f-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="42b6f-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="42b6f-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="42b6f-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-188">Boolean</span></span>|<span data-ttu-id="42b6f-189">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="42b6f-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="42b6f-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="42b6f-190">osMinimumVersion</span></span>|<span data-ttu-id="42b6f-191">String</span><span class="sxs-lookup"><span data-stu-id="42b6f-191">String</span></span>|<span data-ttu-id="42b6f-192">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="42b6f-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="42b6f-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="42b6f-193">osMaximumVersion</span></span>|<span data-ttu-id="42b6f-194">String</span><span class="sxs-lookup"><span data-stu-id="42b6f-194">String</span></span>|<span data-ttu-id="42b6f-195">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="42b6f-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="42b6f-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="42b6f-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="42b6f-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-197">Boolean</span></span>|<span data-ttu-id="42b6f-198">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="42b6f-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="42b6f-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="42b6f-199">bitLockerEnabled</span></span>|<span data-ttu-id="42b6f-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-200">Boolean</span></span>|<span data-ttu-id="42b6f-201">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="42b6f-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="42b6f-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="42b6f-202">secureBootEnabled</span></span>|<span data-ttu-id="42b6f-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-203">Boolean</span></span>|<span data-ttu-id="42b6f-204">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="42b6f-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="42b6f-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="42b6f-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="42b6f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b6f-206">Boolean</span></span>|<span data-ttu-id="42b6f-207">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="42b6f-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="42b6f-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="42b6f-208">storageRequireEncryption</span></span>|<span data-ttu-id="42b6f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="42b6f-209">Boolean</span></span>|<span data-ttu-id="42b6f-210">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="42b6f-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="42b6f-211">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="42b6f-211">activeFirewallRequired</span></span>|<span data-ttu-id="42b6f-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="42b6f-212">Boolean</span></span>|<span data-ttu-id="42b6f-213">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="42b6f-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="42b6f-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="42b6f-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="42b6f-215">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="42b6f-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="42b6f-216">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="42b6f-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="42b6f-217">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="42b6f-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="42b6f-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="42b6f-218">Response</span></span>
<span data-ttu-id="42b6f-219">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42b6f-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b6f-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42b6f-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="42b6f-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42b6f-221">Request</span></span>
<span data-ttu-id="42b6f-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42b6f-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42b6f-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="42b6f-223">Response</span></span>
<span data-ttu-id="42b6f-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42b6f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





