---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8264ab09f29e63a591d05ea0fc317c9933e850dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985192"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="34688-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="34688-103">Create windows10CompliancePolicy</span></span>

<span data-ttu-id="34688-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34688-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34688-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34688-106">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="34688-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34688-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34688-107">Prerequisites</span></span>
<span data-ttu-id="34688-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34688-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34688-110">Permission type</span></span>|<span data-ttu-id="34688-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34688-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34688-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34688-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34688-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34688-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34688-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34688-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34688-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34688-115">Not supported.</span></span>|
|<span data-ttu-id="34688-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34688-116">Application</span></span>|<span data-ttu-id="34688-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34688-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34688-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34688-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="34688-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34688-119">Request headers</span></span>
|<span data-ttu-id="34688-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34688-120">Header</span></span>|<span data-ttu-id="34688-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34688-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34688-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34688-122">Authorization</span></span>|<span data-ttu-id="34688-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34688-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34688-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34688-124">Accept</span></span>|<span data-ttu-id="34688-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34688-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34688-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34688-126">Request body</span></span>
<span data-ttu-id="34688-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="34688-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="34688-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="34688-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="34688-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34688-129">Property</span></span>|<span data-ttu-id="34688-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="34688-130">Type</span></span>|<span data-ttu-id="34688-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="34688-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34688-132">id</span><span class="sxs-lookup"><span data-stu-id="34688-132">id</span></span>|<span data-ttu-id="34688-133">String</span><span class="sxs-lookup"><span data-stu-id="34688-133">String</span></span>|<span data-ttu-id="34688-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34688-134">Key of the entity.</span></span> <span data-ttu-id="34688-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34688-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34688-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34688-136">createdDateTime</span></span>|<span data-ttu-id="34688-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34688-137">DateTimeOffset</span></span>|<span data-ttu-id="34688-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="34688-138">DateTime the object was created.</span></span> <span data-ttu-id="34688-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34688-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34688-140">description</span><span class="sxs-lookup"><span data-stu-id="34688-140">description</span></span>|<span data-ttu-id="34688-141">String</span><span class="sxs-lookup"><span data-stu-id="34688-141">String</span></span>|<span data-ttu-id="34688-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34688-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34688-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34688-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34688-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34688-144">lastModifiedDateTime</span></span>|<span data-ttu-id="34688-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34688-145">DateTimeOffset</span></span>|<span data-ttu-id="34688-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="34688-146">DateTime the object was last modified.</span></span> <span data-ttu-id="34688-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34688-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34688-148">displayName</span><span class="sxs-lookup"><span data-stu-id="34688-148">displayName</span></span>|<span data-ttu-id="34688-149">String</span><span class="sxs-lookup"><span data-stu-id="34688-149">String</span></span>|<span data-ttu-id="34688-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34688-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34688-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34688-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34688-152">version</span><span class="sxs-lookup"><span data-stu-id="34688-152">version</span></span>|<span data-ttu-id="34688-153">Int32</span><span class="sxs-lookup"><span data-stu-id="34688-153">Int32</span></span>|<span data-ttu-id="34688-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34688-154">Version of the device configuration.</span></span> <span data-ttu-id="34688-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34688-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34688-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="34688-156">passwordRequired</span></span>|<span data-ttu-id="34688-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="34688-157">Boolean</span></span>|<span data-ttu-id="34688-158">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="34688-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="34688-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="34688-159">passwordBlockSimple</span></span>|<span data-ttu-id="34688-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="34688-160">Boolean</span></span>|<span data-ttu-id="34688-161">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="34688-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="34688-162">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="34688-162">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="34688-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="34688-163">Boolean</span></span>|<span data-ttu-id="34688-164">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="34688-164">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="34688-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="34688-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="34688-166">Int32</span><span class="sxs-lookup"><span data-stu-id="34688-166">Int32</span></span>|<span data-ttu-id="34688-167">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="34688-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="34688-168">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="34688-168">passwordExpirationDays</span></span>|<span data-ttu-id="34688-169">Int32</span><span class="sxs-lookup"><span data-stu-id="34688-169">Int32</span></span>|<span data-ttu-id="34688-170">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="34688-170">The password expiration in days.</span></span>|
|<span data-ttu-id="34688-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="34688-171">passwordMinimumLength</span></span>|<span data-ttu-id="34688-172">Int32</span><span class="sxs-lookup"><span data-stu-id="34688-172">Int32</span></span>|<span data-ttu-id="34688-173">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="34688-173">The minimum password length.</span></span>|
|<span data-ttu-id="34688-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="34688-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="34688-175">Int32</span><span class="sxs-lookup"><span data-stu-id="34688-175">Int32</span></span>|<span data-ttu-id="34688-176">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="34688-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="34688-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="34688-177">passwordRequiredType</span></span>|[<span data-ttu-id="34688-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34688-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="34688-179">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="34688-179">The required password type.</span></span> <span data-ttu-id="34688-180">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="34688-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="34688-181">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="34688-181">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="34688-182">Int32</span><span class="sxs-lookup"><span data-stu-id="34688-182">Int32</span></span>|<span data-ttu-id="34688-183">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="34688-183">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="34688-184">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="34688-184">requireHealthyDeviceReport</span></span>|<span data-ttu-id="34688-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="34688-185">Boolean</span></span>|<span data-ttu-id="34688-186">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="34688-186">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="34688-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="34688-187">osMinimumVersion</span></span>|<span data-ttu-id="34688-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34688-188">String</span></span>|<span data-ttu-id="34688-189">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="34688-189">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="34688-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="34688-190">osMaximumVersion</span></span>|<span data-ttu-id="34688-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34688-191">String</span></span>|<span data-ttu-id="34688-192">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="34688-192">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="34688-193">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="34688-193">mobileOsMinimumVersion</span></span>|<span data-ttu-id="34688-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34688-194">String</span></span>|<span data-ttu-id="34688-195">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="34688-195">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="34688-196">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="34688-196">mobileOsMaximumVersion</span></span>|<span data-ttu-id="34688-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34688-197">String</span></span>|<span data-ttu-id="34688-198">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="34688-198">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="34688-199">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="34688-199">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="34688-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="34688-200">Boolean</span></span>|<span data-ttu-id="34688-201">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="34688-201">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="34688-202">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="34688-202">bitLockerEnabled</span></span>|<span data-ttu-id="34688-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="34688-203">Boolean</span></span>|<span data-ttu-id="34688-204">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="34688-204">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="34688-205">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="34688-205">secureBootEnabled</span></span>|<span data-ttu-id="34688-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="34688-206">Boolean</span></span>|<span data-ttu-id="34688-207">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="34688-207">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="34688-208">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="34688-208">codeIntegrityEnabled</span></span>|<span data-ttu-id="34688-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="34688-209">Boolean</span></span>|<span data-ttu-id="34688-210">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="34688-210">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="34688-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="34688-211">storageRequireEncryption</span></span>|<span data-ttu-id="34688-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="34688-212">Boolean</span></span>|<span data-ttu-id="34688-213">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="34688-213">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="34688-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="34688-214">Response</span></span>
<span data-ttu-id="34688-215">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34688-215">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34688-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34688-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="34688-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34688-217">Request</span></span>
<span data-ttu-id="34688-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34688-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34688-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="34688-219">Response</span></span>
<span data-ttu-id="34688-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34688-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









