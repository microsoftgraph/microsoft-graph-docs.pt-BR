---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 08b256fc12dcfd7d2d5e79f0dc0b277244214a2d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321060"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="5bb41-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5bb41-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="5bb41-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5bb41-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bb41-105">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5bb41-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bb41-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5bb41-106">Prerequisites</span></span>
<span data-ttu-id="5bb41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bb41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb41-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bb41-109">Permission type</span></span>|<span data-ttu-id="5bb41-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5bb41-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb41-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bb41-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5bb41-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb41-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5bb41-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bb41-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb41-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb41-114">Not supported.</span></span>|
|<span data-ttu-id="5bb41-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bb41-115">Application</span></span>|<span data-ttu-id="5bb41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb41-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb41-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb41-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5bb41-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb41-118">Request headers</span></span>
|<span data-ttu-id="5bb41-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bb41-119">Header</span></span>|<span data-ttu-id="5bb41-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5bb41-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb41-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bb41-121">Authorization</span></span>|<span data-ttu-id="5bb41-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bb41-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb41-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5bb41-123">Accept</span></span>|<span data-ttu-id="5bb41-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb41-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb41-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb41-125">Request body</span></span>
<span data-ttu-id="5bb41-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5bb41-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="5bb41-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5bb41-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="5bb41-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb41-128">Property</span></span>|<span data-ttu-id="5bb41-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb41-129">Type</span></span>|<span data-ttu-id="5bb41-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb41-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb41-131">id</span><span class="sxs-lookup"><span data-stu-id="5bb41-131">id</span></span>|<span data-ttu-id="5bb41-132">String</span><span class="sxs-lookup"><span data-stu-id="5bb41-132">String</span></span>|<span data-ttu-id="5bb41-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5bb41-133">Key of the entity.</span></span> <span data-ttu-id="5bb41-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5bb41-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5bb41-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb41-135">createdDateTime</span></span>|<span data-ttu-id="5bb41-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb41-136">DateTimeOffset</span></span>|<span data-ttu-id="5bb41-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5bb41-137">DateTime the object was created.</span></span> <span data-ttu-id="5bb41-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5bb41-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5bb41-139">description</span><span class="sxs-lookup"><span data-stu-id="5bb41-139">description</span></span>|<span data-ttu-id="5bb41-140">String</span><span class="sxs-lookup"><span data-stu-id="5bb41-140">String</span></span>|<span data-ttu-id="5bb41-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5bb41-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5bb41-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5bb41-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5bb41-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb41-143">lastModifiedDateTime</span></span>|<span data-ttu-id="5bb41-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb41-144">DateTimeOffset</span></span>|<span data-ttu-id="5bb41-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5bb41-145">DateTime the object was last modified.</span></span> <span data-ttu-id="5bb41-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5bb41-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5bb41-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5bb41-147">displayName</span></span>|<span data-ttu-id="5bb41-148">String</span><span class="sxs-lookup"><span data-stu-id="5bb41-148">String</span></span>|<span data-ttu-id="5bb41-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5bb41-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5bb41-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5bb41-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5bb41-151">version</span><span class="sxs-lookup"><span data-stu-id="5bb41-151">version</span></span>|<span data-ttu-id="5bb41-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb41-152">Int32</span></span>|<span data-ttu-id="5bb41-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5bb41-153">Version of the device configuration.</span></span> <span data-ttu-id="5bb41-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5bb41-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5bb41-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5bb41-155">passwordRequired</span></span>|<span data-ttu-id="5bb41-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bb41-156">Boolean</span></span>|<span data-ttu-id="5bb41-157">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="5bb41-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="5bb41-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5bb41-158">passwordBlockSimple</span></span>|<span data-ttu-id="5bb41-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="5bb41-159">Boolean</span></span>|<span data-ttu-id="5bb41-160">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="5bb41-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="5bb41-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5bb41-161">passwordExpirationDays</span></span>|<span data-ttu-id="5bb41-162">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb41-162">Int32</span></span>|<span data-ttu-id="5bb41-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="5bb41-163">Number of days before the password expires.</span></span> <span data-ttu-id="5bb41-164">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="5bb41-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="5bb41-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5bb41-165">passwordMinimumLength</span></span>|<span data-ttu-id="5bb41-166">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb41-166">Int32</span></span>|<span data-ttu-id="5bb41-167">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="5bb41-167">Minimum length of password.</span></span> <span data-ttu-id="5bb41-168">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="5bb41-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="5bb41-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5bb41-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5bb41-170">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb41-170">Int32</span></span>|<span data-ttu-id="5bb41-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="5bb41-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5bb41-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5bb41-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5bb41-173">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb41-173">Int32</span></span>|<span data-ttu-id="5bb41-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="5bb41-174">Number of previous passwords to block.</span></span> <span data-ttu-id="5bb41-175">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="5bb41-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5bb41-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5bb41-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5bb41-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5bb41-177">Int32</span></span>|<span data-ttu-id="5bb41-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="5bb41-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5bb41-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5bb41-179">passwordRequiredType</span></span>|[<span data-ttu-id="5bb41-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5bb41-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5bb41-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="5bb41-181">The required password type.</span></span> <span data-ttu-id="5bb41-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5bb41-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5bb41-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5bb41-183">osMinimumVersion</span></span>|<span data-ttu-id="5bb41-184">String</span><span class="sxs-lookup"><span data-stu-id="5bb41-184">String</span></span>|<span data-ttu-id="5bb41-185">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="5bb41-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="5bb41-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5bb41-186">osMaximumVersion</span></span>|<span data-ttu-id="5bb41-187">String</span><span class="sxs-lookup"><span data-stu-id="5bb41-187">String</span></span>|<span data-ttu-id="5bb41-188">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="5bb41-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="5bb41-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5bb41-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="5bb41-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="5bb41-190">Boolean</span></span>|<span data-ttu-id="5bb41-191">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="5bb41-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="5bb41-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5bb41-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5bb41-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bb41-193">Boolean</span></span>|<span data-ttu-id="5bb41-194">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="5bb41-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="5bb41-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5bb41-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5bb41-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="5bb41-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5bb41-197">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="5bb41-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5bb41-198">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5bb41-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5bb41-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5bb41-199">storageRequireEncryption</span></span>|<span data-ttu-id="5bb41-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="5bb41-200">Boolean</span></span>|<span data-ttu-id="5bb41-201">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="5bb41-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="5bb41-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="5bb41-202">firewallEnabled</span></span>|<span data-ttu-id="5bb41-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bb41-203">Boolean</span></span>|<span data-ttu-id="5bb41-204">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="5bb41-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="5bb41-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="5bb41-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="5bb41-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bb41-206">Boolean</span></span>|<span data-ttu-id="5bb41-207">Corresponde à opção "Bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="5bb41-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="5bb41-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="5bb41-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="5bb41-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bb41-209">Boolean</span></span>|<span data-ttu-id="5bb41-210">Corresponde ao "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="5bb41-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="5bb41-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb41-211">Response</span></span>
<span data-ttu-id="5bb41-212">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bb41-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bb41-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bb41-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bb41-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb41-214">Request</span></span>
<span data-ttu-id="5bb41-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bb41-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bb41-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb41-216">Response</span></span>
<span data-ttu-id="5bb41-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bb41-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



