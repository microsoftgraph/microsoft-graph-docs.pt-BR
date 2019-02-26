---
title: Criar windows10CompliancePolicy
description: Cria um novo objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85f550b95e5a751b379998e753b05b4bc68254ce
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253873"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="15e76-103">Criar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="15e76-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="15e76-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15e76-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15e76-105">Cria um novo objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="15e76-105">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15e76-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15e76-106">Prerequisites</span></span>
<span data-ttu-id="15e76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15e76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15e76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15e76-109">Permission type</span></span>|<span data-ttu-id="15e76-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15e76-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15e76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15e76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15e76-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15e76-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15e76-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15e76-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15e76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15e76-114">Not supported.</span></span>|
|<span data-ttu-id="15e76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15e76-115">Application</span></span>|<span data-ttu-id="15e76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15e76-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15e76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15e76-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="15e76-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15e76-118">Request headers</span></span>
|<span data-ttu-id="15e76-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15e76-119">Header</span></span>|<span data-ttu-id="15e76-120">Valor</span><span class="sxs-lookup"><span data-stu-id="15e76-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15e76-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="15e76-121">Authorization</span></span>|<span data-ttu-id="15e76-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15e76-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15e76-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15e76-123">Accept</span></span>|<span data-ttu-id="15e76-124">application/json</span><span class="sxs-lookup"><span data-stu-id="15e76-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15e76-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15e76-125">Request body</span></span>
<span data-ttu-id="15e76-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="15e76-126">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="15e76-127">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="15e76-127">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="15e76-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15e76-128">Property</span></span>|<span data-ttu-id="15e76-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="15e76-129">Type</span></span>|<span data-ttu-id="15e76-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="15e76-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e76-131">id</span><span class="sxs-lookup"><span data-stu-id="15e76-131">id</span></span>|<span data-ttu-id="15e76-132">String</span><span class="sxs-lookup"><span data-stu-id="15e76-132">String</span></span>|<span data-ttu-id="15e76-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15e76-133">Key of the entity.</span></span> <span data-ttu-id="15e76-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15e76-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="15e76-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15e76-135">createdDateTime</span></span>|<span data-ttu-id="15e76-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e76-136">DateTimeOffset</span></span>|<span data-ttu-id="15e76-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="15e76-137">DateTime the object was created.</span></span> <span data-ttu-id="15e76-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15e76-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="15e76-139">description</span><span class="sxs-lookup"><span data-stu-id="15e76-139">description</span></span>|<span data-ttu-id="15e76-140">String</span><span class="sxs-lookup"><span data-stu-id="15e76-140">String</span></span>|<span data-ttu-id="15e76-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15e76-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15e76-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15e76-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="15e76-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15e76-143">lastModifiedDateTime</span></span>|<span data-ttu-id="15e76-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15e76-144">DateTimeOffset</span></span>|<span data-ttu-id="15e76-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="15e76-145">DateTime the object was last modified.</span></span> <span data-ttu-id="15e76-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15e76-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="15e76-147">displayName</span><span class="sxs-lookup"><span data-stu-id="15e76-147">displayName</span></span>|<span data-ttu-id="15e76-148">String</span><span class="sxs-lookup"><span data-stu-id="15e76-148">String</span></span>|<span data-ttu-id="15e76-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15e76-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15e76-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15e76-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="15e76-151">version</span><span class="sxs-lookup"><span data-stu-id="15e76-151">version</span></span>|<span data-ttu-id="15e76-152">Int32</span><span class="sxs-lookup"><span data-stu-id="15e76-152">Int32</span></span>|<span data-ttu-id="15e76-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15e76-153">Version of the device configuration.</span></span> <span data-ttu-id="15e76-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="15e76-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="15e76-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="15e76-155">passwordRequired</span></span>|<span data-ttu-id="15e76-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-156">Boolean</span></span>|<span data-ttu-id="15e76-157">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="15e76-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="15e76-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="15e76-158">passwordBlockSimple</span></span>|<span data-ttu-id="15e76-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-159">Boolean</span></span>|<span data-ttu-id="15e76-160">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="15e76-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="15e76-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="15e76-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="15e76-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-162">Boolean</span></span>|<span data-ttu-id="15e76-163">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="15e76-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="15e76-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="15e76-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="15e76-165">Int32</span><span class="sxs-lookup"><span data-stu-id="15e76-165">Int32</span></span>|<span data-ttu-id="15e76-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="15e76-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="15e76-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="15e76-167">passwordExpirationDays</span></span>|<span data-ttu-id="15e76-168">Int32</span><span class="sxs-lookup"><span data-stu-id="15e76-168">Int32</span></span>|<span data-ttu-id="15e76-169">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="15e76-169">The password expiration in days.</span></span>|
|<span data-ttu-id="15e76-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="15e76-170">passwordMinimumLength</span></span>|<span data-ttu-id="15e76-171">Int32</span><span class="sxs-lookup"><span data-stu-id="15e76-171">Int32</span></span>|<span data-ttu-id="15e76-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="15e76-172">The minimum password length.</span></span>|
|<span data-ttu-id="15e76-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="15e76-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="15e76-174">Int32</span><span class="sxs-lookup"><span data-stu-id="15e76-174">Int32</span></span>|<span data-ttu-id="15e76-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="15e76-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="15e76-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="15e76-176">passwordRequiredType</span></span>|[<span data-ttu-id="15e76-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="15e76-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="15e76-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="15e76-178">The required password type.</span></span> <span data-ttu-id="15e76-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="15e76-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="15e76-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="15e76-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="15e76-181">Int32</span><span class="sxs-lookup"><span data-stu-id="15e76-181">Int32</span></span>|<span data-ttu-id="15e76-182">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="15e76-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="15e76-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="15e76-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="15e76-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-184">Boolean</span></span>|<span data-ttu-id="15e76-185">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="15e76-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="15e76-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="15e76-186">osMinimumVersion</span></span>|<span data-ttu-id="15e76-187">String</span><span class="sxs-lookup"><span data-stu-id="15e76-187">String</span></span>|<span data-ttu-id="15e76-188">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="15e76-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="15e76-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="15e76-189">osMaximumVersion</span></span>|<span data-ttu-id="15e76-190">String</span><span class="sxs-lookup"><span data-stu-id="15e76-190">String</span></span>|<span data-ttu-id="15e76-191">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="15e76-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="15e76-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="15e76-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="15e76-193">String</span><span class="sxs-lookup"><span data-stu-id="15e76-193">String</span></span>|<span data-ttu-id="15e76-194">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="15e76-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="15e76-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="15e76-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="15e76-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15e76-196">String</span></span>|<span data-ttu-id="15e76-197">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="15e76-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="15e76-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="15e76-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="15e76-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-199">Boolean</span></span>|<span data-ttu-id="15e76-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="15e76-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="15e76-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="15e76-201">bitLockerEnabled</span></span>|<span data-ttu-id="15e76-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="15e76-202">Boolean</span></span>|<span data-ttu-id="15e76-203">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="15e76-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="15e76-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="15e76-204">secureBootEnabled</span></span>|<span data-ttu-id="15e76-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-205">Boolean</span></span>|<span data-ttu-id="15e76-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="15e76-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="15e76-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="15e76-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="15e76-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-208">Boolean</span></span>|<span data-ttu-id="15e76-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="15e76-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="15e76-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="15e76-210">storageRequireEncryption</span></span>|<span data-ttu-id="15e76-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="15e76-211">Boolean</span></span>|<span data-ttu-id="15e76-212">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="15e76-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="15e76-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="15e76-213">Response</span></span>
<span data-ttu-id="15e76-214">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15e76-214">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15e76-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15e76-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="15e76-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15e76-216">Request</span></span>
<span data-ttu-id="15e76-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15e76-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15e76-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="15e76-218">Response</span></span>
<span data-ttu-id="15e76-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15e76-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



