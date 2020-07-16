---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e69151a5f0b7a0bc8c0558fc9f178714e7520d1c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792636"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="96e6e-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="96e6e-103">Create windows10CompliancePolicy</span></span>

<span data-ttu-id="96e6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96e6e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96e6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96e6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96e6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96e6e-107">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="96e6e-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96e6e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96e6e-108">Prerequisites</span></span>
<span data-ttu-id="96e6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96e6e-111">Permission type</span></span>|<span data-ttu-id="96e6e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96e6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96e6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96e6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96e6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96e6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96e6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96e6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96e6e-116">Not supported.</span></span>|
|<span data-ttu-id="96e6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96e6e-117">Application</span></span>|<span data-ttu-id="96e6e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e6e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96e6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96e6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="96e6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96e6e-120">Request headers</span></span>
|<span data-ttu-id="96e6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96e6e-121">Header</span></span>|<span data-ttu-id="96e6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96e6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96e6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96e6e-123">Authorization</span></span>|<span data-ttu-id="96e6e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96e6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96e6e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96e6e-125">Accept</span></span>|<span data-ttu-id="96e6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96e6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96e6e-127">Request body</span></span>
<span data-ttu-id="96e6e-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="96e6e-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="96e6e-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="96e6e-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="96e6e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96e6e-130">Property</span></span>|<span data-ttu-id="96e6e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="96e6e-131">Type</span></span>|<span data-ttu-id="96e6e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="96e6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96e6e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96e6e-133">roleScopeTagIds</span></span>|<span data-ttu-id="96e6e-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96e6e-134">String collection</span></span>|<span data-ttu-id="96e6e-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="96e6e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96e6e-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-137">id</span><span class="sxs-lookup"><span data-stu-id="96e6e-137">id</span></span>|<span data-ttu-id="96e6e-138">String</span><span class="sxs-lookup"><span data-stu-id="96e6e-138">String</span></span>|<span data-ttu-id="96e6e-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96e6e-139">Key of the entity.</span></span> <span data-ttu-id="96e6e-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96e6e-141">createdDateTime</span></span>|<span data-ttu-id="96e6e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e6e-142">DateTimeOffset</span></span>|<span data-ttu-id="96e6e-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="96e6e-143">DateTime the object was created.</span></span> <span data-ttu-id="96e6e-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-145">description</span><span class="sxs-lookup"><span data-stu-id="96e6e-145">description</span></span>|<span data-ttu-id="96e6e-146">String</span><span class="sxs-lookup"><span data-stu-id="96e6e-146">String</span></span>|<span data-ttu-id="96e6e-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96e6e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96e6e-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96e6e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="96e6e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e6e-150">DateTimeOffset</span></span>|<span data-ttu-id="96e6e-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="96e6e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="96e6e-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="96e6e-153">displayName</span></span>|<span data-ttu-id="96e6e-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96e6e-154">String</span></span>|<span data-ttu-id="96e6e-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96e6e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96e6e-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-157">version</span><span class="sxs-lookup"><span data-stu-id="96e6e-157">version</span></span>|<span data-ttu-id="96e6e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="96e6e-158">Int32</span></span>|<span data-ttu-id="96e6e-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96e6e-159">Version of the device configuration.</span></span> <span data-ttu-id="96e6e-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="96e6e-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="96e6e-161">passwordRequired</span></span>|<span data-ttu-id="96e6e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-162">Boolean</span></span>|<span data-ttu-id="96e6e-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="96e6e-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="96e6e-164">passwordBlockSimple</span></span>|<span data-ttu-id="96e6e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-165">Boolean</span></span>|<span data-ttu-id="96e6e-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="96e6e-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="96e6e-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="96e6e-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="96e6e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-168">Boolean</span></span>|<span data-ttu-id="96e6e-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="96e6e-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="96e6e-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="96e6e-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="96e6e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="96e6e-171">Int32</span></span>|<span data-ttu-id="96e6e-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="96e6e-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="96e6e-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="96e6e-173">passwordExpirationDays</span></span>|<span data-ttu-id="96e6e-174">Int32</span><span class="sxs-lookup"><span data-stu-id="96e6e-174">Int32</span></span>|<span data-ttu-id="96e6e-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="96e6e-175">The password expiration in days.</span></span>|
|<span data-ttu-id="96e6e-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="96e6e-176">passwordMinimumLength</span></span>|<span data-ttu-id="96e6e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="96e6e-177">Int32</span></span>|<span data-ttu-id="96e6e-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="96e6e-178">The minimum password length.</span></span>|
|<span data-ttu-id="96e6e-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="96e6e-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="96e6e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="96e6e-180">Int32</span></span>|<span data-ttu-id="96e6e-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="96e6e-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="96e6e-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="96e6e-182">passwordRequiredType</span></span>|[<span data-ttu-id="96e6e-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="96e6e-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="96e6e-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="96e6e-184">The required password type.</span></span> <span data-ttu-id="96e6e-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="96e6e-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="96e6e-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="96e6e-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="96e6e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="96e6e-187">Int32</span></span>|<span data-ttu-id="96e6e-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="96e6e-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="96e6e-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="96e6e-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="96e6e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-190">Boolean</span></span>|<span data-ttu-id="96e6e-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="96e6e-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="96e6e-192">osMinimumVersion</span></span>|<span data-ttu-id="96e6e-193">String</span><span class="sxs-lookup"><span data-stu-id="96e6e-193">String</span></span>|<span data-ttu-id="96e6e-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="96e6e-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="96e6e-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="96e6e-195">osMaximumVersion</span></span>|<span data-ttu-id="96e6e-196">String</span><span class="sxs-lookup"><span data-stu-id="96e6e-196">String</span></span>|<span data-ttu-id="96e6e-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="96e6e-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="96e6e-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="96e6e-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="96e6e-199">String</span><span class="sxs-lookup"><span data-stu-id="96e6e-199">String</span></span>|<span data-ttu-id="96e6e-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="96e6e-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="96e6e-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="96e6e-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="96e6e-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96e6e-202">String</span></span>|<span data-ttu-id="96e6e-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="96e6e-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="96e6e-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="96e6e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-205">Boolean</span></span>|<span data-ttu-id="96e6e-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="96e6e-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="96e6e-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-207">bitLockerEnabled</span></span>|<span data-ttu-id="96e6e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-208">Boolean</span></span>|<span data-ttu-id="96e6e-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="96e6e-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="96e6e-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-210">secureBootEnabled</span></span>|<span data-ttu-id="96e6e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-211">Boolean</span></span>|<span data-ttu-id="96e6e-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="96e6e-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="96e6e-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="96e6e-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-214">Boolean</span></span>|<span data-ttu-id="96e6e-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="96e6e-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="96e6e-216">storageRequireEncryption</span></span>|<span data-ttu-id="96e6e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-217">Boolean</span></span>|<span data-ttu-id="96e6e-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="96e6e-219">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="96e6e-219">activeFirewallRequired</span></span>|<span data-ttu-id="96e6e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-220">Boolean</span></span>|<span data-ttu-id="96e6e-221">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="96e6e-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-222">defenderEnabled</span></span>|<span data-ttu-id="96e6e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-223">Boolean</span></span>|<span data-ttu-id="96e6e-224">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="96e6e-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="96e6e-225">defenderVersion</span></span>|<span data-ttu-id="96e6e-226">String</span><span class="sxs-lookup"><span data-stu-id="96e6e-226">String</span></span>|<span data-ttu-id="96e6e-227">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="96e6e-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="96e6e-228">signatureOutOfDate</span></span>|<span data-ttu-id="96e6e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-229">Boolean</span></span>|<span data-ttu-id="96e6e-230">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="96e6e-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-231">rtpEnabled</span></span>|<span data-ttu-id="96e6e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-232">Boolean</span></span>|<span data-ttu-id="96e6e-233">Requer a proteção em tempo real do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="96e6e-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="96e6e-234">antivirusRequired</span></span>|<span data-ttu-id="96e6e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-235">Boolean</span></span>|<span data-ttu-id="96e6e-236">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="96e6e-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="96e6e-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="96e6e-237">antiSpywareRequired</span></span>|<span data-ttu-id="96e6e-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-238">Boolean</span></span>|<span data-ttu-id="96e6e-239">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="96e6e-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="96e6e-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="96e6e-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="96e6e-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="96e6e-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="96e6e-242">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="96e6e-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="96e6e-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="96e6e-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="96e6e-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="96e6e-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="96e6e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-245">Boolean</span></span>|<span data-ttu-id="96e6e-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="96e6e-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="96e6e-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="96e6e-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="96e6e-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="96e6e-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="96e6e-249">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="96e6e-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="96e6e-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="96e6e-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="96e6e-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="96e6e-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="96e6e-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-252">Boolean</span></span>|<span data-ttu-id="96e6e-253">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="96e6e-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="96e6e-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="96e6e-254">tpmRequired</span></span>|<span data-ttu-id="96e6e-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="96e6e-255">Boolean</span></span>|<span data-ttu-id="96e6e-256">Requer o módulo de plataforma confiável (TPM) para estar presente.</span><span class="sxs-lookup"><span data-stu-id="96e6e-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="96e6e-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="96e6e-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="96e6e-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="96e6e-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="96e6e-259">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96e6e-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="96e6e-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e6e-260">Response</span></span>
<span data-ttu-id="96e6e-261">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96e6e-261">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e6e-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96e6e-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="96e6e-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96e6e-263">Request</span></span>
<span data-ttu-id="96e6e-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96e6e-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1911

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="96e6e-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e6e-265">Response</span></span>
<span data-ttu-id="96e6e-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96e6e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2083

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```



