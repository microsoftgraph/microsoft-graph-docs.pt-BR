---
title: Atualizar windows10MobileCompliancePolicy
description: Atualiza as propriedades de um objeto windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cbfbc758e3457b69a7ae2ef741745531c8a6770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541273"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="3a78a-103">Atualizar windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3a78a-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="3a78a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a78a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a78a-105">Atualiza as propriedades de um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a78a-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a78a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a78a-106">Prerequisites</span></span>
<span data-ttu-id="3a78a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a78a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a78a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a78a-109">Permission type</span></span>|<span data-ttu-id="3a78a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a78a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a78a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a78a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a78a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a78a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a78a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a78a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a78a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a78a-114">Not supported.</span></span>|
|<span data-ttu-id="3a78a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a78a-115">Application</span></span>|<span data-ttu-id="3a78a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a78a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a78a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a78a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3a78a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a78a-118">Request headers</span></span>
|<span data-ttu-id="3a78a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a78a-119">Header</span></span>|<span data-ttu-id="3a78a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3a78a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a78a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a78a-121">Authorization</span></span>|<span data-ttu-id="3a78a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a78a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a78a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a78a-123">Accept</span></span>|<span data-ttu-id="3a78a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a78a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a78a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a78a-125">Request body</span></span>
<span data-ttu-id="3a78a-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a78a-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="3a78a-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a78a-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="3a78a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a78a-128">Property</span></span>|<span data-ttu-id="3a78a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a78a-129">Type</span></span>|<span data-ttu-id="3a78a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a78a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a78a-131">id</span><span class="sxs-lookup"><span data-stu-id="3a78a-131">id</span></span>|<span data-ttu-id="3a78a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a78a-132">String</span></span>|<span data-ttu-id="3a78a-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3a78a-133">Key of the entity.</span></span> <span data-ttu-id="3a78a-134">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3a78a-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a78a-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a78a-135">createdDateTime</span></span>|<span data-ttu-id="3a78a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a78a-136">DateTimeOffset</span></span>|<span data-ttu-id="3a78a-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3a78a-137">DateTime the object was created.</span></span> <span data-ttu-id="3a78a-138">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3a78a-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a78a-139">description</span><span class="sxs-lookup"><span data-stu-id="3a78a-139">description</span></span>|<span data-ttu-id="3a78a-140">String</span><span class="sxs-lookup"><span data-stu-id="3a78a-140">String</span></span>|<span data-ttu-id="3a78a-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3a78a-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a78a-142">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3a78a-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a78a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a78a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3a78a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a78a-144">DateTimeOffset</span></span>|<span data-ttu-id="3a78a-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3a78a-145">DateTime the object was last modified.</span></span> <span data-ttu-id="3a78a-146">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3a78a-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a78a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3a78a-147">displayName</span></span>|<span data-ttu-id="3a78a-148">String</span><span class="sxs-lookup"><span data-stu-id="3a78a-148">String</span></span>|<span data-ttu-id="3a78a-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3a78a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a78a-150">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3a78a-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a78a-151">version</span><span class="sxs-lookup"><span data-stu-id="3a78a-151">version</span></span>|<span data-ttu-id="3a78a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78a-152">Int32</span></span>|<span data-ttu-id="3a78a-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3a78a-153">Version of the device configuration.</span></span> <span data-ttu-id="3a78a-154">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3a78a-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a78a-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3a78a-155">passwordRequired</span></span>|<span data-ttu-id="3a78a-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a78a-156">Boolean</span></span>|<span data-ttu-id="3a78a-157">Exige uma senha para desbloquear o dispositivo Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3a78a-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="3a78a-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3a78a-158">passwordBlockSimple</span></span>|<span data-ttu-id="3a78a-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a78a-159">Boolean</span></span>|<span data-ttu-id="3a78a-160">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3a78a-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="3a78a-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3a78a-161">passwordMinimumLength</span></span>|<span data-ttu-id="3a78a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78a-162">Int32</span></span>|<span data-ttu-id="3a78a-163">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="3a78a-163">Minimum password length.</span></span> <span data-ttu-id="3a78a-164">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="3a78a-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3a78a-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3a78a-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3a78a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78a-166">Int32</span></span>|<span data-ttu-id="3a78a-167">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="3a78a-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3a78a-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3a78a-168">passwordRequiredType</span></span>|[<span data-ttu-id="3a78a-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3a78a-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3a78a-170">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="3a78a-170">The required password type.</span></span> <span data-ttu-id="3a78a-171">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3a78a-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3a78a-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3a78a-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3a78a-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78a-173">Int32</span></span>|<span data-ttu-id="3a78a-174">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="3a78a-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="3a78a-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3a78a-175">passwordExpirationDays</span></span>|<span data-ttu-id="3a78a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78a-176">Int32</span></span>|<span data-ttu-id="3a78a-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="3a78a-177">Number of days before password expiration.</span></span> <span data-ttu-id="3a78a-178">Valores válidos de 1 a 255</span><span class="sxs-lookup"><span data-stu-id="3a78a-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="3a78a-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3a78a-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3a78a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78a-180">Int32</span></span>|<span data-ttu-id="3a78a-181">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="3a78a-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3a78a-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="3a78a-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="3a78a-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a78a-183">Boolean</span></span>|<span data-ttu-id="3a78a-184">Exige uma senha para desbloquear o dispositivo ocioso.</span><span class="sxs-lookup"><span data-stu-id="3a78a-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="3a78a-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3a78a-185">osMinimumVersion</span></span>|<span data-ttu-id="3a78a-186">String</span><span class="sxs-lookup"><span data-stu-id="3a78a-186">String</span></span>|<span data-ttu-id="3a78a-187">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3a78a-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="3a78a-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3a78a-188">osMaximumVersion</span></span>|<span data-ttu-id="3a78a-189">String</span><span class="sxs-lookup"><span data-stu-id="3a78a-189">String</span></span>|<span data-ttu-id="3a78a-190">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3a78a-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="3a78a-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="3a78a-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="3a78a-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a78a-192">Boolean</span></span>|<span data-ttu-id="3a78a-193">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - driver antimalware de inicialização antecipada habilitado.</span><span class="sxs-lookup"><span data-stu-id="3a78a-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="3a78a-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="3a78a-194">bitLockerEnabled</span></span>|<span data-ttu-id="3a78a-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a78a-195">Boolean</span></span>|<span data-ttu-id="3a78a-196">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - bit locker desabilitado</span><span class="sxs-lookup"><span data-stu-id="3a78a-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="3a78a-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="3a78a-197">secureBootEnabled</span></span>|<span data-ttu-id="3a78a-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a78a-198">Boolean</span></span>|<span data-ttu-id="3a78a-199">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows - inicialização segura habilitada.</span><span class="sxs-lookup"><span data-stu-id="3a78a-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="3a78a-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="3a78a-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="3a78a-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a78a-201">Boolean</span></span>|<span data-ttu-id="3a78a-202">Exige que os dispositivos sejam indicados como íntegros pelo Atestado de Integridade do Dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="3a78a-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3a78a-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3a78a-203">storageRequireEncryption</span></span>|<span data-ttu-id="3a78a-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a78a-204">Boolean</span></span>|<span data-ttu-id="3a78a-205">Exige criptografia em dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="3a78a-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="3a78a-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a78a-206">Response</span></span>
<span data-ttu-id="3a78a-207">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a78a-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a78a-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a78a-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a78a-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a78a-209">Request</span></span>
<span data-ttu-id="3a78a-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a78a-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a78a-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a78a-211">Response</span></span>
<span data-ttu-id="3a78a-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a78a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



