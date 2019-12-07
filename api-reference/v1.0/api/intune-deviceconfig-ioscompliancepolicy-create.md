---
title: Criar iosCompliancePolicy
description: Cria um novo objeto iosCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14e5b083e724faa55483018f5687af89de5232e4
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895333"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="e4397-103">Criar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e4397-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="e4397-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4397-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4397-105">Cria um novo objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4397-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4397-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4397-106">Prerequisites</span></span>
<span data-ttu-id="e4397-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4397-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4397-109">Permission type</span></span>|<span data-ttu-id="e4397-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4397-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4397-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4397-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4397-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4397-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4397-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4397-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4397-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4397-114">Not supported.</span></span>|
|<span data-ttu-id="e4397-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4397-115">Application</span></span>|<span data-ttu-id="e4397-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4397-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4397-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4397-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e4397-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4397-118">Request headers</span></span>
|<span data-ttu-id="e4397-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4397-119">Header</span></span>|<span data-ttu-id="e4397-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e4397-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4397-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4397-121">Authorization</span></span>|<span data-ttu-id="e4397-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4397-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4397-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4397-123">Accept</span></span>|<span data-ttu-id="e4397-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e4397-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4397-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4397-125">Request body</span></span>
<span data-ttu-id="e4397-126">No corpo da solicitação, forneça uma representação JSON do objeto iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="e4397-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="e4397-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="e4397-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="e4397-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4397-128">Property</span></span>|<span data-ttu-id="e4397-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4397-129">Type</span></span>|<span data-ttu-id="e4397-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4397-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4397-131">description</span><span class="sxs-lookup"><span data-stu-id="e4397-131">description</span></span>|<span data-ttu-id="e4397-132">String</span><span class="sxs-lookup"><span data-stu-id="e4397-132">String</span></span>|<span data-ttu-id="e4397-133">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4397-133">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4397-134">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e4397-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4397-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e4397-135">displayName</span></span>|<span data-ttu-id="e4397-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4397-136">String</span></span>|<span data-ttu-id="e4397-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4397-137">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4397-138">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e4397-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4397-139">version</span><span class="sxs-lookup"><span data-stu-id="e4397-139">version</span></span>|<span data-ttu-id="e4397-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e4397-140">Int32</span></span>|<span data-ttu-id="e4397-141">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4397-141">Version of the device configuration.</span></span> <span data-ttu-id="e4397-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e4397-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4397-143">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e4397-143">passcodeBlockSimple</span></span>|<span data-ttu-id="e4397-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="e4397-144">Boolean</span></span>|<span data-ttu-id="e4397-145">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="e4397-145">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="e4397-146">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e4397-146">passcodeExpirationDays</span></span>|<span data-ttu-id="e4397-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e4397-147">Int32</span></span>|<span data-ttu-id="e4397-148">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="e4397-148">Number of days before the passcode expires.</span></span> <span data-ttu-id="e4397-149">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="e4397-149">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e4397-150">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e4397-150">passcodeMinimumLength</span></span>|<span data-ttu-id="e4397-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e4397-151">Int32</span></span>|<span data-ttu-id="e4397-152">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="e4397-152">Minimum length of passcode.</span></span> <span data-ttu-id="e4397-153">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="e4397-153">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e4397-154">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e4397-154">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e4397-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e4397-155">Int32</span></span>|<span data-ttu-id="e4397-156">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="e4397-156">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="e4397-157">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="e4397-157">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="e4397-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e4397-158">Int32</span></span>|<span data-ttu-id="e4397-159">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e4397-159">Number of previous passcodes to block.</span></span> <span data-ttu-id="e4397-160">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="e4397-160">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e4397-161">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e4397-161">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="e4397-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e4397-162">Int32</span></span>|<span data-ttu-id="e4397-163">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="e4397-163">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e4397-164">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="e4397-164">passcodeRequiredType</span></span>|[<span data-ttu-id="e4397-165">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e4397-165">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e4397-166">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e4397-166">The required passcode type.</span></span> <span data-ttu-id="e4397-167">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e4397-167">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e4397-168">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="e4397-168">passcodeRequired</span></span>|<span data-ttu-id="e4397-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="e4397-169">Boolean</span></span>|<span data-ttu-id="e4397-170">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="e4397-170">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="e4397-171">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e4397-171">osMinimumVersion</span></span>|<span data-ttu-id="e4397-172">String</span><span class="sxs-lookup"><span data-stu-id="e4397-172">String</span></span>|<span data-ttu-id="e4397-173">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="e4397-173">Minimum IOS version.</span></span>|
|<span data-ttu-id="e4397-174">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e4397-174">osMaximumVersion</span></span>|<span data-ttu-id="e4397-175">String</span><span class="sxs-lookup"><span data-stu-id="e4397-175">String</span></span>|<span data-ttu-id="e4397-176">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="e4397-176">Maximum IOS version.</span></span>|
|<span data-ttu-id="e4397-177">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="e4397-177">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="e4397-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="e4397-178">Boolean</span></span>|<span data-ttu-id="e4397-179">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="e4397-179">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="e4397-180">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e4397-180">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e4397-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="e4397-181">Boolean</span></span>|<span data-ttu-id="e4397-182">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="e4397-182">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="e4397-183">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e4397-183">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e4397-184">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e4397-184">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e4397-185">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="e4397-185">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e4397-186">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e4397-186">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e4397-187">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="e4397-187">managedEmailProfileRequired</span></span>|<span data-ttu-id="e4397-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4397-188">Boolean</span></span>|<span data-ttu-id="e4397-189">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="e4397-189">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="e4397-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4397-190">Response</span></span>
<span data-ttu-id="e4397-191">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4397-191">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4397-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4397-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4397-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4397-193">Request</span></span>
<span data-ttu-id="e4397-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4397-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4397-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4397-195">Response</span></span>
<span data-ttu-id="e4397-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4397-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




