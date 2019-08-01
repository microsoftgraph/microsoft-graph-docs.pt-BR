---
title: Atualizar windows10CompliancePolicy
description: Atualiza as propriedades de um objeto windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d894e85cbd1821f9223b3951c8c88756b90509b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016920"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="b7179-103">Atualizar windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b7179-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="b7179-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7179-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7179-105">Atualiza as propriedades de um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b7179-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7179-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7179-106">Prerequisites</span></span>
<span data-ttu-id="b7179-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7179-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7179-109">Permission type</span></span>|<span data-ttu-id="b7179-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7179-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7179-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7179-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7179-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7179-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7179-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7179-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7179-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7179-114">Not supported.</span></span>|
|<span data-ttu-id="b7179-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7179-115">Application</span></span>|<span data-ttu-id="b7179-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7179-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7179-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7179-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b7179-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7179-118">Request headers</span></span>
|<span data-ttu-id="b7179-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7179-119">Header</span></span>|<span data-ttu-id="b7179-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b7179-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7179-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7179-121">Authorization</span></span>|<span data-ttu-id="b7179-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7179-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7179-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7179-123">Accept</span></span>|<span data-ttu-id="b7179-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7179-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7179-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7179-125">Request body</span></span>
<span data-ttu-id="b7179-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b7179-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="b7179-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b7179-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="b7179-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7179-128">Property</span></span>|<span data-ttu-id="b7179-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7179-129">Type</span></span>|<span data-ttu-id="b7179-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7179-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7179-131">id</span><span class="sxs-lookup"><span data-stu-id="b7179-131">id</span></span>|<span data-ttu-id="b7179-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7179-132">String</span></span>|<span data-ttu-id="b7179-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7179-133">Key of the entity.</span></span> <span data-ttu-id="b7179-134">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7179-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b7179-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7179-135">createdDateTime</span></span>|<span data-ttu-id="b7179-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7179-136">DateTimeOffset</span></span>|<span data-ttu-id="b7179-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b7179-137">DateTime the object was created.</span></span> <span data-ttu-id="b7179-138">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7179-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b7179-139">descrição</span><span class="sxs-lookup"><span data-stu-id="b7179-139">description</span></span>|<span data-ttu-id="b7179-140">String</span><span class="sxs-lookup"><span data-stu-id="b7179-140">String</span></span>|<span data-ttu-id="b7179-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7179-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b7179-142">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7179-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b7179-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7179-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b7179-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7179-144">DateTimeOffset</span></span>|<span data-ttu-id="b7179-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b7179-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b7179-146">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7179-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b7179-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b7179-147">displayName</span></span>|<span data-ttu-id="b7179-148">String</span><span class="sxs-lookup"><span data-stu-id="b7179-148">String</span></span>|<span data-ttu-id="b7179-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7179-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b7179-150">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7179-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b7179-151">version</span><span class="sxs-lookup"><span data-stu-id="b7179-151">version</span></span>|<span data-ttu-id="b7179-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b7179-152">Int32</span></span>|<span data-ttu-id="b7179-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7179-153">Version of the device configuration.</span></span> <span data-ttu-id="b7179-154">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7179-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b7179-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b7179-155">passwordRequired</span></span>|<span data-ttu-id="b7179-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-156">Boolean</span></span>|<span data-ttu-id="b7179-157">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b7179-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b7179-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b7179-158">passwordBlockSimple</span></span>|<span data-ttu-id="b7179-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-159">Boolean</span></span>|<span data-ttu-id="b7179-160">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b7179-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b7179-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="b7179-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="b7179-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-162">Boolean</span></span>|<span data-ttu-id="b7179-163">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="b7179-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="b7179-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b7179-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b7179-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b7179-165">Int32</span></span>|<span data-ttu-id="b7179-166">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="b7179-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b7179-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b7179-167">passwordExpirationDays</span></span>|<span data-ttu-id="b7179-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b7179-168">Int32</span></span>|<span data-ttu-id="b7179-169">A expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="b7179-169">The password expiration in days.</span></span>|
|<span data-ttu-id="b7179-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b7179-170">passwordMinimumLength</span></span>|<span data-ttu-id="b7179-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b7179-171">Int32</span></span>|<span data-ttu-id="b7179-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="b7179-172">The minimum password length.</span></span>|
|<span data-ttu-id="b7179-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b7179-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b7179-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b7179-174">Int32</span></span>|<span data-ttu-id="b7179-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="b7179-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b7179-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b7179-176">passwordRequiredType</span></span>|[<span data-ttu-id="b7179-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b7179-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b7179-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="b7179-178">The required password type.</span></span> <span data-ttu-id="b7179-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b7179-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b7179-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b7179-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b7179-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b7179-181">Int32</span></span>|<span data-ttu-id="b7179-182">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="b7179-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="b7179-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="b7179-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="b7179-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-184">Boolean</span></span>|<span data-ttu-id="b7179-185">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b7179-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b7179-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b7179-186">osMinimumVersion</span></span>|<span data-ttu-id="b7179-187">String</span><span class="sxs-lookup"><span data-stu-id="b7179-187">String</span></span>|<span data-ttu-id="b7179-188">Versão mínima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b7179-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="b7179-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b7179-189">osMaximumVersion</span></span>|<span data-ttu-id="b7179-190">String</span><span class="sxs-lookup"><span data-stu-id="b7179-190">String</span></span>|<span data-ttu-id="b7179-191">Versão máxima do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b7179-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="b7179-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b7179-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="b7179-193">String</span><span class="sxs-lookup"><span data-stu-id="b7179-193">String</span></span>|<span data-ttu-id="b7179-194">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b7179-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="b7179-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b7179-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="b7179-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7179-196">String</span></span>|<span data-ttu-id="b7179-197">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b7179-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="b7179-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="b7179-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="b7179-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-199">Boolean</span></span>|<span data-ttu-id="b7179-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="b7179-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="b7179-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="b7179-201">bitLockerEnabled</span></span>|<span data-ttu-id="b7179-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-202">Boolean</span></span>|<span data-ttu-id="b7179-203">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="b7179-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="b7179-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="b7179-204">secureBootEnabled</span></span>|<span data-ttu-id="b7179-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7179-205">Boolean</span></span>|<span data-ttu-id="b7179-206">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="b7179-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="b7179-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="b7179-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="b7179-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7179-208">Boolean</span></span>|<span data-ttu-id="b7179-209">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b7179-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b7179-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b7179-210">storageRequireEncryption</span></span>|<span data-ttu-id="b7179-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7179-211">Boolean</span></span>|<span data-ttu-id="b7179-212">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b7179-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b7179-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7179-213">Response</span></span>
<span data-ttu-id="b7179-214">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7179-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7179-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7179-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7179-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7179-216">Request</span></span>
<span data-ttu-id="b7179-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7179-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7179-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7179-218">Response</span></span>
<span data-ttu-id="b7179-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7179-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



