---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bbb9f2966d0c643c8b48a3582403127517f116b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514203"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="7d959-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7d959-103">Create windows10CompliancePolicy</span></span>

<span data-ttu-id="7d959-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d959-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d959-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d959-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d959-106">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7d959-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d959-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d959-107">Prerequisites</span></span>
<span data-ttu-id="7d959-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d959-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d959-110">Permission type</span></span>|<span data-ttu-id="7d959-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d959-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d959-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d959-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d959-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d959-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d959-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d959-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d959-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d959-115">Not supported.</span></span>|
|<span data-ttu-id="7d959-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d959-116">Application</span></span>|<span data-ttu-id="7d959-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d959-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d959-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d959-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7d959-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d959-119">Request headers</span></span>
|<span data-ttu-id="7d959-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d959-120">Header</span></span>|<span data-ttu-id="7d959-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d959-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d959-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d959-122">Authorization</span></span>|<span data-ttu-id="7d959-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d959-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d959-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d959-124">Accept</span></span>|<span data-ttu-id="7d959-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d959-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d959-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d959-126">Request body</span></span>
<span data-ttu-id="7d959-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7d959-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="7d959-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7d959-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="7d959-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d959-129">Property</span></span>|<span data-ttu-id="7d959-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d959-130">Type</span></span>|<span data-ttu-id="7d959-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d959-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d959-132">id</span><span class="sxs-lookup"><span data-stu-id="7d959-132">id</span></span>|<span data-ttu-id="7d959-133">String</span><span class="sxs-lookup"><span data-stu-id="7d959-133">String</span></span>|<span data-ttu-id="7d959-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d959-134">Key of the entity.</span></span> <span data-ttu-id="7d959-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d959-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d959-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d959-136">createdDateTime</span></span>|<span data-ttu-id="7d959-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d959-137">DateTimeOffset</span></span>|<span data-ttu-id="7d959-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7d959-138">DateTime the object was created.</span></span> <span data-ttu-id="7d959-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d959-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d959-140">description</span><span class="sxs-lookup"><span data-stu-id="7d959-140">description</span></span>|<span data-ttu-id="7d959-141">String</span><span class="sxs-lookup"><span data-stu-id="7d959-141">String</span></span>|<span data-ttu-id="7d959-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d959-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d959-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d959-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d959-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d959-144">lastModifiedDateTime</span></span>|<span data-ttu-id="7d959-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d959-145">DateTimeOffset</span></span>|<span data-ttu-id="7d959-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7d959-146">DateTime the object was last modified.</span></span> <span data-ttu-id="7d959-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d959-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d959-148">displayName</span><span class="sxs-lookup"><span data-stu-id="7d959-148">displayName</span></span>|<span data-ttu-id="7d959-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d959-149">String</span></span>|<span data-ttu-id="7d959-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d959-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d959-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d959-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d959-152">version</span><span class="sxs-lookup"><span data-stu-id="7d959-152">version</span></span>|<span data-ttu-id="7d959-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7d959-153">Int32</span></span>|<span data-ttu-id="7d959-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d959-154">Version of the device configuration.</span></span> <span data-ttu-id="7d959-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d959-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7d959-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7d959-156">passwordRequired</span></span>|<span data-ttu-id="7d959-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-157">Boolean</span></span>|<span data-ttu-id="7d959-158">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="7d959-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="7d959-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7d959-159">passwordBlockSimple</span></span>|<span data-ttu-id="7d959-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-160">Boolean</span></span>|<span data-ttu-id="7d959-161">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7d959-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="7d959-162">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="7d959-162">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="7d959-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-163">Boolean</span></span>|<span data-ttu-id="7d959-164">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="7d959-164">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="7d959-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7d959-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7d959-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7d959-166">Int32</span></span>|<span data-ttu-id="7d959-167">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="7d959-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7d959-168">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7d959-168">passwordExpirationDays</span></span>|<span data-ttu-id="7d959-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7d959-169">Int32</span></span>|<span data-ttu-id="7d959-170">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="7d959-170">The password expiration in days.</span></span>|
|<span data-ttu-id="7d959-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7d959-171">passwordMinimumLength</span></span>|<span data-ttu-id="7d959-172">Int32</span><span class="sxs-lookup"><span data-stu-id="7d959-172">Int32</span></span>|<span data-ttu-id="7d959-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="7d959-173">The minimum password length.</span></span>|
|<span data-ttu-id="7d959-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7d959-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7d959-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7d959-175">Int32</span></span>|<span data-ttu-id="7d959-176">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="7d959-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7d959-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7d959-177">passwordRequiredType</span></span>|[<span data-ttu-id="7d959-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7d959-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7d959-179">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="7d959-179">The required password type.</span></span> <span data-ttu-id="7d959-180">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7d959-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7d959-181">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7d959-181">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7d959-182">Int32</span><span class="sxs-lookup"><span data-stu-id="7d959-182">Int32</span></span>|<span data-ttu-id="7d959-183">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="7d959-183">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="7d959-184">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="7d959-184">requireHealthyDeviceReport</span></span>|<span data-ttu-id="7d959-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-185">Boolean</span></span>|<span data-ttu-id="7d959-186">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="7d959-186">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7d959-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7d959-187">osMinimumVersion</span></span>|<span data-ttu-id="7d959-188">String</span><span class="sxs-lookup"><span data-stu-id="7d959-188">String</span></span>|<span data-ttu-id="7d959-189">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7d959-189">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="7d959-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7d959-190">osMaximumVersion</span></span>|<span data-ttu-id="7d959-191">String</span><span class="sxs-lookup"><span data-stu-id="7d959-191">String</span></span>|<span data-ttu-id="7d959-192">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7d959-192">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="7d959-193">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7d959-193">mobileOsMinimumVersion</span></span>|<span data-ttu-id="7d959-194">String</span><span class="sxs-lookup"><span data-stu-id="7d959-194">String</span></span>|<span data-ttu-id="7d959-195">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="7d959-195">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7d959-196">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7d959-196">mobileOsMaximumVersion</span></span>|<span data-ttu-id="7d959-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d959-197">String</span></span>|<span data-ttu-id="7d959-198">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="7d959-198">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7d959-199">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="7d959-199">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="7d959-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-200">Boolean</span></span>|<span data-ttu-id="7d959-201">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="7d959-201">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="7d959-202">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="7d959-202">bitLockerEnabled</span></span>|<span data-ttu-id="7d959-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-203">Boolean</span></span>|<span data-ttu-id="7d959-204">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="7d959-204">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="7d959-205">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="7d959-205">secureBootEnabled</span></span>|<span data-ttu-id="7d959-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d959-206">Boolean</span></span>|<span data-ttu-id="7d959-207">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="7d959-207">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="7d959-208">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="7d959-208">codeIntegrityEnabled</span></span>|<span data-ttu-id="7d959-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d959-209">Boolean</span></span>|<span data-ttu-id="7d959-210">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="7d959-210">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7d959-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7d959-211">storageRequireEncryption</span></span>|<span data-ttu-id="7d959-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d959-212">Boolean</span></span>|<span data-ttu-id="7d959-213">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="7d959-213">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7d959-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d959-214">Response</span></span>
<span data-ttu-id="7d959-215">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d959-215">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d959-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d959-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d959-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d959-217">Request</span></span>
<span data-ttu-id="7d959-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d959-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d959-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d959-219">Response</span></span>
<span data-ttu-id="7d959-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d959-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




