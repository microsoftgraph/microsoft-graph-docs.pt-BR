---
title: Criar macOSCompliancePolicy
description: Cria um novo objeto macOSCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44476093dbcabe5db8a3bd6a8ea18673abd6ecab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753850"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="2f36f-103">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2f36f-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="2f36f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f36f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f36f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f36f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f36f-106">Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f36f-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f36f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f36f-107">Prerequisites</span></span>
<span data-ttu-id="2f36f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f36f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f36f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f36f-110">Permission type</span></span>|<span data-ttu-id="2f36f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f36f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f36f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f36f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f36f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f36f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f36f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f36f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f36f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f36f-115">Not supported.</span></span>|
|<span data-ttu-id="2f36f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f36f-116">Application</span></span>|<span data-ttu-id="2f36f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f36f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f36f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f36f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2f36f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f36f-119">Request headers</span></span>
|<span data-ttu-id="2f36f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f36f-120">Header</span></span>|<span data-ttu-id="2f36f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f36f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f36f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f36f-122">Authorization</span></span>|<span data-ttu-id="2f36f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f36f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f36f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f36f-124">Accept</span></span>|<span data-ttu-id="2f36f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f36f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f36f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f36f-126">Request body</span></span>
<span data-ttu-id="2f36f-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2f36f-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="2f36f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2f36f-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="2f36f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f36f-129">Property</span></span>|<span data-ttu-id="2f36f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f36f-130">Type</span></span>|<span data-ttu-id="2f36f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f36f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f36f-132">id</span><span class="sxs-lookup"><span data-stu-id="2f36f-132">id</span></span>|<span data-ttu-id="2f36f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f36f-133">String</span></span>|<span data-ttu-id="2f36f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f36f-134">Key of the entity.</span></span> <span data-ttu-id="2f36f-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f36f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f36f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f36f-136">createdDateTime</span></span>|<span data-ttu-id="2f36f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f36f-137">DateTimeOffset</span></span>|<span data-ttu-id="2f36f-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f36f-138">DateTime the object was created.</span></span> <span data-ttu-id="2f36f-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f36f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f36f-140">descrição</span><span class="sxs-lookup"><span data-stu-id="2f36f-140">description</span></span>|<span data-ttu-id="2f36f-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f36f-141">String</span></span>|<span data-ttu-id="2f36f-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f36f-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f36f-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f36f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f36f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f36f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2f36f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f36f-145">DateTimeOffset</span></span>|<span data-ttu-id="2f36f-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f36f-146">DateTime the object was last modified.</span></span> <span data-ttu-id="2f36f-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f36f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f36f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2f36f-148">displayName</span></span>|<span data-ttu-id="2f36f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f36f-149">String</span></span>|<span data-ttu-id="2f36f-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f36f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f36f-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f36f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f36f-152">version</span><span class="sxs-lookup"><span data-stu-id="2f36f-152">version</span></span>|<span data-ttu-id="2f36f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2f36f-153">Int32</span></span>|<span data-ttu-id="2f36f-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f36f-154">Version of the device configuration.</span></span> <span data-ttu-id="2f36f-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f36f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f36f-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2f36f-156">passwordRequired</span></span>|<span data-ttu-id="2f36f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f36f-157">Boolean</span></span>|<span data-ttu-id="2f36f-158">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="2f36f-158">Whether or not to require a password.</span></span>|
|<span data-ttu-id="2f36f-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2f36f-159">passwordBlockSimple</span></span>|<span data-ttu-id="2f36f-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f36f-160">Boolean</span></span>|<span data-ttu-id="2f36f-161">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="2f36f-161">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="2f36f-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f36f-162">passwordExpirationDays</span></span>|<span data-ttu-id="2f36f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="2f36f-163">Int32</span></span>|<span data-ttu-id="2f36f-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="2f36f-164">Number of days before the password expires.</span></span> <span data-ttu-id="2f36f-165">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="2f36f-165">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="2f36f-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f36f-166">passwordMinimumLength</span></span>|<span data-ttu-id="2f36f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="2f36f-167">Int32</span></span>|<span data-ttu-id="2f36f-168">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="2f36f-168">Minimum length of password.</span></span> <span data-ttu-id="2f36f-169">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="2f36f-169">Valid values 4 to 14</span></span>|
|<span data-ttu-id="2f36f-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2f36f-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2f36f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2f36f-171">Int32</span></span>|<span data-ttu-id="2f36f-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="2f36f-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2f36f-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f36f-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f36f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="2f36f-174">Int32</span></span>|<span data-ttu-id="2f36f-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="2f36f-175">Number of previous passwords to block.</span></span> <span data-ttu-id="2f36f-176">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="2f36f-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="2f36f-177">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2f36f-177">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2f36f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="2f36f-178">Int32</span></span>|<span data-ttu-id="2f36f-179">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="2f36f-179">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2f36f-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f36f-180">passwordRequiredType</span></span>|[<span data-ttu-id="2f36f-181">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f36f-181">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2f36f-182">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="2f36f-182">The required password type.</span></span> <span data-ttu-id="2f36f-183">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2f36f-183">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2f36f-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2f36f-184">osMinimumVersion</span></span>|<span data-ttu-id="2f36f-185">String</span><span class="sxs-lookup"><span data-stu-id="2f36f-185">String</span></span>|<span data-ttu-id="2f36f-186">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="2f36f-186">Minimum MacOS version.</span></span>|
|<span data-ttu-id="2f36f-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2f36f-187">osMaximumVersion</span></span>|<span data-ttu-id="2f36f-188">String</span><span class="sxs-lookup"><span data-stu-id="2f36f-188">String</span></span>|<span data-ttu-id="2f36f-189">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="2f36f-189">Maximum MacOS version.</span></span>|
|<span data-ttu-id="2f36f-190">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2f36f-190">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="2f36f-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f36f-191">Boolean</span></span>|<span data-ttu-id="2f36f-192">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="2f36f-192">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="2f36f-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2f36f-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2f36f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f36f-194">Boolean</span></span>|<span data-ttu-id="2f36f-195">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="2f36f-195">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="2f36f-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2f36f-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2f36f-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2f36f-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2f36f-198">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2f36f-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2f36f-199">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="2f36f-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2f36f-200">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2f36f-200">storageRequireEncryption</span></span>|<span data-ttu-id="2f36f-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f36f-201">Boolean</span></span>|<span data-ttu-id="2f36f-202">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2f36f-202">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="2f36f-203">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="2f36f-203">firewallEnabled</span></span>|<span data-ttu-id="2f36f-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f36f-204">Boolean</span></span>|<span data-ttu-id="2f36f-205">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="2f36f-205">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="2f36f-206">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="2f36f-206">firewallBlockAllIncoming</span></span>|<span data-ttu-id="2f36f-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f36f-207">Boolean</span></span>|<span data-ttu-id="2f36f-208">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="2f36f-208">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="2f36f-209">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="2f36f-209">firewallEnableStealthMode</span></span>|<span data-ttu-id="2f36f-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f36f-210">Boolean</span></span>|<span data-ttu-id="2f36f-211">Corresponde a "Habilitar o modo de furtividade".</span><span class="sxs-lookup"><span data-stu-id="2f36f-211">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="2f36f-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f36f-212">Response</span></span>
<span data-ttu-id="2f36f-213">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f36f-213">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f36f-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f36f-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f36f-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f36f-215">Request</span></span>
<span data-ttu-id="2f36f-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f36f-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f36f-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f36f-217">Response</span></span>
<span data-ttu-id="2f36f-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f36f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




