---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1462f4e65e3a18da4b4f72a97ac4651cd9cca3fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864824"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="d121c-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d121c-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="d121c-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d121c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d121c-105">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d121c-105">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d121c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d121c-106">Prerequisites</span></span>
<span data-ttu-id="d121c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d121c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d121c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d121c-109">Permission type</span></span>|<span data-ttu-id="d121c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d121c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d121c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d121c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d121c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d121c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d121c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d121c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d121c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d121c-114">Not supported.</span></span>|
|<span data-ttu-id="d121c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d121c-115">Application</span></span>|<span data-ttu-id="d121c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d121c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d121c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d121c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d121c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d121c-118">Request headers</span></span>
|<span data-ttu-id="d121c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d121c-119">Header</span></span>|<span data-ttu-id="d121c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d121c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d121c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d121c-121">Authorization</span></span>|<span data-ttu-id="d121c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d121c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d121c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d121c-123">Accept</span></span>|<span data-ttu-id="d121c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d121c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d121c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d121c-125">Request body</span></span>
<span data-ttu-id="d121c-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d121c-126">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="d121c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="d121c-127">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="d121c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d121c-128">Property</span></span>|<span data-ttu-id="d121c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d121c-129">Type</span></span>|<span data-ttu-id="d121c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d121c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d121c-131">id</span><span class="sxs-lookup"><span data-stu-id="d121c-131">id</span></span>|<span data-ttu-id="d121c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-132">String</span></span>|<span data-ttu-id="d121c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d121c-133">Key of the entity.</span></span> <span data-ttu-id="d121c-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d121c-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d121c-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d121c-135">createdDateTime</span></span>|<span data-ttu-id="d121c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d121c-136">DateTimeOffset</span></span>|<span data-ttu-id="d121c-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d121c-137">DateTime the object was created.</span></span> <span data-ttu-id="d121c-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d121c-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d121c-139">description</span><span class="sxs-lookup"><span data-stu-id="d121c-139">description</span></span>|<span data-ttu-id="d121c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-140">String</span></span>|<span data-ttu-id="d121c-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d121c-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d121c-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d121c-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d121c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d121c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="d121c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d121c-144">DateTimeOffset</span></span>|<span data-ttu-id="d121c-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d121c-145">DateTime the object was last modified.</span></span> <span data-ttu-id="d121c-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d121c-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d121c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d121c-147">displayName</span></span>|<span data-ttu-id="d121c-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-148">String</span></span>|<span data-ttu-id="d121c-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d121c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d121c-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d121c-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d121c-151">version</span><span class="sxs-lookup"><span data-stu-id="d121c-151">version</span></span>|<span data-ttu-id="d121c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d121c-152">Int32</span></span>|<span data-ttu-id="d121c-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d121c-153">Version of the device configuration.</span></span> <span data-ttu-id="d121c-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d121c-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d121c-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d121c-155">passwordRequired</span></span>|<span data-ttu-id="d121c-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-156">Boolean</span></span>|<span data-ttu-id="d121c-157">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="d121c-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="d121c-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d121c-158">passwordBlockSimple</span></span>|<span data-ttu-id="d121c-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-159">Boolean</span></span>|<span data-ttu-id="d121c-160">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d121c-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="d121c-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="d121c-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="d121c-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-162">Boolean</span></span>|<span data-ttu-id="d121c-163">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="d121c-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="d121c-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d121c-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d121c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d121c-165">Int32</span></span>|<span data-ttu-id="d121c-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="d121c-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d121c-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d121c-167">passwordExpirationDays</span></span>|<span data-ttu-id="d121c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d121c-168">Int32</span></span>|<span data-ttu-id="d121c-169">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="d121c-169">The password expiration in days.</span></span>|
|<span data-ttu-id="d121c-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d121c-170">passwordMinimumLength</span></span>|<span data-ttu-id="d121c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d121c-171">Int32</span></span>|<span data-ttu-id="d121c-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="d121c-172">The minimum password length.</span></span>|
|<span data-ttu-id="d121c-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d121c-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d121c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="d121c-174">Int32</span></span>|<span data-ttu-id="d121c-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="d121c-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d121c-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d121c-176">passwordRequiredType</span></span>|[<span data-ttu-id="d121c-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d121c-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d121c-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="d121c-178">The required password type.</span></span> <span data-ttu-id="d121c-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d121c-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d121c-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d121c-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d121c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d121c-181">Int32</span></span>|<span data-ttu-id="d121c-182">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="d121c-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="d121c-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="d121c-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="d121c-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-184">Boolean</span></span>|<span data-ttu-id="d121c-185">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="d121c-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="d121c-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d121c-186">osMinimumVersion</span></span>|<span data-ttu-id="d121c-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-187">String</span></span>|<span data-ttu-id="d121c-188">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d121c-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="d121c-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d121c-189">osMaximumVersion</span></span>|<span data-ttu-id="d121c-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-190">String</span></span>|<span data-ttu-id="d121c-191">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d121c-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="d121c-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d121c-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="d121c-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-193">String</span></span>|<span data-ttu-id="d121c-194">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d121c-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="d121c-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d121c-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="d121c-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d121c-196">String</span></span>|<span data-ttu-id="d121c-197">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d121c-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="d121c-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="d121c-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="d121c-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-199">Boolean</span></span>|<span data-ttu-id="d121c-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="d121c-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="d121c-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="d121c-201">bitLockerEnabled</span></span>|<span data-ttu-id="d121c-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-202">Boolean</span></span>|<span data-ttu-id="d121c-203">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="d121c-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="d121c-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="d121c-204">secureBootEnabled</span></span>|<span data-ttu-id="d121c-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-205">Boolean</span></span>|<span data-ttu-id="d121c-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="d121c-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="d121c-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="d121c-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="d121c-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-208">Boolean</span></span>|<span data-ttu-id="d121c-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="d121c-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="d121c-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d121c-210">storageRequireEncryption</span></span>|<span data-ttu-id="d121c-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="d121c-211">Boolean</span></span>|<span data-ttu-id="d121c-212">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="d121c-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="d121c-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="d121c-213">Response</span></span>
<span data-ttu-id="d121c-214">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d121c-214">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d121c-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d121c-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="d121c-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d121c-216">Request</span></span>
<span data-ttu-id="d121c-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d121c-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="d121c-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="d121c-218">Response</span></span>
<span data-ttu-id="d121c-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d121c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



