---
title: Atualizar windows10MobileCompliancePolicy
description: Atualiza as propriedades de um objeto windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8480bd4be5e7af4806381941aaabc94272a9ae20
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430617"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="df0d6-103">Atualizar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="df0d6-103">Update windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="df0d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df0d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df0d6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df0d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df0d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df0d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df0d6-107">Atualiza as propriedades de um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="df0d6-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df0d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df0d6-108">Prerequisites</span></span>
<span data-ttu-id="df0d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df0d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df0d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df0d6-111">Permission type</span></span>|<span data-ttu-id="df0d6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df0d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df0d6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df0d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df0d6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0d6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df0d6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df0d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df0d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df0d6-116">Not supported.</span></span>|
|<span data-ttu-id="df0d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df0d6-117">Application</span></span>|<span data-ttu-id="df0d6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0d6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df0d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df0d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="df0d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df0d6-120">Request headers</span></span>
|<span data-ttu-id="df0d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df0d6-121">Header</span></span>|<span data-ttu-id="df0d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df0d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df0d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df0d6-123">Authorization</span></span>|<span data-ttu-id="df0d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df0d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df0d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df0d6-125">Accept</span></span>|<span data-ttu-id="df0d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df0d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df0d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df0d6-127">Request body</span></span>
<span data-ttu-id="df0d6-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="df0d6-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="df0d6-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="df0d6-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="df0d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df0d6-130">Property</span></span>|<span data-ttu-id="df0d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df0d6-131">Type</span></span>|<span data-ttu-id="df0d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df0d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df0d6-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df0d6-133">roleScopeTagIds</span></span>|<span data-ttu-id="df0d6-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="df0d6-134">String collection</span></span>|<span data-ttu-id="df0d6-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="df0d6-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df0d6-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-137">id</span><span class="sxs-lookup"><span data-stu-id="df0d6-137">id</span></span>|<span data-ttu-id="df0d6-138">String</span><span class="sxs-lookup"><span data-stu-id="df0d6-138">String</span></span>|<span data-ttu-id="df0d6-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df0d6-139">Key of the entity.</span></span> <span data-ttu-id="df0d6-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df0d6-141">createdDateTime</span></span>|<span data-ttu-id="df0d6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df0d6-142">DateTimeOffset</span></span>|<span data-ttu-id="df0d6-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="df0d6-143">DateTime the object was created.</span></span> <span data-ttu-id="df0d6-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-145">description</span><span class="sxs-lookup"><span data-stu-id="df0d6-145">description</span></span>|<span data-ttu-id="df0d6-146">String</span><span class="sxs-lookup"><span data-stu-id="df0d6-146">String</span></span>|<span data-ttu-id="df0d6-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df0d6-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df0d6-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df0d6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="df0d6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df0d6-150">DateTimeOffset</span></span>|<span data-ttu-id="df0d6-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="df0d6-151">DateTime the object was last modified.</span></span> <span data-ttu-id="df0d6-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-153">displayName</span><span class="sxs-lookup"><span data-stu-id="df0d6-153">displayName</span></span>|<span data-ttu-id="df0d6-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df0d6-154">String</span></span>|<span data-ttu-id="df0d6-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df0d6-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df0d6-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-157">version</span><span class="sxs-lookup"><span data-stu-id="df0d6-157">version</span></span>|<span data-ttu-id="df0d6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="df0d6-158">Int32</span></span>|<span data-ttu-id="df0d6-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df0d6-159">Version of the device configuration.</span></span> <span data-ttu-id="df0d6-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="df0d6-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="df0d6-161">passwordRequired</span></span>|<span data-ttu-id="df0d6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-162">Boolean</span></span>|<span data-ttu-id="df0d6-163">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="df0d6-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="df0d6-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="df0d6-164">passwordBlockSimple</span></span>|<span data-ttu-id="df0d6-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="df0d6-165">Boolean</span></span>|<span data-ttu-id="df0d6-166">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="df0d6-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="df0d6-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="df0d6-167">passwordMinimumLength</span></span>|<span data-ttu-id="df0d6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="df0d6-168">Int32</span></span>|<span data-ttu-id="df0d6-169">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="df0d6-169">Minimum password length.</span></span> <span data-ttu-id="df0d6-170">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="df0d6-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="df0d6-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="df0d6-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="df0d6-172">Int32</span><span class="sxs-lookup"><span data-stu-id="df0d6-172">Int32</span></span>|<span data-ttu-id="df0d6-173">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="df0d6-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="df0d6-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="df0d6-174">passwordRequiredType</span></span>|[<span data-ttu-id="df0d6-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="df0d6-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="df0d6-176">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="df0d6-176">The required password type.</span></span> <span data-ttu-id="df0d6-177">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="df0d6-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="df0d6-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="df0d6-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="df0d6-179">Int32</span><span class="sxs-lookup"><span data-stu-id="df0d6-179">Int32</span></span>|<span data-ttu-id="df0d6-180">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="df0d6-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="df0d6-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="df0d6-181">passwordExpirationDays</span></span>|<span data-ttu-id="df0d6-182">Int32</span><span class="sxs-lookup"><span data-stu-id="df0d6-182">Int32</span></span>|<span data-ttu-id="df0d6-183">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="df0d6-183">Number of days before password expiration.</span></span> <span data-ttu-id="df0d6-184">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="df0d6-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="df0d6-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="df0d6-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="df0d6-186">Int32</span><span class="sxs-lookup"><span data-stu-id="df0d6-186">Int32</span></span>|<span data-ttu-id="df0d6-187">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="df0d6-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="df0d6-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="df0d6-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="df0d6-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="df0d6-189">Boolean</span></span>|<span data-ttu-id="df0d6-190">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="df0d6-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="df0d6-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="df0d6-191">osMinimumVersion</span></span>|<span data-ttu-id="df0d6-192">String</span><span class="sxs-lookup"><span data-stu-id="df0d6-192">String</span></span>|<span data-ttu-id="df0d6-193">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="df0d6-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="df0d6-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="df0d6-194">osMaximumVersion</span></span>|<span data-ttu-id="df0d6-195">String</span><span class="sxs-lookup"><span data-stu-id="df0d6-195">String</span></span>|<span data-ttu-id="df0d6-196">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="df0d6-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="df0d6-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="df0d6-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="df0d6-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-198">Boolean</span></span>|<span data-ttu-id="df0d6-199">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="df0d6-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="df0d6-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="df0d6-200">bitLockerEnabled</span></span>|<span data-ttu-id="df0d6-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-201">Boolean</span></span>|<span data-ttu-id="df0d6-202">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="df0d6-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="df0d6-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="df0d6-203">secureBootEnabled</span></span>|<span data-ttu-id="df0d6-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-204">Boolean</span></span>|<span data-ttu-id="df0d6-205">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="df0d6-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="df0d6-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="df0d6-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="df0d6-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-207">Boolean</span></span>|<span data-ttu-id="df0d6-208">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="df0d6-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="df0d6-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="df0d6-209">storageRequireEncryption</span></span>|<span data-ttu-id="df0d6-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-210">Boolean</span></span>|<span data-ttu-id="df0d6-211">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="df0d6-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="df0d6-212">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="df0d6-212">activeFirewallRequired</span></span>|<span data-ttu-id="df0d6-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0d6-213">Boolean</span></span>|<span data-ttu-id="df0d6-214">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="df0d6-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="df0d6-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="df0d6-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="df0d6-216">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="df0d6-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="df0d6-217">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="df0d6-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="df0d6-218">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="df0d6-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="df0d6-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="df0d6-219">Response</span></span>
<span data-ttu-id="df0d6-220">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df0d6-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df0d6-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df0d6-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="df0d6-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df0d6-222">Request</span></span>
<span data-ttu-id="df0d6-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df0d6-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="df0d6-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="df0d6-224">Response</span></span>
<span data-ttu-id="df0d6-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df0d6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



