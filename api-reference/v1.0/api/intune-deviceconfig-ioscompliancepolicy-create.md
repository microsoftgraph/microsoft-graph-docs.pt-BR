---
title: Criar iosCompliancePolicy
description: Cria um novo objeto iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4fbe648cd1b570994da69457421990f9d03a09b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423473"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="4dd64-103">Criar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4dd64-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="4dd64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dd64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dd64-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4dd64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dd64-106">Cria um novo objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4dd64-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dd64-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4dd64-107">Prerequisites</span></span>
<span data-ttu-id="4dd64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dd64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dd64-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dd64-110">Permission type</span></span>|<span data-ttu-id="4dd64-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4dd64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dd64-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dd64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dd64-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd64-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dd64-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dd64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dd64-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dd64-115">Not supported.</span></span>|
|<span data-ttu-id="4dd64-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dd64-116">Application</span></span>|<span data-ttu-id="4dd64-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dd64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dd64-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dd64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4dd64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dd64-119">Request headers</span></span>
|<span data-ttu-id="4dd64-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dd64-120">Header</span></span>|<span data-ttu-id="4dd64-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4dd64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dd64-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dd64-122">Authorization</span></span>|<span data-ttu-id="4dd64-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dd64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dd64-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4dd64-124">Accept</span></span>|<span data-ttu-id="4dd64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dd64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dd64-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dd64-126">Request body</span></span>
<span data-ttu-id="4dd64-127">No corpo da solicitação, forneça uma representação JSON do objeto iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="4dd64-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="4dd64-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="4dd64-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="4dd64-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dd64-129">Property</span></span>|<span data-ttu-id="4dd64-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dd64-130">Type</span></span>|<span data-ttu-id="4dd64-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dd64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dd64-132">description</span><span class="sxs-lookup"><span data-stu-id="4dd64-132">description</span></span>|<span data-ttu-id="4dd64-133">String</span><span class="sxs-lookup"><span data-stu-id="4dd64-133">String</span></span>|<span data-ttu-id="4dd64-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dd64-134">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4dd64-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dd64-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dd64-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4dd64-136">displayName</span></span>|<span data-ttu-id="4dd64-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dd64-137">String</span></span>|<span data-ttu-id="4dd64-138">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dd64-138">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4dd64-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dd64-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dd64-140">version</span><span class="sxs-lookup"><span data-stu-id="4dd64-140">version</span></span>|<span data-ttu-id="4dd64-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4dd64-141">Int32</span></span>|<span data-ttu-id="4dd64-142">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dd64-142">Version of the device configuration.</span></span> <span data-ttu-id="4dd64-143">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dd64-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4dd64-144">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4dd64-144">passcodeBlockSimple</span></span>|<span data-ttu-id="4dd64-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dd64-145">Boolean</span></span>|<span data-ttu-id="4dd64-146">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4dd64-146">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="4dd64-147">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4dd64-147">passcodeExpirationDays</span></span>|<span data-ttu-id="4dd64-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4dd64-148">Int32</span></span>|<span data-ttu-id="4dd64-149">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="4dd64-149">Number of days before the passcode expires.</span></span> <span data-ttu-id="4dd64-150">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="4dd64-150">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4dd64-151">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4dd64-151">passcodeMinimumLength</span></span>|<span data-ttu-id="4dd64-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4dd64-152">Int32</span></span>|<span data-ttu-id="4dd64-153">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="4dd64-153">Minimum length of passcode.</span></span> <span data-ttu-id="4dd64-154">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="4dd64-154">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4dd64-155">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4dd64-155">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4dd64-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4dd64-156">Int32</span></span>|<span data-ttu-id="4dd64-157">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="4dd64-157">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="4dd64-158">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="4dd64-158">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="4dd64-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4dd64-159">Int32</span></span>|<span data-ttu-id="4dd64-160">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="4dd64-160">Number of previous passcodes to block.</span></span> <span data-ttu-id="4dd64-161">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="4dd64-161">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4dd64-162">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4dd64-162">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="4dd64-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4dd64-163">Int32</span></span>|<span data-ttu-id="4dd64-164">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="4dd64-164">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4dd64-165">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="4dd64-165">passcodeRequiredType</span></span>|[<span data-ttu-id="4dd64-166">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4dd64-166">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4dd64-167">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="4dd64-167">The required passcode type.</span></span> <span data-ttu-id="4dd64-168">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4dd64-168">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4dd64-169">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="4dd64-169">passcodeRequired</span></span>|<span data-ttu-id="4dd64-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dd64-170">Boolean</span></span>|<span data-ttu-id="4dd64-171">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="4dd64-171">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="4dd64-172">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4dd64-172">osMinimumVersion</span></span>|<span data-ttu-id="4dd64-173">String</span><span class="sxs-lookup"><span data-stu-id="4dd64-173">String</span></span>|<span data-ttu-id="4dd64-174">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="4dd64-174">Minimum IOS version.</span></span>|
|<span data-ttu-id="4dd64-175">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4dd64-175">osMaximumVersion</span></span>|<span data-ttu-id="4dd64-176">String</span><span class="sxs-lookup"><span data-stu-id="4dd64-176">String</span></span>|<span data-ttu-id="4dd64-177">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="4dd64-177">Maximum IOS version.</span></span>|
|<span data-ttu-id="4dd64-178">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4dd64-178">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4dd64-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dd64-179">Boolean</span></span>|<span data-ttu-id="4dd64-180">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="4dd64-180">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4dd64-181">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4dd64-181">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4dd64-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dd64-182">Boolean</span></span>|<span data-ttu-id="4dd64-183">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="4dd64-183">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="4dd64-184">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4dd64-184">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4dd64-185">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4dd64-185">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4dd64-186">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="4dd64-186">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4dd64-187">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4dd64-187">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4dd64-188">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="4dd64-188">managedEmailProfileRequired</span></span>|<span data-ttu-id="4dd64-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dd64-189">Boolean</span></span>|<span data-ttu-id="4dd64-190">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="4dd64-190">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="4dd64-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dd64-191">Response</span></span>
<span data-ttu-id="4dd64-192">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dd64-192">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dd64-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dd64-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dd64-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dd64-194">Request</span></span>
<span data-ttu-id="4dd64-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dd64-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4dd64-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dd64-196">Response</span></span>
<span data-ttu-id="4dd64-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dd64-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






