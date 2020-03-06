---
title: Criar macOSCompliancePolicy
description: Cria um novo objeto macOSCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2178245ad4038bdfab7cdb19484da07da92bcaa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514428"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="38435-103">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="38435-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="38435-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38435-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38435-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38435-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38435-106">Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="38435-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38435-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38435-107">Prerequisites</span></span>
<span data-ttu-id="38435-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38435-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38435-110">Permission type</span></span>|<span data-ttu-id="38435-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38435-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38435-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38435-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38435-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38435-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38435-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38435-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38435-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38435-115">Not supported.</span></span>|
|<span data-ttu-id="38435-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38435-116">Application</span></span>|<span data-ttu-id="38435-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38435-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38435-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38435-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="38435-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38435-119">Request headers</span></span>
|<span data-ttu-id="38435-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38435-120">Header</span></span>|<span data-ttu-id="38435-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38435-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38435-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38435-122">Authorization</span></span>|<span data-ttu-id="38435-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38435-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38435-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38435-124">Accept</span></span>|<span data-ttu-id="38435-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38435-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38435-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38435-126">Request body</span></span>
<span data-ttu-id="38435-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="38435-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="38435-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="38435-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="38435-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38435-129">Property</span></span>|<span data-ttu-id="38435-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="38435-130">Type</span></span>|<span data-ttu-id="38435-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="38435-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38435-132">id</span><span class="sxs-lookup"><span data-stu-id="38435-132">id</span></span>|<span data-ttu-id="38435-133">String</span><span class="sxs-lookup"><span data-stu-id="38435-133">String</span></span>|<span data-ttu-id="38435-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="38435-134">Key of the entity.</span></span> <span data-ttu-id="38435-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="38435-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="38435-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38435-136">createdDateTime</span></span>|<span data-ttu-id="38435-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38435-137">DateTimeOffset</span></span>|<span data-ttu-id="38435-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="38435-138">DateTime the object was created.</span></span> <span data-ttu-id="38435-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="38435-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="38435-140">description</span><span class="sxs-lookup"><span data-stu-id="38435-140">description</span></span>|<span data-ttu-id="38435-141">String</span><span class="sxs-lookup"><span data-stu-id="38435-141">String</span></span>|<span data-ttu-id="38435-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38435-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38435-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="38435-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="38435-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38435-144">lastModifiedDateTime</span></span>|<span data-ttu-id="38435-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38435-145">DateTimeOffset</span></span>|<span data-ttu-id="38435-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="38435-146">DateTime the object was last modified.</span></span> <span data-ttu-id="38435-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="38435-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="38435-148">displayName</span><span class="sxs-lookup"><span data-stu-id="38435-148">displayName</span></span>|<span data-ttu-id="38435-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38435-149">String</span></span>|<span data-ttu-id="38435-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38435-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38435-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="38435-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="38435-152">version</span><span class="sxs-lookup"><span data-stu-id="38435-152">version</span></span>|<span data-ttu-id="38435-153">Int32</span><span class="sxs-lookup"><span data-stu-id="38435-153">Int32</span></span>|<span data-ttu-id="38435-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38435-154">Version of the device configuration.</span></span> <span data-ttu-id="38435-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="38435-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="38435-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="38435-156">passwordRequired</span></span>|<span data-ttu-id="38435-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="38435-157">Boolean</span></span>|<span data-ttu-id="38435-158">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="38435-158">Whether or not to require a password.</span></span>|
|<span data-ttu-id="38435-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="38435-159">passwordBlockSimple</span></span>|<span data-ttu-id="38435-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="38435-160">Boolean</span></span>|<span data-ttu-id="38435-161">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="38435-161">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="38435-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="38435-162">passwordExpirationDays</span></span>|<span data-ttu-id="38435-163">Int32</span><span class="sxs-lookup"><span data-stu-id="38435-163">Int32</span></span>|<span data-ttu-id="38435-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="38435-164">Number of days before the password expires.</span></span> <span data-ttu-id="38435-165">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="38435-165">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="38435-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="38435-166">passwordMinimumLength</span></span>|<span data-ttu-id="38435-167">Int32</span><span class="sxs-lookup"><span data-stu-id="38435-167">Int32</span></span>|<span data-ttu-id="38435-168">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="38435-168">Minimum length of password.</span></span> <span data-ttu-id="38435-169">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="38435-169">Valid values 4 to 14</span></span>|
|<span data-ttu-id="38435-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="38435-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="38435-171">Int32</span><span class="sxs-lookup"><span data-stu-id="38435-171">Int32</span></span>|<span data-ttu-id="38435-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="38435-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="38435-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="38435-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="38435-174">Int32</span><span class="sxs-lookup"><span data-stu-id="38435-174">Int32</span></span>|<span data-ttu-id="38435-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="38435-175">Number of previous passwords to block.</span></span> <span data-ttu-id="38435-176">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="38435-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="38435-177">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="38435-177">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="38435-178">Int32</span><span class="sxs-lookup"><span data-stu-id="38435-178">Int32</span></span>|<span data-ttu-id="38435-179">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="38435-179">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="38435-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="38435-180">passwordRequiredType</span></span>|[<span data-ttu-id="38435-181">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="38435-181">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="38435-182">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="38435-182">The required password type.</span></span> <span data-ttu-id="38435-183">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="38435-183">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="38435-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="38435-184">osMinimumVersion</span></span>|<span data-ttu-id="38435-185">String</span><span class="sxs-lookup"><span data-stu-id="38435-185">String</span></span>|<span data-ttu-id="38435-186">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="38435-186">Minimum MacOS version.</span></span>|
|<span data-ttu-id="38435-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="38435-187">osMaximumVersion</span></span>|<span data-ttu-id="38435-188">String</span><span class="sxs-lookup"><span data-stu-id="38435-188">String</span></span>|<span data-ttu-id="38435-189">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="38435-189">Maximum MacOS version.</span></span>|
|<span data-ttu-id="38435-190">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="38435-190">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="38435-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="38435-191">Boolean</span></span>|<span data-ttu-id="38435-192">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="38435-192">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="38435-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="38435-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="38435-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="38435-194">Boolean</span></span>|<span data-ttu-id="38435-195">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="38435-195">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="38435-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="38435-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="38435-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="38435-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="38435-198">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="38435-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="38435-199">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="38435-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="38435-200">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="38435-200">storageRequireEncryption</span></span>|<span data-ttu-id="38435-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="38435-201">Boolean</span></span>|<span data-ttu-id="38435-202">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="38435-202">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="38435-203">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="38435-203">firewallEnabled</span></span>|<span data-ttu-id="38435-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="38435-204">Boolean</span></span>|<span data-ttu-id="38435-205">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="38435-205">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="38435-206">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="38435-206">firewallBlockAllIncoming</span></span>|<span data-ttu-id="38435-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="38435-207">Boolean</span></span>|<span data-ttu-id="38435-208">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="38435-208">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="38435-209">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="38435-209">firewallEnableStealthMode</span></span>|<span data-ttu-id="38435-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="38435-210">Boolean</span></span>|<span data-ttu-id="38435-211">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="38435-211">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="38435-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="38435-212">Response</span></span>
<span data-ttu-id="38435-213">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38435-213">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38435-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38435-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="38435-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38435-215">Request</span></span>
<span data-ttu-id="38435-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38435-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="38435-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="38435-217">Response</span></span>
<span data-ttu-id="38435-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38435-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




