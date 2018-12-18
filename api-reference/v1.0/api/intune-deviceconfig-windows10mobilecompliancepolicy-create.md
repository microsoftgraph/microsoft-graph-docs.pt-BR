---
title: Criar windows10MobileCompliancePolicy
description: Cria um novo objeto windows10MobileCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 2d0c7c4a4f27ad723f8d29a24fc20d1fddd2633f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324280"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="3e4f8-103">Criar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3e4f8-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="3e4f8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e4f8-105">Cria um novo objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3e4f8-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e4f8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e4f8-106">Prerequisites</span></span>
<span data-ttu-id="3e4f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e4f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e4f8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e4f8-109">Permission type</span></span>|<span data-ttu-id="3e4f8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e4f8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e4f8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4f8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e4f8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e4f8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-114">Not supported.</span></span>|
|<span data-ttu-id="3e4f8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e4f8-115">Application</span></span>|<span data-ttu-id="3e4f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e4f8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e4f8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3e4f8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4f8-118">Request headers</span></span>
|<span data-ttu-id="3e4f8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e4f8-119">Header</span></span>|<span data-ttu-id="3e4f8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3e4f8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e4f8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e4f8-121">Authorization</span></span>|<span data-ttu-id="3e4f8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e4f8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3e4f8-123">Accept</span></span>|<span data-ttu-id="3e4f8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3e4f8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4f8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4f8-125">Request body</span></span>
<span data-ttu-id="3e4f8-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="3e4f8-127">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="3e4f8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e4f8-128">Property</span></span>|<span data-ttu-id="3e4f8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e4f8-129">Type</span></span>|<span data-ttu-id="3e4f8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e4f8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e4f8-131">id</span><span class="sxs-lookup"><span data-stu-id="3e4f8-131">id</span></span>|<span data-ttu-id="3e4f8-132">String</span><span class="sxs-lookup"><span data-stu-id="3e4f8-132">String</span></span>|<span data-ttu-id="3e4f8-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-133">Key of the entity.</span></span> <span data-ttu-id="3e4f8-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3e4f8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4f8-135">createdDateTime</span></span>|<span data-ttu-id="3e4f8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4f8-136">DateTimeOffset</span></span>|<span data-ttu-id="3e4f8-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-137">DateTime the object was created.</span></span> <span data-ttu-id="3e4f8-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3e4f8-139">description</span><span class="sxs-lookup"><span data-stu-id="3e4f8-139">description</span></span>|<span data-ttu-id="3e4f8-140">String</span><span class="sxs-lookup"><span data-stu-id="3e4f8-140">String</span></span>|<span data-ttu-id="3e4f8-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e4f8-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3e4f8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4f8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3e4f8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4f8-144">DateTimeOffset</span></span>|<span data-ttu-id="3e4f8-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-145">DateTime the object was last modified.</span></span> <span data-ttu-id="3e4f8-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3e4f8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3e4f8-147">displayName</span></span>|<span data-ttu-id="3e4f8-148">String</span><span class="sxs-lookup"><span data-stu-id="3e4f8-148">String</span></span>|<span data-ttu-id="3e4f8-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e4f8-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3e4f8-151">version</span><span class="sxs-lookup"><span data-stu-id="3e4f8-151">version</span></span>|<span data-ttu-id="3e4f8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4f8-152">Int32</span></span>|<span data-ttu-id="3e4f8-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-153">Version of the device configuration.</span></span> <span data-ttu-id="3e4f8-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3e4f8-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3e4f8-155">passwordRequired</span></span>|<span data-ttu-id="3e4f8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-156">Boolean</span></span>|<span data-ttu-id="3e4f8-157">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="3e4f8-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3e4f8-158">passwordBlockSimple</span></span>|<span data-ttu-id="3e4f8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-159">Boolean</span></span>|<span data-ttu-id="3e4f8-160">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="3e4f8-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3e4f8-161">passwordMinimumLength</span></span>|<span data-ttu-id="3e4f8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4f8-162">Int32</span></span>|<span data-ttu-id="3e4f8-163">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-163">Minimum password length.</span></span> <span data-ttu-id="3e4f8-164">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="3e4f8-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3e4f8-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3e4f8-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3e4f8-166">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4f8-166">Int32</span></span>|<span data-ttu-id="3e4f8-167">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3e4f8-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3e4f8-168">passwordRequiredType</span></span>|[<span data-ttu-id="3e4f8-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3e4f8-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3e4f8-170">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-170">The required password type.</span></span> <span data-ttu-id="3e4f8-171">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3e4f8-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3e4f8-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3e4f8-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4f8-173">Int32</span></span>|<span data-ttu-id="3e4f8-174">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="3e4f8-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3e4f8-175">passwordExpirationDays</span></span>|<span data-ttu-id="3e4f8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4f8-176">Int32</span></span>|<span data-ttu-id="3e4f8-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-177">Number of days before password expiration.</span></span> <span data-ttu-id="3e4f8-178">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="3e4f8-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="3e4f8-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3e4f8-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3e4f8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4f8-180">Int32</span></span>|<span data-ttu-id="3e4f8-181">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3e4f8-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="3e4f8-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="3e4f8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-183">Boolean</span></span>|<span data-ttu-id="3e4f8-184">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="3e4f8-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3e4f8-185">osMinimumVersion</span></span>|<span data-ttu-id="3e4f8-186">String</span><span class="sxs-lookup"><span data-stu-id="3e4f8-186">String</span></span>|<span data-ttu-id="3e4f8-187">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="3e4f8-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3e4f8-188">osMaximumVersion</span></span>|<span data-ttu-id="3e4f8-189">String</span><span class="sxs-lookup"><span data-stu-id="3e4f8-189">String</span></span>|<span data-ttu-id="3e4f8-190">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="3e4f8-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="3e4f8-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="3e4f8-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-192">Boolean</span></span>|<span data-ttu-id="3e4f8-193">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="3e4f8-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="3e4f8-194">bitLockerEnabled</span></span>|<span data-ttu-id="3e4f8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-195">Boolean</span></span>|<span data-ttu-id="3e4f8-196">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="3e4f8-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="3e4f8-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="3e4f8-197">secureBootEnabled</span></span>|<span data-ttu-id="3e4f8-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-198">Boolean</span></span>|<span data-ttu-id="3e4f8-199">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="3e4f8-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="3e4f8-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="3e4f8-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-201">Boolean</span></span>|<span data-ttu-id="3e4f8-202">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3e4f8-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3e4f8-203">storageRequireEncryption</span></span>|<span data-ttu-id="3e4f8-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e4f8-204">Boolean</span></span>|<span data-ttu-id="3e4f8-205">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="3e4f8-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e4f8-206">Response</span></span>
<span data-ttu-id="3e4f8-207">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4f8-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e4f8-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e4f8-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4f8-209">Request</span></span>
<span data-ttu-id="3e4f8-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="3e4f8-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e4f8-211">Response</span></span>
<span data-ttu-id="3e4f8-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```



