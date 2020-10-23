---
title: Atualizar windows10CompliancePolicy
description: Atualiza as propriedades de um objeto windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3143b55824a8b71807a96d880aa565cdd9cbaebc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692027"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="6e6e8-103">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6e6e8-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="6e6e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e6e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e6e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e6e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e6e8-107">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e6e8-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e6e8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e6e8-108">Prerequisites</span></span>
<span data-ttu-id="6e6e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e6e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e6e8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e6e8-111">Permission type</span></span>|<span data-ttu-id="6e6e8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e6e8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e6e8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6e8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e6e8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e6e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-116">Not supported.</span></span>|
|<span data-ttu-id="6e6e8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e6e8-117">Application</span></span>|<span data-ttu-id="6e6e8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e6e8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e6e8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e6e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6e6e8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e6e8-120">Request headers</span></span>
|<span data-ttu-id="6e6e8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e6e8-121">Header</span></span>|<span data-ttu-id="6e6e8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e6e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e6e8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e6e8-123">Authorization</span></span>|<span data-ttu-id="6e6e8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e6e8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e6e8-125">Accept</span></span>|<span data-ttu-id="6e6e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e6e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e6e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e6e8-127">Request body</span></span>
<span data-ttu-id="6e6e8-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e6e8-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="6e6e8-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e6e8-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="6e6e8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e6e8-130">Property</span></span>|<span data-ttu-id="6e6e8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e6e8-131">Type</span></span>|<span data-ttu-id="6e6e8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e6e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e6e8-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e6e8-133">roleScopeTagIds</span></span>|<span data-ttu-id="6e6e8-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e6e8-134">String collection</span></span>|<span data-ttu-id="6e6e8-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e6e8-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-137">id</span><span class="sxs-lookup"><span data-stu-id="6e6e8-137">id</span></span>|<span data-ttu-id="6e6e8-138">String</span><span class="sxs-lookup"><span data-stu-id="6e6e8-138">String</span></span>|<span data-ttu-id="6e6e8-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-139">Key of the entity.</span></span> <span data-ttu-id="6e6e8-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e6e8-141">createdDateTime</span></span>|<span data-ttu-id="6e6e8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e6e8-142">DateTimeOffset</span></span>|<span data-ttu-id="6e6e8-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-143">DateTime the object was created.</span></span> <span data-ttu-id="6e6e8-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-145">description</span><span class="sxs-lookup"><span data-stu-id="6e6e8-145">description</span></span>|<span data-ttu-id="6e6e8-146">String</span><span class="sxs-lookup"><span data-stu-id="6e6e8-146">String</span></span>|<span data-ttu-id="6e6e8-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e6e8-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e6e8-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6e6e8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e6e8-150">DateTimeOffset</span></span>|<span data-ttu-id="6e6e8-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-151">DateTime the object was last modified.</span></span> <span data-ttu-id="6e6e8-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6e6e8-153">displayName</span></span>|<span data-ttu-id="6e6e8-154">String</span><span class="sxs-lookup"><span data-stu-id="6e6e8-154">String</span></span>|<span data-ttu-id="6e6e8-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e6e8-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-157">version</span><span class="sxs-lookup"><span data-stu-id="6e6e8-157">version</span></span>|<span data-ttu-id="6e6e8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6e6e8-158">Int32</span></span>|<span data-ttu-id="6e6e8-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-159">Version of the device configuration.</span></span> <span data-ttu-id="6e6e8-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e6e8-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6e6e8-161">passwordRequired</span></span>|<span data-ttu-id="6e6e8-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e6e8-162">Boolean</span></span>|<span data-ttu-id="6e6e8-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="6e6e8-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6e6e8-164">passwordBlockSimple</span></span>|<span data-ttu-id="6e6e8-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e6e8-165">Boolean</span></span>|<span data-ttu-id="6e6e8-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="6e6e8-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="6e6e8-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="6e6e8-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e6e8-168">Boolean</span></span>|<span data-ttu-id="6e6e8-169">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="6e6e8-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6e6e8-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6e6e8-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6e6e8-171">Int32</span></span>|<span data-ttu-id="6e6e8-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6e6e8-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6e6e8-173">passwordExpirationDays</span></span>|<span data-ttu-id="6e6e8-174">Int32</span><span class="sxs-lookup"><span data-stu-id="6e6e8-174">Int32</span></span>|<span data-ttu-id="6e6e8-175">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-175">The password expiration in days.</span></span>|
|<span data-ttu-id="6e6e8-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6e6e8-176">passwordMinimumLength</span></span>|<span data-ttu-id="6e6e8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6e6e8-177">Int32</span></span>|<span data-ttu-id="6e6e8-178">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-178">The minimum password length.</span></span>|
|<span data-ttu-id="6e6e8-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6e6e8-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6e6e8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6e6e8-180">Int32</span></span>|<span data-ttu-id="6e6e8-181">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6e6e8-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6e6e8-182">passwordRequiredType</span></span>|[<span data-ttu-id="6e6e8-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6e6e8-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6e6e8-184">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-184">The required password type.</span></span> <span data-ttu-id="6e6e8-185">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6e6e8-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6e6e8-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6e6e8-187">Int32</span><span class="sxs-lookup"><span data-stu-id="6e6e8-187">Int32</span></span>|<span data-ttu-id="6e6e8-188">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="6e6e8-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="6e6e8-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="6e6e8-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e6e8-190">Boolean</span></span>|<span data-ttu-id="6e6e8-191">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="6e6e8-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e6e8-192">osMinimumVersion</span></span>|<span data-ttu-id="6e6e8-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e6e8-193">String</span></span>|<span data-ttu-id="6e6e8-194">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="6e6e8-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e6e8-195">osMaximumVersion</span></span>|<span data-ttu-id="6e6e8-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e6e8-196">String</span></span>|<span data-ttu-id="6e6e8-197">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="6e6e8-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e6e8-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="6e6e8-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e6e8-199">String</span></span>|<span data-ttu-id="6e6e8-200">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="6e6e8-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e6e8-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="6e6e8-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e6e8-202">String</span></span>|<span data-ttu-id="6e6e8-203">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="6e6e8-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="6e6e8-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-205">Boolean</span></span>|<span data-ttu-id="6e6e8-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="6e6e8-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-207">bitLockerEnabled</span></span>|<span data-ttu-id="6e6e8-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-208">Boolean</span></span>|<span data-ttu-id="6e6e8-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="6e6e8-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="6e6e8-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-210">secureBootEnabled</span></span>|<span data-ttu-id="6e6e8-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-211">Boolean</span></span>|<span data-ttu-id="6e6e8-212">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="6e6e8-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="6e6e8-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-214">Boolean</span></span>|<span data-ttu-id="6e6e8-215">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="6e6e8-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6e6e8-216">storageRequireEncryption</span></span>|<span data-ttu-id="6e6e8-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-217">Boolean</span></span>|<span data-ttu-id="6e6e8-218">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="6e6e8-219">Propriedades activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="6e6e8-219">activeFirewallRequired</span></span>|<span data-ttu-id="6e6e8-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-220">Boolean</span></span>|<span data-ttu-id="6e6e8-221">Exigir firewall ativo em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="6e6e8-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-222">defenderEnabled</span></span>|<span data-ttu-id="6e6e8-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-223">Boolean</span></span>|<span data-ttu-id="6e6e8-224">Requer o Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="6e6e8-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="6e6e8-225">defenderVersion</span></span>|<span data-ttu-id="6e6e8-226">String</span><span class="sxs-lookup"><span data-stu-id="6e6e8-226">String</span></span>|<span data-ttu-id="6e6e8-227">Requer a versão mínima do Windows Defender Antimalware em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="6e6e8-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="6e6e8-228">signatureOutOfDate</span></span>|<span data-ttu-id="6e6e8-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-229">Boolean</span></span>|<span data-ttu-id="6e6e8-230">Requer que a assinatura antimalware do Windows Defender esteja atualizada em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="6e6e8-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-231">rtpEnabled</span></span>|<span data-ttu-id="6e6e8-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-232">Boolean</span></span>|<span data-ttu-id="6e6e8-233">Requer o Windows Defender Antimalware Real-Time proteção em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="6e6e8-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="6e6e8-234">antivirusRequired</span></span>|<span data-ttu-id="6e6e8-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-235">Boolean</span></span>|<span data-ttu-id="6e6e8-236">Exigir que qualquer solução antivírus registrada com o Windows Decurity Center seja ativada e monitorando (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="6e6e8-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="6e6e8-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="6e6e8-237">antiSpywareRequired</span></span>|<span data-ttu-id="6e6e8-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-238">Boolean</span></span>|<span data-ttu-id="6e6e8-239">Exija que qualquer solução AntiSpyware registrada com o Windows Decurity Center seja ativada e monitoramento (por exemplo, Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="6e6e8-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="6e6e8-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="6e6e8-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="6e6e8-241">coleção [operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="6e6e8-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="6e6e8-242">Os intervalos válidos da compilação do sistema operacional em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="6e6e8-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6e6e8-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e6e8-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6e6e8-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-245">Boolean</span></span>|<span data-ttu-id="6e6e8-246">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6e6e8-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6e6e8-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6e6e8-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6e6e8-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6e6e8-249">Requer nível mínimo de risco de proteção contra ameaças ao dispositivo para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6e6e8-250">Os possíveis valores são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6e6e8-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="6e6e8-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="6e6e8-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-252">Boolean</span></span>|<span data-ttu-id="6e6e8-253">Exigir que o estado de conformidade do SCCM seja considerado para o estado de conformidade do Intune.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="6e6e8-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="6e6e8-254">tpmRequired</span></span>|<span data-ttu-id="6e6e8-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e6e8-255">Boolean</span></span>|<span data-ttu-id="6e6e8-256">Requer o módulo de plataforma confiável (TPM) para estar presente.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="6e6e8-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="6e6e8-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="6e6e8-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="6e6e8-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="6e6e8-259">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6e6e8-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6e6e8-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e6e8-260">Response</span></span>
<span data-ttu-id="6e6e8-261">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-261">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e6e8-262">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e6e8-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e6e8-263">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e6e8-263">Request</span></span>
<span data-ttu-id="6e6e8-264">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="6e6e8-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e6e8-265">Response</span></span>
<span data-ttu-id="6e6e8-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e6e8-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





