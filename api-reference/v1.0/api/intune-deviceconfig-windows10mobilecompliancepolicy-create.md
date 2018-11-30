---
title: Criar windows10MobileCompliancePolicy
description: Cria um novo objeto windows10MobileCompliancePolicy.
ms.openlocfilehash: 819f97b9512792bdfef03e82e9f1ee179dfee655
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005804"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="b6843-103">Criar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b6843-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="b6843-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6843-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6843-105">Cria um novo objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6843-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6843-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6843-106">Prerequisites</span></span>
<span data-ttu-id="b6843-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6843-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6843-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6843-109">Permission type</span></span>|<span data-ttu-id="b6843-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6843-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6843-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6843-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6843-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6843-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6843-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6843-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6843-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6843-114">Not supported.</span></span>|
|<span data-ttu-id="b6843-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6843-115">Application</span></span>|<span data-ttu-id="b6843-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6843-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6843-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6843-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b6843-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6843-118">Request headers</span></span>
|<span data-ttu-id="b6843-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6843-119">Header</span></span>|<span data-ttu-id="b6843-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b6843-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6843-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6843-121">Authorization</span></span>|<span data-ttu-id="b6843-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6843-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6843-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b6843-123">Accept</span></span>|<span data-ttu-id="b6843-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b6843-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6843-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6843-125">Request body</span></span>
<span data-ttu-id="b6843-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="b6843-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="b6843-127">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="b6843-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="b6843-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6843-128">Property</span></span>|<span data-ttu-id="b6843-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6843-129">Type</span></span>|<span data-ttu-id="b6843-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6843-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6843-131">id</span><span class="sxs-lookup"><span data-stu-id="b6843-131">id</span></span>|<span data-ttu-id="b6843-132">String</span><span class="sxs-lookup"><span data-stu-id="b6843-132">String</span></span>|<span data-ttu-id="b6843-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6843-133">Key of the entity.</span></span> <span data-ttu-id="b6843-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6843-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6843-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6843-135">createdDateTime</span></span>|<span data-ttu-id="b6843-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6843-136">DateTimeOffset</span></span>|<span data-ttu-id="b6843-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b6843-137">DateTime the object was created.</span></span> <span data-ttu-id="b6843-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6843-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6843-139">description</span><span class="sxs-lookup"><span data-stu-id="b6843-139">description</span></span>|<span data-ttu-id="b6843-140">String</span><span class="sxs-lookup"><span data-stu-id="b6843-140">String</span></span>|<span data-ttu-id="b6843-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6843-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6843-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6843-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6843-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6843-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b6843-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6843-144">DateTimeOffset</span></span>|<span data-ttu-id="b6843-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b6843-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b6843-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6843-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6843-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b6843-147">displayName</span></span>|<span data-ttu-id="b6843-148">String</span><span class="sxs-lookup"><span data-stu-id="b6843-148">String</span></span>|<span data-ttu-id="b6843-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6843-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6843-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6843-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6843-151">version</span><span class="sxs-lookup"><span data-stu-id="b6843-151">version</span></span>|<span data-ttu-id="b6843-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b6843-152">Int32</span></span>|<span data-ttu-id="b6843-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6843-153">Version of the device configuration.</span></span> <span data-ttu-id="b6843-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6843-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6843-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b6843-155">passwordRequired</span></span>|<span data-ttu-id="b6843-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-156">Boolean</span></span>|<span data-ttu-id="b6843-157">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b6843-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="b6843-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b6843-158">passwordBlockSimple</span></span>|<span data-ttu-id="b6843-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-159">Boolean</span></span>|<span data-ttu-id="b6843-160">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b6843-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="b6843-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6843-161">passwordMinimumLength</span></span>|<span data-ttu-id="b6843-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b6843-162">Int32</span></span>|<span data-ttu-id="b6843-163">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="b6843-163">Minimum password length.</span></span> <span data-ttu-id="b6843-164">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="b6843-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b6843-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b6843-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b6843-166">Int32</span><span class="sxs-lookup"><span data-stu-id="b6843-166">Int32</span></span>|<span data-ttu-id="b6843-167">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="b6843-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b6843-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6843-168">passwordRequiredType</span></span>|[<span data-ttu-id="b6843-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b6843-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b6843-170">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="b6843-170">The required password type.</span></span> <span data-ttu-id="b6843-171">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b6843-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b6843-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b6843-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b6843-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b6843-173">Int32</span></span>|<span data-ttu-id="b6843-174">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="b6843-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="b6843-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6843-175">passwordExpirationDays</span></span>|<span data-ttu-id="b6843-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b6843-176">Int32</span></span>|<span data-ttu-id="b6843-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="b6843-177">Number of days before password expiration.</span></span> <span data-ttu-id="b6843-178">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="b6843-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="b6843-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b6843-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b6843-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b6843-180">Int32</span></span>|<span data-ttu-id="b6843-181">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="b6843-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b6843-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="b6843-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="b6843-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-183">Boolean</span></span>|<span data-ttu-id="b6843-184">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="b6843-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="b6843-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b6843-185">osMinimumVersion</span></span>|<span data-ttu-id="b6843-186">String</span><span class="sxs-lookup"><span data-stu-id="b6843-186">String</span></span>|<span data-ttu-id="b6843-187">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b6843-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="b6843-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b6843-188">osMaximumVersion</span></span>|<span data-ttu-id="b6843-189">String</span><span class="sxs-lookup"><span data-stu-id="b6843-189">String</span></span>|<span data-ttu-id="b6843-190">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b6843-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="b6843-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="b6843-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="b6843-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-192">Boolean</span></span>|<span data-ttu-id="b6843-193">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="b6843-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="b6843-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="b6843-194">bitLockerEnabled</span></span>|<span data-ttu-id="b6843-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-195">Boolean</span></span>|<span data-ttu-id="b6843-196">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="b6843-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="b6843-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="b6843-197">secureBootEnabled</span></span>|<span data-ttu-id="b6843-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-198">Boolean</span></span>|<span data-ttu-id="b6843-199">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="b6843-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="b6843-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="b6843-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="b6843-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-201">Boolean</span></span>|<span data-ttu-id="b6843-202">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="b6843-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b6843-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b6843-203">storageRequireEncryption</span></span>|<span data-ttu-id="b6843-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6843-204">Boolean</span></span>|<span data-ttu-id="b6843-205">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="b6843-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b6843-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6843-206">Response</span></span>
<span data-ttu-id="b6843-207">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6843-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6843-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6843-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6843-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6843-209">Request</span></span>
<span data-ttu-id="b6843-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6843-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6843-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6843-211">Response</span></span>
<span data-ttu-id="b6843-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6843-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



