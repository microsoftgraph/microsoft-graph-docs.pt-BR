---
title: Atualizar windows10CompliancePolicy
description: Atualiza as propriedades de um objeto windows10CompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 2e1fe8fb9894e15ed1b122760ddb9d6536ca60f6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350173"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="4fc8e-103">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4fc8e-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="4fc8e-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fc8e-105">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4fc8e-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4fc8e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4fc8e-106">Prerequisites</span></span>
<span data-ttu-id="4fc8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fc8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc8e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fc8e-109">Permission type</span></span>|<span data-ttu-id="4fc8e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc8e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc8e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc8e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fc8e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc8e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-114">Not supported.</span></span>|
|<span data-ttu-id="4fc8e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fc8e-115">Application</span></span>|<span data-ttu-id="4fc8e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc8e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fc8e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4fc8e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fc8e-118">Request headers</span></span>
|<span data-ttu-id="4fc8e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fc8e-119">Header</span></span>|<span data-ttu-id="4fc8e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4fc8e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc8e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fc8e-121">Authorization</span></span>|<span data-ttu-id="4fc8e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc8e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4fc8e-123">Accept</span></span>|<span data-ttu-id="4fc8e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc8e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc8e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fc8e-125">Request body</span></span>
<span data-ttu-id="4fc8e-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4fc8e-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="4fc8e-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4fc8e-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="4fc8e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fc8e-128">Property</span></span>|<span data-ttu-id="4fc8e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fc8e-129">Type</span></span>|<span data-ttu-id="4fc8e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fc8e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc8e-131">id</span><span class="sxs-lookup"><span data-stu-id="4fc8e-131">id</span></span>|<span data-ttu-id="4fc8e-132">String</span><span class="sxs-lookup"><span data-stu-id="4fc8e-132">String</span></span>|<span data-ttu-id="4fc8e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-133">Key of the entity.</span></span> <span data-ttu-id="4fc8e-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4fc8e-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc8e-135">createdDateTime</span></span>|<span data-ttu-id="4fc8e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc8e-136">DateTimeOffset</span></span>|<span data-ttu-id="4fc8e-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-137">DateTime the object was created.</span></span> <span data-ttu-id="4fc8e-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4fc8e-139">description</span><span class="sxs-lookup"><span data-stu-id="4fc8e-139">description</span></span>|<span data-ttu-id="4fc8e-140">String</span><span class="sxs-lookup"><span data-stu-id="4fc8e-140">String</span></span>|<span data-ttu-id="4fc8e-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4fc8e-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4fc8e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc8e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4fc8e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc8e-144">DateTimeOffset</span></span>|<span data-ttu-id="4fc8e-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-145">DateTime the object was last modified.</span></span> <span data-ttu-id="4fc8e-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4fc8e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4fc8e-147">displayName</span></span>|<span data-ttu-id="4fc8e-148">String</span><span class="sxs-lookup"><span data-stu-id="4fc8e-148">String</span></span>|<span data-ttu-id="4fc8e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4fc8e-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4fc8e-151">version</span><span class="sxs-lookup"><span data-stu-id="4fc8e-151">version</span></span>|<span data-ttu-id="4fc8e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc8e-152">Int32</span></span>|<span data-ttu-id="4fc8e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-153">Version of the device configuration.</span></span> <span data-ttu-id="4fc8e-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4fc8e-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4fc8e-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4fc8e-155">passwordRequired</span></span>|<span data-ttu-id="4fc8e-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fc8e-156">Boolean</span></span>|<span data-ttu-id="4fc8e-157">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="4fc8e-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4fc8e-158">passwordBlockSimple</span></span>|<span data-ttu-id="4fc8e-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fc8e-159">Boolean</span></span>|<span data-ttu-id="4fc8e-160">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="4fc8e-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="4fc8e-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="4fc8e-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fc8e-162">Boolean</span></span>|<span data-ttu-id="4fc8e-163">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="4fc8e-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4fc8e-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4fc8e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc8e-165">Int32</span></span>|<span data-ttu-id="4fc8e-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4fc8e-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4fc8e-167">passwordExpirationDays</span></span>|<span data-ttu-id="4fc8e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc8e-168">Int32</span></span>|<span data-ttu-id="4fc8e-169">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-169">The password expiration in days.</span></span>|
|<span data-ttu-id="4fc8e-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4fc8e-170">passwordMinimumLength</span></span>|<span data-ttu-id="4fc8e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc8e-171">Int32</span></span>|<span data-ttu-id="4fc8e-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-172">The minimum password length.</span></span>|
|<span data-ttu-id="4fc8e-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4fc8e-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4fc8e-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc8e-174">Int32</span></span>|<span data-ttu-id="4fc8e-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4fc8e-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4fc8e-176">passwordRequiredType</span></span>|[<span data-ttu-id="4fc8e-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4fc8e-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4fc8e-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-178">The required password type.</span></span> <span data-ttu-id="4fc8e-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4fc8e-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4fc8e-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4fc8e-181">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc8e-181">Int32</span></span>|<span data-ttu-id="4fc8e-182">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="4fc8e-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="4fc8e-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="4fc8e-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fc8e-184">Boolean</span></span>|<span data-ttu-id="4fc8e-185">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4fc8e-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4fc8e-186">osMinimumVersion</span></span>|<span data-ttu-id="4fc8e-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fc8e-187">String</span></span>|<span data-ttu-id="4fc8e-188">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="4fc8e-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4fc8e-189">osMaximumVersion</span></span>|<span data-ttu-id="4fc8e-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fc8e-190">String</span></span>|<span data-ttu-id="4fc8e-191">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="4fc8e-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4fc8e-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="4fc8e-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fc8e-193">String</span></span>|<span data-ttu-id="4fc8e-194">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="4fc8e-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4fc8e-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="4fc8e-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fc8e-196">String</span></span>|<span data-ttu-id="4fc8e-197">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="4fc8e-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="4fc8e-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="4fc8e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc8e-199">Boolean</span></span>|<span data-ttu-id="4fc8e-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="4fc8e-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="4fc8e-201">bitLockerEnabled</span></span>|<span data-ttu-id="4fc8e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc8e-202">Boolean</span></span>|<span data-ttu-id="4fc8e-203">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="4fc8e-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="4fc8e-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="4fc8e-204">secureBootEnabled</span></span>|<span data-ttu-id="4fc8e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc8e-205">Boolean</span></span>|<span data-ttu-id="4fc8e-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="4fc8e-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="4fc8e-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="4fc8e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc8e-208">Boolean</span></span>|<span data-ttu-id="4fc8e-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4fc8e-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4fc8e-210">storageRequireEncryption</span></span>|<span data-ttu-id="4fc8e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc8e-211">Boolean</span></span>|<span data-ttu-id="4fc8e-212">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="4fc8e-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fc8e-213">Response</span></span>
<span data-ttu-id="4fc8e-214">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc8e-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fc8e-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="4fc8e-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fc8e-216">Request</span></span>
<span data-ttu-id="4fc8e-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="4fc8e-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fc8e-218">Response</span></span>
<span data-ttu-id="4fc8e-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```



