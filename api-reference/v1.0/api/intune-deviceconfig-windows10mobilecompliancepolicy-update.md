---
title: Atualizar windows10MobileCompliancePolicy
description: Atualiza as propriedades de um objeto windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30b20277e1a52e8411cae960a4b4a12b17fba0a9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760486"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="690c6-103">Atualizar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="690c6-103">Update windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="690c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="690c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="690c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="690c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="690c6-106">Atualiza as propriedades de um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="690c6-106">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="690c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="690c6-107">Prerequisites</span></span>
<span data-ttu-id="690c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="690c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="690c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="690c6-110">Permission type</span></span>|<span data-ttu-id="690c6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="690c6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="690c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="690c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="690c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="690c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="690c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="690c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690c6-115">Not supported.</span></span>|
|<span data-ttu-id="690c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="690c6-116">Application</span></span>|<span data-ttu-id="690c6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690c6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="690c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="690c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="690c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="690c6-119">Request headers</span></span>
|<span data-ttu-id="690c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="690c6-120">Header</span></span>|<span data-ttu-id="690c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="690c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="690c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="690c6-122">Authorization</span></span>|<span data-ttu-id="690c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="690c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="690c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="690c6-124">Accept</span></span>|<span data-ttu-id="690c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="690c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="690c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="690c6-126">Request body</span></span>
<span data-ttu-id="690c6-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="690c6-127">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="690c6-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="690c6-128">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="690c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="690c6-129">Property</span></span>|<span data-ttu-id="690c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="690c6-130">Type</span></span>|<span data-ttu-id="690c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="690c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="690c6-132">id</span><span class="sxs-lookup"><span data-stu-id="690c6-132">id</span></span>|<span data-ttu-id="690c6-133">String</span><span class="sxs-lookup"><span data-stu-id="690c6-133">String</span></span>|<span data-ttu-id="690c6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="690c6-134">Key of the entity.</span></span> <span data-ttu-id="690c6-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="690c6-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="690c6-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="690c6-136">createdDateTime</span></span>|<span data-ttu-id="690c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="690c6-137">DateTimeOffset</span></span>|<span data-ttu-id="690c6-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="690c6-138">DateTime the object was created.</span></span> <span data-ttu-id="690c6-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="690c6-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="690c6-140">description</span><span class="sxs-lookup"><span data-stu-id="690c6-140">description</span></span>|<span data-ttu-id="690c6-141">String</span><span class="sxs-lookup"><span data-stu-id="690c6-141">String</span></span>|<span data-ttu-id="690c6-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="690c6-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="690c6-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="690c6-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="690c6-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="690c6-144">lastModifiedDateTime</span></span>|<span data-ttu-id="690c6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="690c6-145">DateTimeOffset</span></span>|<span data-ttu-id="690c6-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="690c6-146">DateTime the object was last modified.</span></span> <span data-ttu-id="690c6-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="690c6-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="690c6-148">displayName</span><span class="sxs-lookup"><span data-stu-id="690c6-148">displayName</span></span>|<span data-ttu-id="690c6-149">String</span><span class="sxs-lookup"><span data-stu-id="690c6-149">String</span></span>|<span data-ttu-id="690c6-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="690c6-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="690c6-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="690c6-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="690c6-152">version</span><span class="sxs-lookup"><span data-stu-id="690c6-152">version</span></span>|<span data-ttu-id="690c6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="690c6-153">Int32</span></span>|<span data-ttu-id="690c6-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="690c6-154">Version of the device configuration.</span></span> <span data-ttu-id="690c6-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="690c6-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="690c6-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="690c6-156">passwordRequired</span></span>|<span data-ttu-id="690c6-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-157">Boolean</span></span>|<span data-ttu-id="690c6-158">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="690c6-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="690c6-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="690c6-159">passwordBlockSimple</span></span>|<span data-ttu-id="690c6-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-160">Boolean</span></span>|<span data-ttu-id="690c6-161">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="690c6-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="690c6-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="690c6-162">passwordMinimumLength</span></span>|<span data-ttu-id="690c6-163">Int32</span><span class="sxs-lookup"><span data-stu-id="690c6-163">Int32</span></span>|<span data-ttu-id="690c6-164">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="690c6-164">Minimum password length.</span></span> <span data-ttu-id="690c6-165">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="690c6-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="690c6-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="690c6-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="690c6-167">Int32</span><span class="sxs-lookup"><span data-stu-id="690c6-167">Int32</span></span>|<span data-ttu-id="690c6-168">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="690c6-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="690c6-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="690c6-169">passwordRequiredType</span></span>|[<span data-ttu-id="690c6-170">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="690c6-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="690c6-171">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="690c6-171">The required password type.</span></span> <span data-ttu-id="690c6-172">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="690c6-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="690c6-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="690c6-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="690c6-174">Int32</span><span class="sxs-lookup"><span data-stu-id="690c6-174">Int32</span></span>|<span data-ttu-id="690c6-175">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="690c6-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="690c6-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="690c6-176">passwordExpirationDays</span></span>|<span data-ttu-id="690c6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="690c6-177">Int32</span></span>|<span data-ttu-id="690c6-178">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="690c6-178">Number of days before password expiration.</span></span> <span data-ttu-id="690c6-179">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="690c6-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="690c6-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="690c6-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="690c6-181">Int32</span><span class="sxs-lookup"><span data-stu-id="690c6-181">Int32</span></span>|<span data-ttu-id="690c6-182">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="690c6-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="690c6-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="690c6-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="690c6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-184">Boolean</span></span>|<span data-ttu-id="690c6-185">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="690c6-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="690c6-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="690c6-186">osMinimumVersion</span></span>|<span data-ttu-id="690c6-187">String</span><span class="sxs-lookup"><span data-stu-id="690c6-187">String</span></span>|<span data-ttu-id="690c6-188">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="690c6-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="690c6-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="690c6-189">osMaximumVersion</span></span>|<span data-ttu-id="690c6-190">String</span><span class="sxs-lookup"><span data-stu-id="690c6-190">String</span></span>|<span data-ttu-id="690c6-191">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="690c6-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="690c6-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="690c6-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="690c6-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-193">Boolean</span></span>|<span data-ttu-id="690c6-194">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="690c6-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="690c6-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="690c6-195">bitLockerEnabled</span></span>|<span data-ttu-id="690c6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-196">Boolean</span></span>|<span data-ttu-id="690c6-197">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="690c6-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="690c6-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="690c6-198">secureBootEnabled</span></span>|<span data-ttu-id="690c6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-199">Boolean</span></span>|<span data-ttu-id="690c6-200">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="690c6-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="690c6-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="690c6-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="690c6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-202">Boolean</span></span>|<span data-ttu-id="690c6-203">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="690c6-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="690c6-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="690c6-204">storageRequireEncryption</span></span>|<span data-ttu-id="690c6-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="690c6-205">Boolean</span></span>|<span data-ttu-id="690c6-206">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="690c6-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="690c6-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="690c6-207">Response</span></span>
<span data-ttu-id="690c6-208">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="690c6-208">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="690c6-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="690c6-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="690c6-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="690c6-210">Request</span></span>
<span data-ttu-id="690c6-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="690c6-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="690c6-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="690c6-212">Response</span></span>
<span data-ttu-id="690c6-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="690c6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




