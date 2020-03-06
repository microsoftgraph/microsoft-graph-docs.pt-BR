---
title: Criar windows10MobileCompliancePolicy
description: Cria um novo objeto windows10MobileCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11b8b543ea442fc7de448efead59dc28342a87be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514011"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="426f1-103">Criar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="426f1-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="426f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="426f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="426f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="426f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="426f1-106">Cria um novo objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="426f1-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="426f1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="426f1-107">Prerequisites</span></span>
<span data-ttu-id="426f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="426f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="426f1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="426f1-110">Permission type</span></span>|<span data-ttu-id="426f1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="426f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="426f1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="426f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="426f1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="426f1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="426f1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="426f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="426f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="426f1-115">Not supported.</span></span>|
|<span data-ttu-id="426f1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="426f1-116">Application</span></span>|<span data-ttu-id="426f1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="426f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="426f1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="426f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="426f1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="426f1-119">Request headers</span></span>
|<span data-ttu-id="426f1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="426f1-120">Header</span></span>|<span data-ttu-id="426f1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="426f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="426f1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="426f1-122">Authorization</span></span>|<span data-ttu-id="426f1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="426f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="426f1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="426f1-124">Accept</span></span>|<span data-ttu-id="426f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="426f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="426f1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="426f1-126">Request body</span></span>
<span data-ttu-id="426f1-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="426f1-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="426f1-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="426f1-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="426f1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="426f1-129">Property</span></span>|<span data-ttu-id="426f1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="426f1-130">Type</span></span>|<span data-ttu-id="426f1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="426f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="426f1-132">id</span><span class="sxs-lookup"><span data-stu-id="426f1-132">id</span></span>|<span data-ttu-id="426f1-133">String</span><span class="sxs-lookup"><span data-stu-id="426f1-133">String</span></span>|<span data-ttu-id="426f1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="426f1-134">Key of the entity.</span></span> <span data-ttu-id="426f1-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="426f1-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="426f1-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="426f1-136">createdDateTime</span></span>|<span data-ttu-id="426f1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426f1-137">DateTimeOffset</span></span>|<span data-ttu-id="426f1-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="426f1-138">DateTime the object was created.</span></span> <span data-ttu-id="426f1-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="426f1-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="426f1-140">description</span><span class="sxs-lookup"><span data-stu-id="426f1-140">description</span></span>|<span data-ttu-id="426f1-141">String</span><span class="sxs-lookup"><span data-stu-id="426f1-141">String</span></span>|<span data-ttu-id="426f1-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="426f1-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="426f1-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="426f1-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="426f1-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="426f1-144">lastModifiedDateTime</span></span>|<span data-ttu-id="426f1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426f1-145">DateTimeOffset</span></span>|<span data-ttu-id="426f1-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="426f1-146">DateTime the object was last modified.</span></span> <span data-ttu-id="426f1-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="426f1-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="426f1-148">displayName</span><span class="sxs-lookup"><span data-stu-id="426f1-148">displayName</span></span>|<span data-ttu-id="426f1-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="426f1-149">String</span></span>|<span data-ttu-id="426f1-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="426f1-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="426f1-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="426f1-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="426f1-152">version</span><span class="sxs-lookup"><span data-stu-id="426f1-152">version</span></span>|<span data-ttu-id="426f1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="426f1-153">Int32</span></span>|<span data-ttu-id="426f1-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="426f1-154">Version of the device configuration.</span></span> <span data-ttu-id="426f1-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="426f1-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="426f1-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="426f1-156">passwordRequired</span></span>|<span data-ttu-id="426f1-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="426f1-157">Boolean</span></span>|<span data-ttu-id="426f1-158">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="426f1-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="426f1-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="426f1-159">passwordBlockSimple</span></span>|<span data-ttu-id="426f1-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="426f1-160">Boolean</span></span>|<span data-ttu-id="426f1-161">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="426f1-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="426f1-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="426f1-162">passwordMinimumLength</span></span>|<span data-ttu-id="426f1-163">Int32</span><span class="sxs-lookup"><span data-stu-id="426f1-163">Int32</span></span>|<span data-ttu-id="426f1-164">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="426f1-164">Minimum password length.</span></span> <span data-ttu-id="426f1-165">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="426f1-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="426f1-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="426f1-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="426f1-167">Int32</span><span class="sxs-lookup"><span data-stu-id="426f1-167">Int32</span></span>|<span data-ttu-id="426f1-168">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="426f1-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="426f1-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="426f1-169">passwordRequiredType</span></span>|[<span data-ttu-id="426f1-170">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="426f1-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="426f1-171">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="426f1-171">The required password type.</span></span> <span data-ttu-id="426f1-172">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="426f1-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="426f1-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="426f1-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="426f1-174">Int32</span><span class="sxs-lookup"><span data-stu-id="426f1-174">Int32</span></span>|<span data-ttu-id="426f1-175">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="426f1-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="426f1-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="426f1-176">passwordExpirationDays</span></span>|<span data-ttu-id="426f1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="426f1-177">Int32</span></span>|<span data-ttu-id="426f1-178">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="426f1-178">Number of days before password expiration.</span></span> <span data-ttu-id="426f1-179">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="426f1-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="426f1-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="426f1-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="426f1-181">Int32</span><span class="sxs-lookup"><span data-stu-id="426f1-181">Int32</span></span>|<span data-ttu-id="426f1-182">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="426f1-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="426f1-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="426f1-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="426f1-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="426f1-184">Boolean</span></span>|<span data-ttu-id="426f1-185">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="426f1-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="426f1-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="426f1-186">osMinimumVersion</span></span>|<span data-ttu-id="426f1-187">String</span><span class="sxs-lookup"><span data-stu-id="426f1-187">String</span></span>|<span data-ttu-id="426f1-188">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="426f1-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="426f1-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="426f1-189">osMaximumVersion</span></span>|<span data-ttu-id="426f1-190">String</span><span class="sxs-lookup"><span data-stu-id="426f1-190">String</span></span>|<span data-ttu-id="426f1-191">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="426f1-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="426f1-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="426f1-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="426f1-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="426f1-193">Boolean</span></span>|<span data-ttu-id="426f1-194">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="426f1-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="426f1-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="426f1-195">bitLockerEnabled</span></span>|<span data-ttu-id="426f1-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="426f1-196">Boolean</span></span>|<span data-ttu-id="426f1-197">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="426f1-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="426f1-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="426f1-198">secureBootEnabled</span></span>|<span data-ttu-id="426f1-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="426f1-199">Boolean</span></span>|<span data-ttu-id="426f1-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="426f1-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="426f1-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="426f1-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="426f1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="426f1-202">Boolean</span></span>|<span data-ttu-id="426f1-203">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="426f1-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="426f1-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="426f1-204">storageRequireEncryption</span></span>|<span data-ttu-id="426f1-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="426f1-205">Boolean</span></span>|<span data-ttu-id="426f1-206">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="426f1-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="426f1-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="426f1-207">Response</span></span>
<span data-ttu-id="426f1-208">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="426f1-208">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="426f1-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="426f1-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="426f1-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="426f1-210">Request</span></span>
<span data-ttu-id="426f1-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="426f1-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="426f1-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="426f1-212">Response</span></span>
<span data-ttu-id="426f1-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="426f1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




