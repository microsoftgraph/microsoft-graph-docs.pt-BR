---
title: Criar macOSCompliancePolicy
description: Cria um novo objeto macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0874cb0aa02adb95715f60885e7fce5ff6201820
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549800"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="7ff4b-103">Criar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7ff4b-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="7ff4b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff4b-105">Cria um novo objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7ff4b-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ff4b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ff4b-106">Prerequisites</span></span>
<span data-ttu-id="7ff4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ff4b-109">Permission type</span></span>|<span data-ttu-id="7ff4b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ff4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ff4b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff4b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ff4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ff4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-114">Not supported.</span></span>|
|<span data-ttu-id="7ff4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ff4b-115">Application</span></span>|<span data-ttu-id="7ff4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ff4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7ff4b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ff4b-118">Request headers</span></span>
|<span data-ttu-id="7ff4b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ff4b-119">Header</span></span>|<span data-ttu-id="7ff4b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7ff4b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ff4b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ff4b-121">Authorization</span></span>|<span data-ttu-id="7ff4b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ff4b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ff4b-123">Accept</span></span>|<span data-ttu-id="7ff4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ff4b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ff4b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ff4b-125">Request body</span></span>
<span data-ttu-id="7ff4b-126">No corpo da solicitação, forneça uma representação JSON do objeto macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="7ff4b-127">A tabela a seguir mostra as propriedades obrigatórias ao criar macOSCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="7ff4b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ff4b-128">Property</span></span>|<span data-ttu-id="7ff4b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ff4b-129">Type</span></span>|<span data-ttu-id="7ff4b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ff4b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff4b-131">id</span><span class="sxs-lookup"><span data-stu-id="7ff4b-131">id</span></span>|<span data-ttu-id="7ff4b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ff4b-132">String</span></span>|<span data-ttu-id="7ff4b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-133">Key of the entity.</span></span> <span data-ttu-id="7ff4b-134">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff4b-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff4b-135">createdDateTime</span></span>|<span data-ttu-id="7ff4b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ff4b-136">DateTimeOffset</span></span>|<span data-ttu-id="7ff4b-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-137">DateTime the object was created.</span></span> <span data-ttu-id="7ff4b-138">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff4b-139">description</span><span class="sxs-lookup"><span data-stu-id="7ff4b-139">description</span></span>|<span data-ttu-id="7ff4b-140">String</span><span class="sxs-lookup"><span data-stu-id="7ff4b-140">String</span></span>|<span data-ttu-id="7ff4b-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ff4b-142">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff4b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ff4b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7ff4b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ff4b-144">DateTimeOffset</span></span>|<span data-ttu-id="7ff4b-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-145">DateTime the object was last modified.</span></span> <span data-ttu-id="7ff4b-146">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff4b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7ff4b-147">displayName</span></span>|<span data-ttu-id="7ff4b-148">String</span><span class="sxs-lookup"><span data-stu-id="7ff4b-148">String</span></span>|<span data-ttu-id="7ff4b-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ff4b-150">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff4b-151">version</span><span class="sxs-lookup"><span data-stu-id="7ff4b-151">version</span></span>|<span data-ttu-id="7ff4b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff4b-152">Int32</span></span>|<span data-ttu-id="7ff4b-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-153">Version of the device configuration.</span></span> <span data-ttu-id="7ff4b-154">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ff4b-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7ff4b-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7ff4b-155">passwordRequired</span></span>|<span data-ttu-id="7ff4b-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ff4b-156">Boolean</span></span>|<span data-ttu-id="7ff4b-157">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="7ff4b-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7ff4b-158">passwordBlockSimple</span></span>|<span data-ttu-id="7ff4b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ff4b-159">Boolean</span></span>|<span data-ttu-id="7ff4b-160">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="7ff4b-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7ff4b-161">passwordExpirationDays</span></span>|<span data-ttu-id="7ff4b-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff4b-162">Int32</span></span>|<span data-ttu-id="7ff4b-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-163">Number of days before the password expires.</span></span> <span data-ttu-id="7ff4b-164">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="7ff4b-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="7ff4b-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7ff4b-165">passwordMinimumLength</span></span>|<span data-ttu-id="7ff4b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff4b-166">Int32</span></span>|<span data-ttu-id="7ff4b-167">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-167">Minimum length of password.</span></span> <span data-ttu-id="7ff4b-168">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="7ff4b-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="7ff4b-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7ff4b-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7ff4b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff4b-170">Int32</span></span>|<span data-ttu-id="7ff4b-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7ff4b-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7ff4b-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7ff4b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff4b-173">Int32</span></span>|<span data-ttu-id="7ff4b-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-174">Number of previous passwords to block.</span></span> <span data-ttu-id="7ff4b-175">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="7ff4b-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7ff4b-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7ff4b-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7ff4b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7ff4b-177">Int32</span></span>|<span data-ttu-id="7ff4b-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7ff4b-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7ff4b-179">passwordRequiredType</span></span>|[<span data-ttu-id="7ff4b-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7ff4b-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7ff4b-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-181">The required password type.</span></span> <span data-ttu-id="7ff4b-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7ff4b-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7ff4b-183">osMinimumVersion</span></span>|<span data-ttu-id="7ff4b-184">String</span><span class="sxs-lookup"><span data-stu-id="7ff4b-184">String</span></span>|<span data-ttu-id="7ff4b-185">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-185">Minimum MacOS version.</span></span>|
|<span data-ttu-id="7ff4b-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7ff4b-186">osMaximumVersion</span></span>|<span data-ttu-id="7ff4b-187">String</span><span class="sxs-lookup"><span data-stu-id="7ff4b-187">String</span></span>|<span data-ttu-id="7ff4b-188">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-188">Maximum MacOS version.</span></span>|
|<span data-ttu-id="7ff4b-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7ff4b-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="7ff4b-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ff4b-190">Boolean</span></span>|<span data-ttu-id="7ff4b-191">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="7ff4b-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7ff4b-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="7ff4b-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ff4b-193">Boolean</span></span>|<span data-ttu-id="7ff4b-194">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-194">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="7ff4b-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7ff4b-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7ff4b-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="7ff4b-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7ff4b-197">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7ff4b-198">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7ff4b-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7ff4b-199">storageRequireEncryption</span></span>|<span data-ttu-id="7ff4b-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ff4b-200">Boolean</span></span>|<span data-ttu-id="7ff4b-201">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="7ff4b-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="7ff4b-202">firewallEnabled</span></span>|<span data-ttu-id="7ff4b-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ff4b-203">Boolean</span></span>|<span data-ttu-id="7ff4b-204">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="7ff4b-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="7ff4b-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="7ff4b-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ff4b-206">Boolean</span></span>|<span data-ttu-id="7ff4b-207">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="7ff4b-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="7ff4b-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="7ff4b-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="7ff4b-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ff4b-209">Boolean</span></span>|<span data-ttu-id="7ff4b-210">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="7ff4b-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="7ff4b-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ff4b-211">Response</span></span>
<span data-ttu-id="7ff4b-212">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ff4b-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ff4b-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ff4b-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ff4b-214">Request</span></span>
<span data-ttu-id="7ff4b-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ff4b-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ff4b-216">Response</span></span>
<span data-ttu-id="7ff4b-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ff4b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



