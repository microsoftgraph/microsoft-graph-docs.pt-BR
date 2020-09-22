---
title: Atualizar iosCompliancePolicy
description: Atualiza as propriedades de um objeto iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f292e991cdfb32a26538eb703eae9fd710ef95d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066737"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="f66e5-103">Atualizar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f66e5-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="f66e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f66e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f66e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f66e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f66e5-106">Atualiza as propriedades de um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f66e5-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f66e5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f66e5-107">Prerequisites</span></span>
<span data-ttu-id="f66e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f66e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f66e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f66e5-110">Permission type</span></span>|<span data-ttu-id="f66e5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f66e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f66e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f66e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f66e5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f66e5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f66e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f66e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f66e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f66e5-115">Not supported.</span></span>|
|<span data-ttu-id="f66e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f66e5-116">Application</span></span>|<span data-ttu-id="f66e5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f66e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f66e5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f66e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f66e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f66e5-119">Request headers</span></span>
|<span data-ttu-id="f66e5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f66e5-120">Header</span></span>|<span data-ttu-id="f66e5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f66e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f66e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f66e5-122">Authorization</span></span>|<span data-ttu-id="f66e5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f66e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f66e5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f66e5-124">Accept</span></span>|<span data-ttu-id="f66e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f66e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f66e5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f66e5-126">Request body</span></span>
<span data-ttu-id="f66e5-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f66e5-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="f66e5-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f66e5-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="f66e5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f66e5-129">Property</span></span>|<span data-ttu-id="f66e5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f66e5-130">Type</span></span>|<span data-ttu-id="f66e5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f66e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f66e5-132">id</span><span class="sxs-lookup"><span data-stu-id="f66e5-132">id</span></span>|<span data-ttu-id="f66e5-133">String</span><span class="sxs-lookup"><span data-stu-id="f66e5-133">String</span></span>|<span data-ttu-id="f66e5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f66e5-134">Key of the entity.</span></span> <span data-ttu-id="f66e5-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f66e5-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f66e5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f66e5-136">createdDateTime</span></span>|<span data-ttu-id="f66e5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f66e5-137">DateTimeOffset</span></span>|<span data-ttu-id="f66e5-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f66e5-138">DateTime the object was created.</span></span> <span data-ttu-id="f66e5-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f66e5-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f66e5-140">description</span><span class="sxs-lookup"><span data-stu-id="f66e5-140">description</span></span>|<span data-ttu-id="f66e5-141">String</span><span class="sxs-lookup"><span data-stu-id="f66e5-141">String</span></span>|<span data-ttu-id="f66e5-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f66e5-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f66e5-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f66e5-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f66e5-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f66e5-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f66e5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f66e5-145">DateTimeOffset</span></span>|<span data-ttu-id="f66e5-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f66e5-146">DateTime the object was last modified.</span></span> <span data-ttu-id="f66e5-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f66e5-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f66e5-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f66e5-148">displayName</span></span>|<span data-ttu-id="f66e5-149">String</span><span class="sxs-lookup"><span data-stu-id="f66e5-149">String</span></span>|<span data-ttu-id="f66e5-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f66e5-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f66e5-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f66e5-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f66e5-152">version</span><span class="sxs-lookup"><span data-stu-id="f66e5-152">version</span></span>|<span data-ttu-id="f66e5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f66e5-153">Int32</span></span>|<span data-ttu-id="f66e5-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f66e5-154">Version of the device configuration.</span></span> <span data-ttu-id="f66e5-155">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f66e5-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f66e5-156">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f66e5-156">passcodeBlockSimple</span></span>|<span data-ttu-id="f66e5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f66e5-157">Boolean</span></span>|<span data-ttu-id="f66e5-158">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="f66e5-158">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="f66e5-159">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f66e5-159">passcodeExpirationDays</span></span>|<span data-ttu-id="f66e5-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f66e5-160">Int32</span></span>|<span data-ttu-id="f66e5-161">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="f66e5-161">Number of days before the passcode expires.</span></span> <span data-ttu-id="f66e5-162">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="f66e5-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f66e5-163">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f66e5-163">passcodeMinimumLength</span></span>|<span data-ttu-id="f66e5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f66e5-164">Int32</span></span>|<span data-ttu-id="f66e5-165">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="f66e5-165">Minimum length of passcode.</span></span> <span data-ttu-id="f66e5-166">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="f66e5-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f66e5-167">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f66e5-167">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f66e5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f66e5-168">Int32</span></span>|<span data-ttu-id="f66e5-169">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="f66e5-169">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="f66e5-170">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="f66e5-170">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="f66e5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="f66e5-171">Int32</span></span>|<span data-ttu-id="f66e5-172">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f66e5-172">Number of previous passcodes to block.</span></span> <span data-ttu-id="f66e5-173">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="f66e5-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f66e5-174">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f66e5-174">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="f66e5-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f66e5-175">Int32</span></span>|<span data-ttu-id="f66e5-176">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="f66e5-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f66e5-177">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="f66e5-177">passcodeRequiredType</span></span>|[<span data-ttu-id="f66e5-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f66e5-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f66e5-179">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f66e5-179">The required passcode type.</span></span> <span data-ttu-id="f66e5-180">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f66e5-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f66e5-181">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="f66e5-181">passcodeRequired</span></span>|<span data-ttu-id="f66e5-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f66e5-182">Boolean</span></span>|<span data-ttu-id="f66e5-183">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="f66e5-183">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="f66e5-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f66e5-184">osMinimumVersion</span></span>|<span data-ttu-id="f66e5-185">String</span><span class="sxs-lookup"><span data-stu-id="f66e5-185">String</span></span>|<span data-ttu-id="f66e5-186">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="f66e5-186">Minimum IOS version.</span></span>|
|<span data-ttu-id="f66e5-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f66e5-187">osMaximumVersion</span></span>|<span data-ttu-id="f66e5-188">String</span><span class="sxs-lookup"><span data-stu-id="f66e5-188">String</span></span>|<span data-ttu-id="f66e5-189">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="f66e5-189">Maximum IOS version.</span></span>|
|<span data-ttu-id="f66e5-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f66e5-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f66e5-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f66e5-191">Boolean</span></span>|<span data-ttu-id="f66e5-192">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="f66e5-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f66e5-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f66e5-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f66e5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f66e5-194">Boolean</span></span>|<span data-ttu-id="f66e5-195">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="f66e5-195">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="f66e5-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f66e5-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f66e5-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f66e5-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f66e5-198">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="f66e5-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f66e5-199">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="f66e5-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f66e5-200">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="f66e5-200">managedEmailProfileRequired</span></span>|<span data-ttu-id="f66e5-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="f66e5-201">Boolean</span></span>|<span data-ttu-id="f66e5-202">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="f66e5-202">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="f66e5-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="f66e5-203">Response</span></span>
<span data-ttu-id="f66e5-204">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f66e5-204">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f66e5-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f66e5-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="f66e5-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f66e5-206">Request</span></span>
<span data-ttu-id="f66e5-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f66e5-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="f66e5-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="f66e5-208">Response</span></span>
<span data-ttu-id="f66e5-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f66e5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









