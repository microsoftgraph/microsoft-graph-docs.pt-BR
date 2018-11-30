---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
ms.openlocfilehash: 99b4586ee0651a34630b25719425290cf700fef3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004337"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="25490-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="25490-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="25490-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="25490-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25490-105">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="25490-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="25490-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25490-106">Prerequisites</span></span>
<span data-ttu-id="25490-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25490-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25490-109">Permission type</span></span>|<span data-ttu-id="25490-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="25490-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25490-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25490-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25490-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25490-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25490-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25490-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25490-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25490-114">Not supported.</span></span>|
|<span data-ttu-id="25490-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25490-115">Application</span></span>|<span data-ttu-id="25490-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25490-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25490-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25490-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="25490-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25490-118">Request headers</span></span>
|<span data-ttu-id="25490-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="25490-119">Header</span></span>|<span data-ttu-id="25490-120">Valor</span><span class="sxs-lookup"><span data-stu-id="25490-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25490-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="25490-121">Authorization</span></span>|<span data-ttu-id="25490-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25490-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25490-123">Accept</span><span class="sxs-lookup"><span data-stu-id="25490-123">Accept</span></span>|<span data-ttu-id="25490-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25490-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25490-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25490-125">Request body</span></span>
<span data-ttu-id="25490-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="25490-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="25490-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="25490-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="25490-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25490-128">Property</span></span>|<span data-ttu-id="25490-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="25490-129">Type</span></span>|<span data-ttu-id="25490-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="25490-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25490-131">id</span><span class="sxs-lookup"><span data-stu-id="25490-131">id</span></span>|<span data-ttu-id="25490-132">String</span><span class="sxs-lookup"><span data-stu-id="25490-132">String</span></span>|<span data-ttu-id="25490-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="25490-133">Key of the entity.</span></span> <span data-ttu-id="25490-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="25490-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="25490-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25490-135">createdDateTime</span></span>|<span data-ttu-id="25490-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25490-136">DateTimeOffset</span></span>|<span data-ttu-id="25490-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="25490-137">DateTime the object was created.</span></span> <span data-ttu-id="25490-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="25490-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="25490-139">description</span><span class="sxs-lookup"><span data-stu-id="25490-139">description</span></span>|<span data-ttu-id="25490-140">String</span><span class="sxs-lookup"><span data-stu-id="25490-140">String</span></span>|<span data-ttu-id="25490-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25490-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25490-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="25490-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="25490-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25490-143">lastModifiedDateTime</span></span>|<span data-ttu-id="25490-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25490-144">DateTimeOffset</span></span>|<span data-ttu-id="25490-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="25490-145">DateTime the object was last modified.</span></span> <span data-ttu-id="25490-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="25490-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="25490-147">displayName</span><span class="sxs-lookup"><span data-stu-id="25490-147">displayName</span></span>|<span data-ttu-id="25490-148">String</span><span class="sxs-lookup"><span data-stu-id="25490-148">String</span></span>|<span data-ttu-id="25490-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25490-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25490-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="25490-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="25490-151">version</span><span class="sxs-lookup"><span data-stu-id="25490-151">version</span></span>|<span data-ttu-id="25490-152">Int32</span><span class="sxs-lookup"><span data-stu-id="25490-152">Int32</span></span>|<span data-ttu-id="25490-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="25490-153">Version of the device configuration.</span></span> <span data-ttu-id="25490-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="25490-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="25490-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="25490-155">passwordRequired</span></span>|<span data-ttu-id="25490-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-156">Boolean</span></span>|<span data-ttu-id="25490-157">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="25490-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="25490-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="25490-158">passwordBlockSimple</span></span>|<span data-ttu-id="25490-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-159">Boolean</span></span>|<span data-ttu-id="25490-160">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="25490-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="25490-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="25490-161">passwordExpirationDays</span></span>|<span data-ttu-id="25490-162">Int32</span><span class="sxs-lookup"><span data-stu-id="25490-162">Int32</span></span>|<span data-ttu-id="25490-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="25490-163">Number of days before the password expires.</span></span> <span data-ttu-id="25490-164">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="25490-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="25490-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="25490-165">passwordMinimumLength</span></span>|<span data-ttu-id="25490-166">Int32</span><span class="sxs-lookup"><span data-stu-id="25490-166">Int32</span></span>|<span data-ttu-id="25490-167">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="25490-167">Minimum length of password.</span></span> <span data-ttu-id="25490-168">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="25490-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="25490-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="25490-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="25490-170">Int32</span><span class="sxs-lookup"><span data-stu-id="25490-170">Int32</span></span>|<span data-ttu-id="25490-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="25490-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="25490-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="25490-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="25490-173">Int32</span><span class="sxs-lookup"><span data-stu-id="25490-173">Int32</span></span>|<span data-ttu-id="25490-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="25490-174">Number of previous passwords to block.</span></span> <span data-ttu-id="25490-175">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="25490-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="25490-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="25490-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="25490-177">Int32</span><span class="sxs-lookup"><span data-stu-id="25490-177">Int32</span></span>|<span data-ttu-id="25490-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="25490-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="25490-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="25490-179">passwordRequiredType</span></span>|[<span data-ttu-id="25490-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="25490-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="25490-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="25490-181">The required password type.</span></span> <span data-ttu-id="25490-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="25490-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="25490-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="25490-183">osMinimumVersion</span></span>|<span data-ttu-id="25490-184">String</span><span class="sxs-lookup"><span data-stu-id="25490-184">String</span></span>|<span data-ttu-id="25490-185">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="25490-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="25490-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="25490-186">osMaximumVersion</span></span>|<span data-ttu-id="25490-187">String</span><span class="sxs-lookup"><span data-stu-id="25490-187">String</span></span>|<span data-ttu-id="25490-188">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="25490-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="25490-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="25490-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="25490-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-190">Boolean</span></span>|<span data-ttu-id="25490-191">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="25490-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="25490-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="25490-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="25490-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-193">Boolean</span></span>|<span data-ttu-id="25490-194">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="25490-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="25490-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="25490-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="25490-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="25490-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="25490-197">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="25490-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="25490-198">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="25490-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="25490-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="25490-199">storageRequireEncryption</span></span>|<span data-ttu-id="25490-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-200">Boolean</span></span>|<span data-ttu-id="25490-201">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="25490-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="25490-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="25490-202">firewallEnabled</span></span>|<span data-ttu-id="25490-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-203">Boolean</span></span>|<span data-ttu-id="25490-204">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="25490-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="25490-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="25490-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="25490-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-206">Boolean</span></span>|<span data-ttu-id="25490-207">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="25490-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="25490-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="25490-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="25490-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="25490-209">Boolean</span></span>|<span data-ttu-id="25490-210">Corresponde ao "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="25490-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="25490-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="25490-211">Response</span></span>
<span data-ttu-id="25490-212">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25490-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25490-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25490-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="25490-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25490-214">Request</span></span>
<span data-ttu-id="25490-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25490-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="25490-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="25490-216">Response</span></span>
<span data-ttu-id="25490-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25490-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



