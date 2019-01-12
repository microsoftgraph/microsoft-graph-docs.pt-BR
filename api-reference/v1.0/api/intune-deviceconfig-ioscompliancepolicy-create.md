---
title: Criar iosCompliancePolicy
description: Cria um novo objeto iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e46fc768617882852b42765a436dce5444cbef4a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986968"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="9954a-103">Criar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9954a-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="9954a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9954a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9954a-105">Cria um novo objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9954a-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9954a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9954a-106">Prerequisites</span></span>
<span data-ttu-id="9954a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9954a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9954a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9954a-109">Permission type</span></span>|<span data-ttu-id="9954a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9954a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9954a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9954a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9954a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9954a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9954a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9954a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9954a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9954a-114">Not supported.</span></span>|
|<span data-ttu-id="9954a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9954a-115">Application</span></span>|<span data-ttu-id="9954a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9954a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9954a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9954a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9954a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9954a-118">Request headers</span></span>
|<span data-ttu-id="9954a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9954a-119">Header</span></span>|<span data-ttu-id="9954a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9954a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9954a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9954a-121">Authorization</span></span>|<span data-ttu-id="9954a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9954a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9954a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9954a-123">Accept</span></span>|<span data-ttu-id="9954a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9954a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9954a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9954a-125">Request body</span></span>
<span data-ttu-id="9954a-126">No corpo da solicitação, forneça uma representação JSON do objeto iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="9954a-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="9954a-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="9954a-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="9954a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9954a-128">Property</span></span>|<span data-ttu-id="9954a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9954a-129">Type</span></span>|<span data-ttu-id="9954a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9954a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9954a-131">id</span><span class="sxs-lookup"><span data-stu-id="9954a-131">id</span></span>|<span data-ttu-id="9954a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9954a-132">String</span></span>|<span data-ttu-id="9954a-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9954a-133">Key of the entity.</span></span> <span data-ttu-id="9954a-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9954a-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9954a-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9954a-135">createdDateTime</span></span>|<span data-ttu-id="9954a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9954a-136">DateTimeOffset</span></span>|<span data-ttu-id="9954a-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9954a-137">DateTime the object was created.</span></span> <span data-ttu-id="9954a-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9954a-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9954a-139">description</span><span class="sxs-lookup"><span data-stu-id="9954a-139">description</span></span>|<span data-ttu-id="9954a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9954a-140">String</span></span>|<span data-ttu-id="9954a-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9954a-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9954a-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9954a-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9954a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9954a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9954a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9954a-144">DateTimeOffset</span></span>|<span data-ttu-id="9954a-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9954a-145">DateTime the object was last modified.</span></span> <span data-ttu-id="9954a-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9954a-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9954a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9954a-147">displayName</span></span>|<span data-ttu-id="9954a-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9954a-148">String</span></span>|<span data-ttu-id="9954a-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9954a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9954a-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9954a-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9954a-151">version</span><span class="sxs-lookup"><span data-stu-id="9954a-151">version</span></span>|<span data-ttu-id="9954a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9954a-152">Int32</span></span>|<span data-ttu-id="9954a-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9954a-153">Version of the device configuration.</span></span> <span data-ttu-id="9954a-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9954a-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9954a-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9954a-155">passcodeBlockSimple</span></span>|<span data-ttu-id="9954a-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="9954a-156">Boolean</span></span>|<span data-ttu-id="9954a-157">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="9954a-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="9954a-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9954a-158">passcodeExpirationDays</span></span>|<span data-ttu-id="9954a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9954a-159">Int32</span></span>|<span data-ttu-id="9954a-160">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="9954a-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="9954a-161">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="9954a-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9954a-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9954a-162">passcodeMinimumLength</span></span>|<span data-ttu-id="9954a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="9954a-163">Int32</span></span>|<span data-ttu-id="9954a-164">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="9954a-164">Minimum length of passcode.</span></span> <span data-ttu-id="9954a-165">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="9954a-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9954a-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9954a-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9954a-167">Int32</span><span class="sxs-lookup"><span data-stu-id="9954a-167">Int32</span></span>|<span data-ttu-id="9954a-168">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="9954a-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="9954a-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="9954a-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="9954a-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9954a-170">Int32</span></span>|<span data-ttu-id="9954a-171">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="9954a-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="9954a-172">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="9954a-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9954a-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9954a-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="9954a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="9954a-174">Int32</span></span>|<span data-ttu-id="9954a-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="9954a-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9954a-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="9954a-176">passcodeRequiredType</span></span>|[<span data-ttu-id="9954a-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9954a-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9954a-178">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="9954a-178">The required passcode type.</span></span> <span data-ttu-id="9954a-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9954a-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9954a-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="9954a-180">passcodeRequired</span></span>|<span data-ttu-id="9954a-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="9954a-181">Boolean</span></span>|<span data-ttu-id="9954a-182">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="9954a-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="9954a-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9954a-183">osMinimumVersion</span></span>|<span data-ttu-id="9954a-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9954a-184">String</span></span>|<span data-ttu-id="9954a-185">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="9954a-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="9954a-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9954a-186">osMaximumVersion</span></span>|<span data-ttu-id="9954a-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9954a-187">String</span></span>|<span data-ttu-id="9954a-188">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="9954a-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="9954a-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="9954a-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="9954a-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="9954a-190">Boolean</span></span>|<span data-ttu-id="9954a-191">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="9954a-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="9954a-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9954a-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9954a-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="9954a-193">Boolean</span></span>|<span data-ttu-id="9954a-194">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="9954a-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="9954a-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9954a-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9954a-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9954a-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9954a-197">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="9954a-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9954a-198">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="9954a-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9954a-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="9954a-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="9954a-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="9954a-200">Boolean</span></span>|<span data-ttu-id="9954a-201">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="9954a-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="9954a-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="9954a-202">Response</span></span>
<span data-ttu-id="9954a-203">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9954a-203">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9954a-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9954a-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="9954a-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9954a-205">Request</span></span>
<span data-ttu-id="9954a-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9954a-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="9954a-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="9954a-207">Response</span></span>
<span data-ttu-id="9954a-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9954a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



